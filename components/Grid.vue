<template lang="pug">
  .Grid
    .item.item1.center Súper animación
    .item.item2.center CSS Grid
    .item.item3.center
      button.btn  Animación 1
    .item.item4.center 
      button.btn  Animación 2
    .item.item5.center
      button.btn  Animación 3
    .item.item6.center
      button.btn  Animación 4
    .item.item7.center Layout
    .item.item8.center
    .item.item9.center
    .item.item10.center
    .item.item11.center
    .item.item12.center
    .item.item13.center
    .item.item14.center
    .item.item15.center
    .item.item16.center
    .item.item17.center
    .item.item18.center
    .item.item19.center
    .item.item20.center
    //- .item.item21.center
</template>

<script>
export default {
  name: 'grid'
}
</script>

<style lang="scss" scoped>
  .Grid {
    box-sizing: border-box;
    // grid-gap: 10px;
    padding: 10px;
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    width: 100%;
    height: 100%;
    @media screen and (max-width: 700px){
      grid-template-columns: repeat(3, 1fr)
    }
    .item {color: #363636}
    .item1{ color: #f1f1f1 }

    grid-template-areas: 
                         "i17 i18 i1  i19 i20"
                         "i3  i8  i7  i9  i6" 
                         "i11 i4  i12 i5  i15" 
                         "i16 i13 i2  i10 i14"
                         ;
    transition: 1s all;
    // animation: move 5s forwards infinite linear alternate;
    @keyframes move {
      0% {
        grid-template-areas: 
                      "i17 i18 i1  i19 i20"
                      "i3  i8  i7  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
      25% {
        grid-template-areas: 
                      "i17 i18 i1  i19 i20"
                      "i3  i8  i7  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
      50% {
        grid-template-areas: 
                      "i17 i18 i1  i19 i20"
                      "i3  i8  i7  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
      75% {
        grid-template-areas: 
                      "i17 i18 i1  i19 i20"
                      "i3  i8  i7  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
      100% {
        grid-template-areas: 
                      "i17 i18 i1  i19 i20"
                      "i3  i8  i7  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
    }
    
    
    
    
    
    
    
    
    
    
    .item1{grid-area: i1; background-color: #0B132B}
    .item2{grid-area: i2; background-color: #F7FFF7}
    .item3{grid-area: i3; background-color: #6FFFE9}
    .item4{grid-area: i4; background-color: #6FFFE9}
    .item5{grid-area: i5; background-color: #6FFFE9}
    .item6{grid-area: i6; background-color: #6FFFE9}
    .item7{grid-area: i7; background-color: #F7FFF7}
    .item8{grid-area: i8; background-color: #1C2541}
    .item9{grid-area: i9; background-color: #3A506B}
    .item10{grid-area: i10; background-color: #1C2541}
    .item11{grid-area: i11; background-color: #3A506B}
    .item12{grid-area: i12; background-color: #5BC0BE}
    .item13{grid-area: i13; background-color: #3A506B}
    .item14{grid-area: i14; background-color: #5BC0BE}
    .item15{grid-area: i15; background-color: #3A506B}
    .item16{grid-area: i16; background-color: #5BC0BE}
    .item17{grid-area: i17; background-color: #0B132B}
    .item18{grid-area: i18; background-color: #0B132B}
    .item19{grid-area: i19; background-color: #0B132B}
    .item20{grid-area: i20; background-color: #0B132B}
  }

</style>
