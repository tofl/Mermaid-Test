<template>
  <Collapsible
      :collapsed="true"
      id="pfd"
  >
    <template #header><div class="collapsible-header">PFD</div></template>
    <template #content>
      <Mermaid @click="goToElement"/>
    </template>
  </Collapsible>

  <Collapsible
      :collapsed="false"
      id="energy"
  >
    <template #header><div class="collapsible-header">Energy & Raw Material</div></template>
    <template #content>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vestibulum pellentesque odio ut venenatis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Morbi nec nulla lorem. Etiam rhoncus nulla sed eleifend fermentum. Curabitur consectetur risus in libero iaculis scelerisque. Praesent vel placerat nunc, nec consectetur dui. Nullam in arcu arcu. Morbi rhoncus quam eros, eget mollis tellus ultricies in. Integer tincidunt nunc id justo molestie, in vestibulum dolor interdum. Suspendisse potenti. In eu pulvinar quam. Cras lobortis blandit lorem sed dictum. Nullam a finibus lacus, quis commodo ex. Etiam mollis enim eu varius sollicitudin. Nulla gravida pretium ipsum, a tempor ipsum lacinia sed. Nam nibh velit, semper ut risus vitae, porta tincidunt neque.
        <br /><br />
        Sed ut suscipit quam, quis iaculis justo. Cras venenatis nisl at lacus fringilla, vitae laoreet nisl viverra. Phasellus at iaculis eros, interdum vulputate justo. In facilisis odio sodales, condimentum ligula ut, varius ligula. Sed eget lobortis purus, sit amet maximus neque. Maecenas quis massa at odio viverra pulvinar. Nam lorem elit, suscipit ac mollis eget, efficitur ac turpis. Phasellus pharetra aliquam dui at ultricies. Suspendisse ac nulla eu purus tempus tempus et et sem. Quisque eu lorem felis. Nam quis iaculis ante, non varius nisl. Nunc in ante posuere, lacinia odio consequat, volutpat nisi. Duis eget eleifend sem. Integer viverra odio sem, at aliquet arcu eleifend a. Pellentesque vitae lectus vel massa molestie dapibus.
      </p>
    </template>
  </Collapsible>

  <Collapsible
      :collapsed="false"
      id="equipment"
  >
    <template #header><div class="collapsible-header">Equipment</div></template>
    <template #content>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vestibulum pellentesque odio ut venenatis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Morbi nec nulla lorem. Etiam rhoncus nulla sed eleifend fermentum. Curabitur consectetur risus in libero iaculis scelerisque. Praesent vel placerat nunc, nec consectetur dui. Nullam in arcu arcu. Morbi rhoncus quam eros, eget mollis tellus ultricies in. Integer tincidunt nunc id justo molestie, in vestibulum dolor interdum. Suspendisse potenti. In eu pulvinar quam. Cras lobortis blandit lorem sed dictum. Nullam a finibus lacus, quis commodo ex. Etiam mollis enim eu varius sollicitudin. Nulla gravida pretium ipsum, a tempor ipsum lacinia sed. Nam nibh velit, semper ut risus vitae, porta tincidunt neque.
        <br /><br />
        Sed ut suscipit quam, quis iaculis justo. Cras venenatis nisl at lacus fringilla, vitae laoreet nisl viverra. Phasellus at iaculis eros, interdum vulputate justo. In facilisis odio sodales, condimentum ligula ut, varius ligula. Sed eget lobortis purus, sit amet maximus neque. Maecenas quis massa at odio viverra pulvinar. Nam lorem elit, suscipit ac mollis eget, efficitur ac turpis. Phasellus pharetra aliquam dui at ultricies. Suspendisse ac nulla eu purus tempus tempus et et sem. Quisque eu lorem felis. Nam quis iaculis ante, non varius nisl. Nunc in ante posuere, lacinia odio consequat, volutpat nisi. Duis eget eleifend sem. Integer viverra odio sem, at aliquet arcu eleifend a. Pellentesque vitae lectus vel massa molestie dapibus.
      </p>
    </template>
  </Collapsible>

  <Collapsible
      :collapsed="usesIsCollapsed"
      id="uses"
  >
    <template #header><div class="collapsible-header">Uses & Users</div></template>
    <template #content>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vestibulum pellentesque odio ut venenatis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Morbi nec nulla lorem. Etiam rhoncus nulla sed eleifend fermentum. Curabitur consectetur risus in libero iaculis scelerisque. Praesent vel placerat nunc, nec consectetur dui. Nullam in arcu arcu. Morbi rhoncus quam eros, eget mollis tellus ultricies in. Integer tincidunt nunc id justo molestie, in vestibulum dolor interdum. Suspendisse potenti. In eu pulvinar quam. Cras lobortis blandit lorem sed dictum. Nullam a finibus lacus, quis commodo ex. Etiam mollis enim eu varius sollicitudin. Nulla gravida pretium ipsum, a tempor ipsum lacinia sed. Nam nibh velit, semper ut risus vitae, porta tincidunt neque.
        <br /><br />
        Sed ut suscipit quam, quis iaculis justo. Cras venenatis nisl at lacus fringilla, vitae laoreet nisl viverra. Phasellus at iaculis eros, interdum vulputate justo. In facilisis odio sodales, condimentum ligula ut, varius ligula. Sed eget lobortis purus, sit amet maximus neque. Maecenas quis massa at odio viverra pulvinar. Nam lorem elit, suscipit ac mollis eget, efficitur ac turpis. Phasellus pharetra aliquam dui at ultricies. Suspendisse ac nulla eu purus tempus tempus et et sem. Quisque eu lorem felis. Nam quis iaculis ante, non varius nisl. Nunc in ante posuere, lacinia odio consequat, volutpat nisi. Duis eget eleifend sem. Integer viverra odio sem, at aliquet arcu eleifend a. Pellentesque vitae lectus vel massa molestie dapibus.
      </p>
      <div class="content10" id="go"><strong>GO</strong></div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque vestibulum pellentesque odio ut venenatis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Morbi nec nulla lorem. Etiam rhoncus nulla sed eleifend fermentum. Curabitur consectetur risus in libero iaculis scelerisque. Praesent vel placerat nunc, nec consectetur dui. Nullam in arcu arcu. Morbi rhoncus quam eros, eget mollis tellus ultricies in. Integer tincidunt nunc id justo molestie, in vestibulum dolor interdum. Suspendisse potenti. In eu pulvinar quam. Cras lobortis blandit lorem sed dictum. Nullam a finibus lacus, quis commodo ex. Etiam mollis enim eu varius sollicitudin. Nulla gravida pretium ipsum, a tempor ipsum lacinia sed. Nam nibh velit, semper ut risus vitae, porta tincidunt neque.
        <br />
        Sed ut suscipit quam, quis iaculis justo. Cras venenatis nisl at lacus fringilla, vitae laoreet nisl viverra. Phasellus at iaculis eros, interdum vulputate justo. In facilisis odio sodales, condimentum ligula ut, varius ligula. Sed eget lobortis purus, sit amet maximus neque. Maecenas quis massa at odio viverra pulvinar. Nam lorem elit, suscipit ac mollis eget, efficitur ac turpis. Phasellus pharetra aliquam dui at ultricies. Suspendisse ac nulla eu purus tempus tempus et et sem. Quisque eu lorem felis. Nam quis iaculis ante, non varius nisl. Nunc in ante posuere, lacinia odio consequat, volutpat nisi. Duis eget eleifend sem. Integer viverra odio sem, at aliquet arcu eleifend a. Pellentesque vitae lectus vel massa molestie dapibus.
      </p>
    </template>
  </Collapsible>
</template>

<script>
import Mermaid from './components/Mermaid';
import Collapsible from './components/Collapsible';

export default {
  name: 'App',

  components: {
    Mermaid,
    Collapsible,
  },

  data() {
    return {
      usesIsCollapsed: true,
    };
  },

  methods: {
    goToElement(e) {
      e.preventDefault();
      let target = e.path.filter(el => el.nodeName === 'a'); //[0]; //.href.baseVal;
      if (target.length === 0) return;
      target = target[0].href.baseVal;
      this.usesIsCollapsed = false;
      window.setTimeout(() => document.querySelector(target).scrollIntoView({ behavior: "smooth" }), 100);
    },
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.collapsible {
  margin-top: 40px;
}

.collapsible-header {
  cursor: pointer;
  border-bottom: 1px solid black;
  margin-bottom: 5px;
}

.collapsible-header:hover {
  background-color: lightslategray;
}
</style>
