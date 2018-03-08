<template lang="pug">
  section.index.center
      app-logo
      h1 CSS GRID LAYOUT
      p ¡ Bienvenidos !
      p Este es una proyecto que nace del curso de CSS GRID LAYOUT de Platzi. 
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style lang="sass" scoped>
  .index
    font-size: 1.3em
</style>
