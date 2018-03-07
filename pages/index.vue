<template lang="pug">
  section.index.center
      app-logo
      h1 mi-sitio
      h2 mi otro sitio
      router-link(to="about") Nosotros

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
    // display: grid
    // justify-content: center
    // justify-items: center
</style>
