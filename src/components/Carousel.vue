<template>
  <v-carousel show-arrows-on-hover height="auto">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
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
          },
          {
            src:'https://github.com/isaacwrk/js-exercises/blob/master/ex/ct1.png?raw=true'
          }
        ],
      }
    },
  }
</script>

<style>
.c{
  width: 1160px;
}
</style>