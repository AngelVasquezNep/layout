<template lang="pug">
  .footer.center
    h4 By Ángel Vásquez 
    p 🚀 Twitter 
      a(href="http://twitter.com/angelvasqueznep", target="_blank") @angelvasqueznep
    p 🐱 
      a(href="https://github.com/angelvasqueznep/layout", target="_blanck") GitHub
</template>

<script>
  export default {
    name: "Footer"
  }
</script>

<style lang="sass" scoped>
  .footer
    height: 70px
    color: #fff 
    background-color: #3B8070
    background-color: #32aaaa
    font-weight: initial
    grid-template-columns: repeat(3, minmax(max-content, 1fr))
    a 
      color: #fff;
      text-decoration: none;
  @media screen and (max-width: 544px)
    .footer
      // grid-template-columns: auto
</style>
