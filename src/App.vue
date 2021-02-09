<!-- This file will be used to layout and connect your views -->
<template>
  <div id="app">
      <!-- This is only a basic setup to display your views. Use HTML and CSS to create your layout using these basic commands -->
      <View1 class="v1" />
      <View2 class="v2" />
      <View3 class="v3" />
  </div>
</template>

<script>
// Try to use descriptive names like 'OverviewScatterPlot' or 'DetailLineChart'
import View1 from './components/View1.vue'
import View2 from './components/View2.vue'
import View3 from './components/View3.vue'

export default {
  name: 'App',
  components: {
    View1,
    View2,
    View3
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

  display: grid;
  grid-template-columns: 1fr 10fr 5fr 1fr;
  grid-template-rows: 10vh 50vh 30vh auto;
  grid-template-areas: 
  ". . . ."
  ". ov d1 ."
  ". ov d2 ."
  ". . . .";
}

.v1 {
  grid-area: ov;
}

.v2 {
  grid-area: d1;
}

.v3 {
  grid-area: d2;
}

</style>
