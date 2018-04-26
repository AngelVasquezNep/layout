<template lang="pug">
  .Grid
    .item.item1.center 
      img(src="~/assets/lego-1.png", alt="L")
    .item.item2.center 
      img(src="~/assets/lego-2.png", alt="L")
    .item.item3.center 
      img(src="~/assets/lego-5.png", alt="L")
    .item.item4.center 
      //- img(src="~/assets/lego-5.png", alt="L")
      img(src="~/assets/lego-3.png", alt="L")
    .item.item5.center 
      //- img(src="~/assets/lego-5.png", alt="L")
      img(src="~/assets/lego-6.png", alt="L")
    .item.item6.center 
      img(src="~/assets/lego-5.png", alt="L")
    .item.item7.center 
      img(src="~/assets/lego-2.png", alt="L")
    .item.item8.center
      img(src="~/assets/lego-3.png", alt="L")
    .item.item9.center
      //- img(src="~/assets/lego-4.png", alt="L")
      img(src="~/assets/lego-6.png", alt="L")
    .item.item10.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item11.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item12.center
      img(src="~/assets/lego-8.png", alt="L")
    .item.item13.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item14.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item15.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item16.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item17.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item18.center
      //- img(src="~/assets/lego-6.png", alt="L")
      img(src="~/assets/lego-3.png", alt="L")
    .item.item19.center
      //- img(src="~/assets/lego-7.png", alt="L")
      img(src="~/assets/lego-6.png", alt="L")
    .item.item20.center
      img(src="~/assets/lego-2.png", alt="L")
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
    padding: 3px;
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    width: 100%;
    height: 100%;
    .item {
      color: #363636;
      img { margin: 0 auto; max-width: 100%;}
    }

    .item1{ color: #f1f1f1 }

    grid-template-areas: 
                         "i17 i18 i1  i19 i20"
                         "i3  i8  i7  i9  i6" 
                         "i11 i4  i12 i5  i15" 
                         "i16 i13 i2  i10 i14"
                         ;
    transition: 1s all;
    animation: move 10s forwards infinite linear alternate;
    @keyframes move {
      15% {
        grid-template-areas: 
                      "i17 i18 i1  i19 i20"
                      "i3  i8  i7  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
      25% {
        grid-template-areas: 
                      "i17 i18 i7  i19 i20"
                      "i3  i8  i1  i9  i6" 
                      "i11 i4  i12 i5  i15" 
                      "i16 i13 i2  i10 i14"
                      ;
      }
      35% {
        grid-template-areas: 
                      "i17 i8   i7  i9  i20"
                      "i3  i18  i12 i19  i6" 
                      "i11 i4   i1  i5  i15" 
                      "i16 i13  i2  i10 i14"
                      ;
      }
      45% {
        grid-template-areas: 
                      "i3  i8   i7  i9  i6"
                      "i17 i4   i12 i5  i20" 
                      "i11 i18  i2  i19 i15" 
                      "i16 i13  i1  i10 i14"
                      ;
      }
      //Inicio
      55% {
        grid-template-areas: 
                      "i3  i9   i5  i19 i6"
                      "i17 i7   i12 i2  i20" 
                      "i11 i8   i4  i18 i15" 
                      "i16 i13  i1  i10 i14"
                      ;
      }
      65% {
        grid-template-areas: 
                      "i3  i19  i2  i18 i6"
                      "i17 i5   i12 i4  i20" 
                      "i11 i9   i7  i8  i15" 
                      "i16 i13  i1  i10 i14"
                      ;
      }
      75% {
        grid-template-areas: 
                      "i3  i18   i4  i8  i6"
                      "i17 i2   i12 i7  i20" 
                      "i11 i19  i5  i9 i15" 
                      "i16 i13  i1  i10 i14"
                      ;
      }
      85% {
        grid-template-areas: 
                      "i3  i8   i7  i9  i6"
                      "i17 i4   i12 i5  i20" 
                      "i11 i18  i2  i19 i15" 
                      "i16 i13  i1  i10 i14"
                      ;
      }
      // Fin
      95% {
        grid-template-areas: 
                      "i3  i8   i7  i9  i6"
                      "i17 i4   i12 i5  i20" 
                      "i11 i18  i2  i19 i15" 
                      "i16 i13  i1  i10 i14"
                      ;
      }
      100% {
        grid-template-areas: 
                      "i3  i8   i7  i9  i6"
                      "i17 i4   i12 i5  i20" 
                      "i11 i18  i2  i19 i15" 
                      "i16 i13  i1  i10 i14"
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
