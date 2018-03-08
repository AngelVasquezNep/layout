<template lang="pug">
  .instagram
    section.headerInsta.center
      .logo
        | Instagram
      .buscador
        input#buscador(type='search', name='buscador', placeholder='buscar')
      .iconos B
       
    section.user

    section.post-list
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-2.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-3.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-2.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-3.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-2.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-3.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-2.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-3.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-2.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/batman-3.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10

</template>

<script>
  export default {
    name: "Instagram"
  }
</script>

<style lang="sass" scoped>
  .headerInsta
    display: grid
    margin: 20px 0
    padding: 20px 0
    grid-template-columns: repeat(3, minmax(min-content, 293px))
    grid-template-columns: repeat(3, minmax(100px, 293px))
    justify-content: center
    align-items: center
    text-align: center

  /* Post Insta */

  .post-list
    display: grid
    grid-template-columns: repeat(auto-fill, minmax(100px, 293px))
    justify-content: center
    grid-gap: 25px

  .post
    cursor: pointer
    position: relative
    display: flex
    max-height: 293px
    overflow: hidden
    
    justify-content: center
    align-items: center

  .post-image
    height: 293px
    margin: 0
    img
      height: 100%
      vertical-align: auto
    
      
      
  .post-overlay
    background-color: rgba(0, 0, 0, 0.4)
    position: absolute
    left: 0
    right: 0
    top: 0
    bottom: 0
    justify-content: center
    align-items: center
    color: #fff
    text-align: center
    display: none

  .post:hover .post-overlay
    display: flex
    opacity: .1
    transition: .5s
    &:hover
      opacity: 1

  .post-likes, .post-comments
    width: 80px
    margin: 5px
    font-weight: bold
    display: inline-block

  @media screen and (max-width: 768px)
    .post-list
      grid-gap: 3px
</style>
