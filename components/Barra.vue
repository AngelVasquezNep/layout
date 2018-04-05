<template lang="pug">
  .barra.center
    p Hazme pequeño para que veas la mágia. Estoy al 
      strong {{ valor }} %
    input.input(type="range", v-model="valor", min="45") 
</template>

<script>
  export default {
    name: 'Barra',
    data () {
      return {
        valor: 100
      }
    },

    watch: {
      valor (newValor, oldValor) {
        this.$bus.$emit('valor', newValor)
        console.log(newValor)
      }
    }
  }
</script>

<style lang="sass" scoped>

.barra
  font-family: 'Courier New', Courier, monospace;
  width: 100%
  color: #1f1f1f
  background-color: #00C485
  justify-content: initial
  .input
    margin: 0px auto
    margin-bottom: 10px
    width: 80%
    
</style>
