<template lang="pug">
  .Grid
    .item.item1.center 
      img(src="~/assets/lego-7.png", alt="L")
    .item.item2.center 
      img(src="~/assets/lego-1.png", alt="L")
    .item.item3.center 
      img(src="~/assets/lego-6.png", alt="L")
    .item.item4.center 
      img(src="~/assets/lego-4.png", alt="L")
    .item.item5.center 
      img(src="~/assets/lego-3.png", alt="L")
    
    .item.item6.center 
      //- img(src="~/assets/lego-8.png", alt="L")
      img(src="~/assets/lego-2.png", alt="L")
    .item.item7.center 
      //- img(src="~/assets/lego-5.png", alt="L")
      img(src="~/assets/lego-2.png", alt="L")
    .item.item8.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item9.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item10.center
      img(src="~/assets/lego-2.png", alt="L")
    
    .item.item11.center
      img(src="~/assets/lego-2.png", alt="L")
    .item.item12.center
      img(src="~/assets/lego-2.png", alt="L")
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
      img(src="~/assets/lego-2.png", alt="L")
    .item.item19.center
      img(src="~/assets/lego-2.png", alt="L")
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

    &:hover {
      animation-play-state: pause ;
    }

    .item1{ color: #f1f1f1 }

    grid-template-areas: 
                         "i1  i2  i3  i4  i5"
                         "i6  i7  i8  i9  i10"
                         "i11 i12 i13 i14 i15"
                         "i16 i17 i18 i19 i20"
                         ;
    transition: 1s all;
    animation: move 20s infinite linear 3s;
    @keyframes move {
      5% {
          grid-template-areas: 
                              "i1  i2  i3  i4  i5"
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i16 i17 i18 i19 i20"
                              ;
      }
      10% {
          grid-template-areas: 
                              "i1  i2  i8  i4  i5"
                              "i6  i7  i3  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i16 i17 i18 i19 i20"
                              ;
      }
      15% {
          grid-template-areas: 
                              "i1  i7  i8  i9  i5"
                              "i6  i2  i13 i4  i10"
                              "i11 i12 i3  i14 i15"
                              "i16 i17 i18 i19 i20"
                              ;
      }
      20% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i1  i12 i13 i14 i5"
                              "i11 i2  i18 i4  i15"
                              "i16 i17 i3  i19 i20"
                              ;
      }
      25% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i1  i17 i18 i19 i5"
                              "i16 i2  i3  i4  i20"
                              ;
      }
      30% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i16 i17 i18 i19 i20"
                              "i1  i2  i3  i4  i5"
                              ;
      }
      // LLegaron abajo
      31% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i1  i17 i18 i19 i20"
                              "i16 i2  i3  i4  i5"
                              ;
      }
      32% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i1  i12 i13 i14 i15"
                              "i11 i17 i18 i19 i20"
                              "i16 i2  i3  i4  i5"
                              ;
      }
      33% {
          grid-template-areas: 
                              "i1  i7  i8  i9  i10"
                              "i6  i12 i13 i14 i15"
                              "i11 i17 i18 i19 i20"
                              "i16 i2  i3  i4  i5"
                              ;
      }
      34% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i1  i12 i13 i14 i15"
                              "i11 i17 i18 i19 i20"
                              "i16 i2  i3  i4  i5"
                              ;
      }
      35% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i1  i17 i18 i19 i20"
                              "i16 i2  i3  i4  i5"
                              ;
      }
      36% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i16 i17 i18 i19 i20"
                              "i1  i2  i3  i4  i5"
                              ;
      }
      // Uno bajó
      38% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i14 i15"
                              "i16 i17 i3  i19 i20"
                              "i1  i2  i18 i4  i5"
                              ;
      }
      40% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i10"
                              "i11 i12 i13 i4  i15"
                              "i16 i17 i3  i19 i20"
                              "i1  i2  i18 i14 i5"
                              ;
      }
      42% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i5"
                              "i11 i12 i13 i4  i15"
                              "i16 i17 i3  i19 i20"
                              "i1  i2  i18 i14 i10"
                              ;
      }
      // Escalera arriba
      47% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i5"
                              "i11 i12 i13 i4  i15"
                              "i16 i1  i3  i19 i20"
                              "i17 i2  i18 i14 i10"
                              ;
      }
      52% {
          grid-template-areas: 
                              "i6  i7  i8  i9  i5"
                              "i11 i12 i1  i4  i15"
                              "i16 i13 i3  i19 i20"
                              "i17 i2  i18 i14 i10"
                              ;
      }
      57% {
          grid-template-areas: 
                              "i6  i7  i8  i1  i5"
                              "i11 i12 i9  i4  i15"
                              "i16 i13 i3  i19 i20"
                              "i17 i2  i18 i14 i10"
                              ;
      }
      60% {
          grid-template-areas: 
                              "i6  i7  i8  i15 i1"
                              "i11 i12 i9  i4  i5"
                              "i16 i13 i3  i19 i20"
                              "i17 i2  i18 i14 i10"
                              ;
      }
      62% {
          grid-template-areas: 
                              "i6  i7  i8  i15 i20"
                              "i11 i12 i9  i4  i1"
                              "i16 i13 i3  i19 i5"
                              "i17 i2  i18 i14 i10"
                              ;
      }
      64% {
          grid-template-areas: 
                              "i6  i7  i8  i15 i20"
                              "i11 i12 i9  i4  i10"
                              "i16 i13 i3  i19 i1"
                              "i17 i2  i18 i14 i5"
                              ;
      }
      66% {
          grid-template-areas: 
                              "i6  i7  i8  i15 i20"
                              "i11 i12 i9  i10 i4"
                              "i16 i13 i3  i19 i1"
                              "i17 i2  i18 i14 i5"
                              ;
      }
      68% {
          grid-template-areas: 
                              "i6  i7  i8  i15 i20"
                              "i11 i12 i2  i10 i4"
                              "i16 i13 i3  i19 i1"
                              "i17 i9  i18 i14 i5"
                              ;
      }
      70% {
          grid-template-areas: 
                              "i6  i7  i8  i2  i20"
                              "i11 i12 i15 i10 i4"
                              "i16 i13 i18 i19 i1"
                              "i17 i9  i3  i14 i5"
                              ;
      }
      72% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i2"
                              "i11 i12 i15 i10 i4"
                              "i16 i13 i18 i19 i1"
                              "i17 i9  i3  i14 i5"
                              ;
      }
      74% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i2"
                              "i11 i12 i15 i10 i4"
                              "i16 i13 i18 i19 i1"
                              "i17 i9  i14 i3 i5"
                              ;
      }
      76% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i2"
                              "i16 i13 i18 i19 i4"
                              "i17 i9  i3  i5  i1"
                              ;
      }
      78% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i9"
                              "i16 i13 i18 i19 i2"
                              "i17 i3  i5  i1  i4"
                              ;
      }
      80% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              "i3  i5  i1  i4  i2"
                              ;
      }
      82% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              "i5  i3  i1  i4  i2"
                              ;
      }
      84% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              "i5  i1  i3  i4  i2"
                              ;
      }
      86% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              "i5  i1  i4  i3  i2"
                              ;
      }
      88% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              "i5  i1  i4  i2  i3"
                              ;
      }
      90% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i9  i10"
                              "i16 i13 i18 i19 i3"
                              "i5  i1  i4  i2  i17"
                              ;
      }
      92% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i3"
                              "i16 i13 i18 i2  i17"
                              "i5  i1  i4  i19 i9"
                              ;
      }
      94% {
          grid-template-areas: 
                              "i6  i7  i8  i20 i3"
                              "i11 i12 i15 i2  i14"
                              "i16 i13 i4  i10 i17"
                              "i5  i1  i18 i19 i9"
                              ;
      }
      96% {
          grid-template-areas: 
                              "i6  i7  i8  i2  i3"
                              "i11 i12 i4  i20 i14"
                              "i16 i1  i15 i10 i17"
                              "i5  i13 i18 i19 i9"
                              ;
      }
      98% {
          grid-template-areas: 
                              "i6  i7  i4  i2  i3"
                              "i11 i1  i8  i20 i14"
                              "i5  i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              ;
      }
      100% {
          grid-template-areas: 
                              "i6  i1  i4  i2  i3"
                              "i5  i7  i8  i20 i14"
                              "i11 i12 i15 i10 i17"
                              "i16 i13 i18 i19 i9"
                              ;
      }
    }
    
    
    
    
    
    
    
    
    
    
    .item1{grid-area: i1; background-color: #0B132B}
    .item2{grid-area: i2; background-color: #0B132B}
    .item3{grid-area: i3; background-color: #0B132B}
    .item4{grid-area: i4; background-color: #0B132B}
    .item5{grid-area: i5; background-color: #0B132B}

    .item6{grid-area: i6; background-color: #6FFFE9}
    .item7{grid-area: i7; background-color: #0297D6}
    .item8{grid-area: i8; background-color: #0E6B9D}
    .item9{grid-area: i9; background-color: #0297D6}
    .item10{grid-area: i10; background-color: #6FFFE9}
    
    .item11{grid-area: i11; background-color: #3A506B}
    .item12{grid-area: i12; background-color: #00A8E8}
    .item13{grid-area: i13; background-color: #2EC4B6}
    .item14{grid-area: i14; background-color: #00A8E8}
    .item15{grid-area: i15; background-color: #3A506B}
    
    .item16{grid-area: i16; background-color: #0297D6}
    .item17{grid-area: i17; background-color: #0E6B9D}
    .item18{grid-area: i18; background-color: #0297D6}
    .item19{grid-area: i19; background-color: #0E6B9D}
    .item20{grid-area: i20; background-color: #0297D6}
  }

</style>
