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
    grid-template-rows: auto 1fr auto 

    .myheader
      grid-column: span 2
      // position: fixed

    .nuxt 
      grid-column: span 2

    .myfooter
      grid-column: span 2
  
  .btn 
    text-decoration: none;
    padding: 5px 20px;
    border: 1px solid #1f1f1f;
    border-radius: 5px;
    margin: 0 5px;
    transition: all .1s;
    outline: none;
    background-color: #fff;
    &:hover,
    &:focus 
      color: #fff
      background-color: #42E0C3
      cursor: pointer
    &:active 
      transform: scale(.95)


</style>
