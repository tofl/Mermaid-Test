<template>
    <div class="container">
        <button @click="swapCharts">Swap charts</button>
        <div id="mermaid">
            <div ref="mermaidVal"></div>
        </div>
    </div>
</template>

<script>
    import mermaid from 'mermaid';
    import chart1 from 'raw-loader!../assets/chart1.md';
    import chart2 from 'raw-loader!../assets/chart2.md';

    export default {
        name: 'Mermaid',

        data() {
            return {
                currentChart: 'chart1',
                chart: chart1,
            };
        },

        mounted() {
            // Documentation : https://github.com/mermaidjs/mermaid-gitbook/blob/master/content/usage.md
            mermaid.mermaidAPI.initialize({
                startOnLoad: true,
                securityLevel: 'loose',
                theme: 'neutral',
            });
            this.renderGraph();
        },

        methods: {
            renderGraph() {
                mermaid.mermaidAPI.render('mermaidVal', this.chart, (svgCode) => {
                    this.$refs.mermaidVal.innerHTML = svgCode;
                });
            },

            swapCharts() {
                if (this.currentChart === 'chart1') {
                    this.chart = chart2;
                    this.currentChart = 'chart2';
                } else {
                    this.chart = chart1;
                    this.currentChart = 'chart1';
                }
                this.renderGraph();
            },
        },
    }
</script>

<style scoped>
    .container {
        border: 1px solid black;
        min-height: 600px;
    }
</style>
