<template lang="pug" >
  .container
    h1(v-if="error.statusCode === 404") Página no encontrada
    h1(v-else) Ocurrió un error, recarga la página o ve a la Home:
    router-link.btn(to="/") Home page
</template>

<script>
export default {
  props: ['error']
}
</script>

<style scoped>
.container {
  font-family: sans-serif;
  text-align: center;
}
h1 {
  font-size: 20px;
  margin: 50px 0;
}

.btn {
  padding: 10px 20px;
  border-radius: 5px;
  border: 1px solid #1f1f1f;
  margin: 20px;
}

.btn:hover {
  background-color: #5FBFB5;
  color: #fff;
}
</style>