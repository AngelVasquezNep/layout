<template lang="pug">
  .pinterest
    h2.title Pinterest

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
    name: "Pinterest"
  }
</script>

<style lang="sass" scoped>

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
  font-size: 2rem
  padding: 3px 10px
  display: inline-flex
  font-weight: bold
  border-radius: 50%
  &:hover
    box-shadow: inset 0 -1px 1px 1px red

</style>
