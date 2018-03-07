<template lang="pug">
  .default
    my-header.myheader
    nuxt.nuxt
    my-footer.myfooter
</template>

<script>
  import myHeader from '~/components/Header.vue';
  import myFooter from '~/components/Footer.vue';

  export default {
    components: { myHeader, myFooter }
  }
</script>

<style lang="sass" >
  body 
    margin: 0

  .center
    display: grid
    justify-content: center
    justify-items: center
  
  .default
    display: grid
    grid-template-columns: 1fr 1fr
    grid-template-rows: 100px auto 75px 
    min-height: 100vh

    .myheader
      grid-column: span 2

    .nuxt 
      grid-column: span 2

    .myfooter
      grid-column: span 2


</style>
