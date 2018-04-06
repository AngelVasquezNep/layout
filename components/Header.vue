<template lang="pug">
  .header-container
    .header.center
      h1.title CSS GRID LAYOUT
      router-link.home(to="/") Home
      router-link.instagram(to="instagram") Instagram
      router-link.platzi(to="platzi") Platzi
      router-link.pinterest(to="pinterest") Pinterest

</template>

<script>
import Barra from '~/components/Barra.vue'

export default {
  name: "Header",
  data () {
    return {

    }
  },

  mounted() {
    this.$bus.$on('valor', (newValor) => {
      this.valor = newValor
      console.log(newValor)
    })
  }

}
</script>

<style lang="sass" scoped>

  .header-container
    margin: 0 auto
    width: 100%
    justify-content: center

  .header
    padding: 10px 0
    color: #fff
    grid-template-columns: repeat(6, 1fr)
    grid-template-areas: "title title home instagram platzi pinterest"
    background-color: #32aaaa
    background-color: #3B8070
    height: 70px 
    transition: .5s all
    // margin-bottom: 20px
    
    .title
      grid-area: title
      padding: 0 10px
      margin: 0
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
  
  @mixin media768
      height: 100px
      grid-template-columns: repeat(4, 1fr)
      grid-template-areas: "title title title title" "home instagram platzi pinterest"
  
  @media screen and (max-width: 768px)
    .header 
      @include media768

</style>
