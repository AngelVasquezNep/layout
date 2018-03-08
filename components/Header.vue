<template lang="pug">
  .header.center
    h1.title CSS GRID LAYOUT
    router-link.home(to="/") Home
    router-link.instagram(to="instagram") Instagram
    router-link.platzi(to="platzi") Platzi
    router-link.pinterest(to="pinterest") Pinterest
    
</template>

<script>
  export default {
    name: "Header"
  }
</script>

<style lang="sass" scoped>
  .header
    padding: 10px 0
    color: #fff
    grid-template-columns: repeat(6, 1fr)
    grid-template-areas: "title title home instagram platzi pinterest"
    background-color: #32aaaa
    background-color: #3B8070
    margin-bottom: 20px
    
    .title
      grid-area: title
      padding: 0 10px
    .home
      grid-area: home
    .instagram
      grid-area: instagram
    .platzi
      grid-area: platzi
    .pinterest
      grid-area: pinterest
    a 
     color: #fff
     text-transform: uppercase
  
  @media screen and (max-width: 768px)
    .header 
      grid-template-columns: repeat(4, 1fr)
      grid-template-areas: "title title title title" "home instagram platzi pinterest"


</style>
