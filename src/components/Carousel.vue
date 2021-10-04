<template>
  <v-carousel show-arrows-on-hover height="100%" :style="{'height': this.carouselHeight}">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      style="height: auto" 
      id="carousel"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    carouselHeight: 0,
    data () {
      return {
        items: [
          {
            src: 'https://github.com/isaacwrk/js-exercises/blob/master/ex/cot.png?raw=true',
          },
          {
            src: 'https://github.com/isaacwrk/js-exercises/blob/master/ex/mmxp.png?raw=true',
          },
          {
            src: 'https://github.com/isaacwrk/login.glassmorphism/blob/master/ex/glass.png?raw=true',
          },
          {
            src: 'https://github.com/isaacwrk/js-exercises/blob/master/ex/js.png?raw=true',
          }
        ],
      }
    },
    methods:{
      getCarouselHeight () {
      var item = document.getElementsByClassName('v-image__image--cover')
      this.carouselHeight = item[0].clientHeight + 'px'
      }
    },
    mounted () {
      this.getCarouselHeight()
    }
  }
</script>

<style>
.c{
  width: 1160px;
}
</style>