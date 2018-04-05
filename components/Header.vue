<template lang="pug">
  .header-container
    .header.center(:class="valor1")
      h1.title CSS GRID LAYOUT
      router-link.home(to="/") Home
      router-link.instagram(to="instagram") Instagram
      router-link.platzi(to="platzi") Platzi
      router-link.pinterest(to="pinterest") Pinterest
    Barra

</template>

<script>
import Barra from '~/components/Barra.vue'

export default {
  name: "Header",
  components: { Barra },
  data () {
    return {
      valor: 100
    }
  },

  mounted() {
    this.$bus.$on('valor', (newValor) => {
      this.valor = newValor
    })
  },

  computed: {
    valor1 () {
      return {
        is768: this.valor < 90
      }
    }
  }
}
</script>

<style lang="sass" scoped>
  .red
    border: 1px solid red

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
  
  @media screen and (max-width: 768px)
    .header 
      height: 100px
      grid-template-columns: repeat(4, 1fr)
      grid-template-areas: "title title title title" "home instagram platzi pinterest"

  .is768
    width: 768px
    height: 100px
    grid-template-columns: repeat(4, 1fr)
    grid-template-areas: "title title title title" "home instagram platzi pinterest"
</style>
