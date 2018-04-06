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
  
  a 
    text-decoration: none
    color: #000

  .center
    width: 100%
    display: grid
    margin: 0 auto
    // justify-content: center
    align-items: center
    text-align: center
  
  .default
    display: grid
    grid-template-columns: 1fr 1fr
    min-height: 100vh
    // grid-template-rows: 75px 1fr 100px 

    .myheader
      grid-column: span 2
      // position: fixed

    .nuxt 
      grid-column: span 2

    .myfooter
      grid-column: span 2


</style>
