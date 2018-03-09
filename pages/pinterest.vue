<template lang="pug">
  .pinterest
    .headerPinterest.center
      .logo
        figure
          img(src='~/assets/batman-3.jpg')
      .buscador
        input(type="search", placeholder="Buscar")
      .opciones
        p 
          a(href="#") Inicio
        p 
          a(href="#") Explorar
        p 
          a(href="#") Batman
        p 
          a(href="#") 🗨️
        p 
          a(href="#") ⚪⚪⚪
      
    .container
      .item.level-3
        img(src='~/assets/pinterest-5.jpg', alt='')
      .item.level-1
        img(src='~/assets/batman-3.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-1.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-4.jpg', alt='')
      .item.level-3
        img(src='~/assets/escaleras.jpg', alt='')
      .item.level-1
        img(src='~/assets/acuarela.jpg', alt='')
      .item.level-3
        img(src='~/assets/pinterest-5.jpg', alt='')
      .item.level-1
        img(src='~/assets/batman-3.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-1.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-4.jpg', alt='')
      .item.level-3
        img(src='~/assets/escaleras.jpg', alt='')
      .item.level-1
        img(src='~/assets/acuarela.jpg', alt='')
      .item.level-3
        img(src='~/assets/pinterest-5.jpg', alt='')
      .item.level-1
        img(src='~/assets/batman-3.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-1.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-4.jpg', alt='')
      .item.level-3
        img(src='~/assets/escaleras.jpg', alt='')
      .item.level-1
        img(src='~/assets/acuarela.jpg', alt='')
      .item.level-3
        img(src='~/assets/pinterest-5.jpg', alt='')
      .item.level-1
        img(src='~/assets/batman-3.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-1.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-4.jpg', alt='')
      .item.level-3
        img(src='~/assets/escaleras.jpg', alt='')
      .item.level-1
        img(src='~/assets/acuarela.jpg', alt='')
      .item.level-3
        img(src='~/assets/pinterest-5.jpg', alt='')
      .item.level-1
        img(src='~/assets/batman-3.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-1.jpg', alt='')
      .item.level-2
        img(src='~/assets/pinterest-4.jpg', alt='')
      .item.level-3
        img(src='~/assets/escaleras.jpg', alt='')
      .item.level-1
        img(src='~/assets/acuarela.jpg', alt='')


</template>

<script>
  export default {
    name: "pinterest"
  }
</script>

<style lang="sass" scoped>

.headerPinterest
  grid-template-columns: 50px 1fr auto
  grid-gap: 10px
  padding: 10px
  border-bottom: 1px solid #dcdcdc
  margin-bottom: 20px
  .logo
    figure
      margin: 0
      width: 100%
      height: 50px
      overflow: hidden
      padding: 10px
      box-sizing: border-box
      position: relative
      border-radius: 50%
      img
        width: 400%
        position: absolute
        left: -82px
        top: -50px
        transform: rotate(-25deg)
  .buscador
    input
      outline: none
      width: 100%
      height: 40px
      border: 1px solid #f1f1f1
      border-radius: 5px
      padding: 0 10px
      font-size: 1.1rem
      background-color: #dcdcdc
      &:focus
        box-shadow: 0 0 0px 3px #8EB5FF

  .opciones
    height: 100%
    p
      display: inline-block
      height: 100%
      margin: 0
      padding: 0
      a
        padding: 0 10px
        align-items: center
        height: 100%
        display: flex
.title
  text-align: center

.container
  display: grid
  grid-template-columns: repeat(auto-fill, 250px)
  grid-gap: 5px
  justify-content: center

.item
  border-radius: 5px
  padding: 10px
  background-color: #f1f1f1
  background-color: #ececec
  img
    max-width: 100%

.level-1
  grid-row-end: span 1

.level-2
  grid-row-end: span 2

.level-3
  grid-row-end: span 3

.level-4
  grid-row-end: span 4

.level-5
  grid-row-end: span 5

p
  padding: 3px 10px
  display: inline-flex

@media screen and (max-width: 544px)
  .headerPinterest
    grid-template-columns: 50px 1fr
    .opciones
      padding: 10px 0
      display: flex
      justify-content: space-evenly
      grid-column: span 2
  .container
    grid-template-columns: repeat(auto-fill, 220px)



</style>
