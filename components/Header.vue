<template lang="pug">
  .header.center
    h1 Proyectos con CSS GRID LAYOUT
    router-link(to="/") Home        
    router-link(to="instagram") Instagram
    router-link(to="platzi") Platzi
    router-link(to="pinterest") Pinterest
    
</template>

<script>
  export default {
    name: "Header"
  }
</script>

<style lang="sass" scoped>
  .header
    color: #fff
    // grid-template-columns: repeat(3, minmax(max-content, 1fr))
    grid-auto-columns: minmax(max-content, 1fr)
    grid-auto-flow: column
    background-color: #32aaaa
    
    h1 
      padding: 0 10px
    a 
     color: #fff
     text-transform: uppercase
</style>
