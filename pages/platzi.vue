<template lang="pug">
  .platzi.center
    h2 🌠 Landing de Platzi 🚀 
    .hero
      .hero-container
        .badge
          img(src="~/assets/react.png", alt='logo')
        h1.title
          | Curso de React.js
        .description
          p
            | React es una de las librerias más utilizadas hoy en aplicaciones web. En este curso podrás dominar la creación de aplicaciones a través de un proyecto que te ayudará a explotar todas las capacidades de esta libreria.
        form.form(@submit.prevent="algo")
          p Registrate
          input(type='text', name='', id='', placeholder='Nombre')
          input(type='email', name='', id='', placeholder='Correo Electrónico')
          button(type='') Comienza ahora
        .countdown
          p Lanzamiento:
          p
            span 01d
            span 03h
            span 09m
            span 05s
    p ¡ Hazlo Responsive para ver la mágia !
</template>

<script>
  export default {
    name: "Platzi",
    methods: {
      algo(){
        console.log("Algo")
      }
    }

  }
</script>

<style lang="sass" scoped>

h2
  color: #23475b
  

.hero
  background-color: #23475b
  color: #fff
  padding: 32px 15px
  display: grid
  grid-template-columns: minmax(auto, 1024px)
  justify-content: center

.hero-container
  display: grid
  grid-template-columns: 70px 1fr 320px
  grid-template-areas: "badge      title   form " " .     description form " " .     countdown   form "  
  grid-gap: 10px

.badge
  grid-area: badge
  width: 70px
  img
    width: 100%

.title
  grid-area: title
  font-size: 36px
  font-weight: normal
  margin: 0
  display: flex
  align-items: center

.description
  grid-area: description

.form
  grid-area: form
  text-align: center
  background-color: rgba(255, 255, 255, 0.9)
  padding: 1.5em
  border-radius: 10px
  input
    width: 100%
    padding: 10px
    font-size: 16px
    border: 1px solid #dbdbe2
    border-radius: 5px
    box-sizing: border-box
    margin-bottom: 10px
    outline: none
    &:focus
      box-shadow: 0 0 2px 2px darkcyan
  p
    font-size: 20px
    color: #3a3b3f
    margin-bottom: 1em
  button
    background-color: #98ca3f
    color: #fff
    padding: 10px 15px
    border-radius: 5px
    border: none
    font-size: 16px
    border-bottom: 5px solid #6d932b
    display: inline-block
    outline: none
    transition: .3s
    &:active
      transform: scale(.95)
.countdown
  grid-area: countdown
  p
    font-size: 20px
    text-align: center
    font-weight: lighter
  span
    font-size: 33px
    &:after
      content: ":"
      display: inline-block
      margin: 0 5px
    &:last-child:after
      display: none

  p
    margin: 0

@media screen and (max-width: 768px)
  .hero-container
    grid-template-columns: 70px 1fr
    grid-template-areas: " badge        title   " " description  description " " form         form    " " countdown    countdown   " 
  .description
    text-align: center

</style>
