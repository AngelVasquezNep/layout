<template lang="pug">
  .instagram
    section.headerInsta.center
      .logo 
        p 📷 
        p Instagram
      .buscador
        input(type='search', name='buscador', placeholder='buscar')
      .icons 
        p 🌎  
        p 💜  
        p 👤
       
    section.user
      .perfil.center
        figure.fotoPerfil
          img(src="~/assets/avatar-batman.jpg")
        .datos.center
            h2 BatmanOriginal
            p 
             span 147 
             | publicaciones  
             span 5302 
             | seguidores 
             span 123 
             | seguidos
            p Batman Bruno Díaz 

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
          img(src='~/assets/avatar-batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/acuarela.jpg', alt='')
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
          img(src='~/assets/happiness.jpg', alt='')
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
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/acuarela-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/react.png', alt='')
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
          img(src='~/assets/avatar-batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/acuarela.jpg', alt='')
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
          img(src='~/assets/happiness.jpg', alt='')
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
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/acuarela-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/react.png', alt='')
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
          img(src='~/assets/avatar-batman.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/acuarela.jpg', alt='')
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
          img(src='~/assets/happiness.jpg', alt='')
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
          img(src='~/assets/batman-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/acuarela-1.jpg', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      a.post(href='#')
        figure.post-image
          img(src='~/assets/react.png', alt='')
        span.post-overlay
          p
            span.post-likes 150
            span.post-comments 10
      
      

</template>

<script>
  export default {
    name: "instagram"
  }
</script>

<style lang="sass" scoped>
  .instagram

  .headerInsta
    display: grid
    
    grid-template-columns: repeat(3, minmax(100px, 293px))
    justify-content: center
    align-items: center
    text-align: center
    border-bottom: 1px solid #dcdcdc

  .logo 
    font-size: 2em
    line-height: 50px
    font-family: 'Lobster', cursive

    
  .logo p
    display: inline-block
    padding: 0 10px 
  .logo p:first-child
    border-right: 1px solid grey  

  .icons
    font-size: 2em
    cursor: pointer
    p
      transition: .2s
      display: inline-block
      padding: 5px 10px
      &:active
        transform: scale(.8)

  // Perfil
  .user
    background-color: #FAFAFA
    padding: 30px 0

  .perfil
    margin: 0 auto
    max-width: 1024px
    grid-template-columns: minmax(auto, 300px) 1fr 

  .fotoPerfil
    margin: 0 auto
    position: relative
    width: 150px
    height: 150px
    overflow: hidden
    border-radius: 50% 
    img
      top: -61%
      left: -26%
      position: absolute
      width: 150%

  .datos 
    justify-content: start
    text-align: start
    font-size: 1.1em
    
    span 
      font-weight: bold
  /* Post Insta */

  .post-list
    display: grid
    grid-template-columns: repeat(auto-fill, minmax(100px, 293px))
    justify-content: center
    grid-gap: 39px
    background-color: #FAFAFA
    

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

  .buscador input
    text-align: center
    width: 100%
    padding: 8px
    border: 1px solid #dbdbe2
    border-radius: 5px
    box-sizing: border-box
    outline: none
    &:focus
      box-shadow: 0 0 2px 2px darkcyan

  @media screen and (max-width: 768px)
    .post-list
      grid-gap: 3px
</style>
