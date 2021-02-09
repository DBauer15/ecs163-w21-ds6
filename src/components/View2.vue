<!-- Your HTML goes here -->
<template>
    <div class='container'>
    <h2>View2</h2>
    <svg viewBox='0 0 800 600'>
        <rect x=5 y=5 width=790 height=590 fill='transparent' stroke='black' stroke-width=5 stroke-dasharray=10 stroke-opacity=0.3 />
        <text x=370 y=70 fill-opacity=0.3>SVG</text>
        <rect x=300 y=200 width=200 height=200 fill='black' fill-opacity=0.3 />
        <text x=370 y=310>Rect</text>
    </svg>
    </div>
</template>

<script>
import * as d3 from 'd3'

export default {
  name: 'View2', // Feel free to rename this and the file
  props: {
      // Feel free to add props to communicate between components
  },
  mounted() {
      this.init()
  },
  methods: {
      init() {
            console.log(d3) // This can be savely removed
          // This will be called when the page loads.
          // You can load your data and setup D3 here
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
    background-color: #b3ffca;    
    display: flex;
    flex-direction: column;
}

.container svg {
    background-color: #77ffa0;
    font-size: 30px;
}
</style>