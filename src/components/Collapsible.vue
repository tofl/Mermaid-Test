<template>
    <div class="collapsible"
         @click="expand"
    >
        <slot name="header">
            <div class="has-background-grey-light p-1">Open Collapsible</div>
        </slot>
    </div>
    <div class="collapsible-content" :id="`collapsible-content-${id}`">
        <slot name="content">
            <div class="has-background-light">
                <p>Content</p>
            </div>
        </slot>
    </div>
</template>

<script>
/* This is a template component for collapsible items.
You must provide a unique id when you using multiple collapsible items
*/

export default {
    name: 'Collapsible',

    props: {
        id: {
            type: String,
            default: 'id',
        },
        collapsed: Boolean,
    },

    watch: {
        collapsed() {
            this.expand();
        },
    },

    mounted() {
        if (!this.collapsed) this.expand();
    },

    methods: {
        expand() {
            const content = document.getElementById(`collapsible-content-${this.id}`);
            if (content.style.maxHeight) {
                content.style.maxHeight = null;
            } else {
                content.style.maxHeight = `${content.scrollHeight}px`;
            }
            this.$emit('collapsed', Boolean(content.style.maxHeight));
        },
    },
};
</script>

<style scoped>
.collapsible-content {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.2s ease-out;
}
</style>
