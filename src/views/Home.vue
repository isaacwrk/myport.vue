<template>
  <v-card class="mx-auto" max-width="100%" outlined>
  <v-list-item-avatar rounded-circle size="200" color="grey" class="avatar">
      <v-img src='https://avatars.githubusercontent.com/u/62186529?v=4'></v-img>
      </v-list-item-avatar>
    <v-list-item>
      <v-list-item-content>
        <div class="text-overline mb-4">
          Olá! eu sou Isaac! seu próximo front-end developer!
        </div>
        <Sobre/>
        <v-list-item-subtitle class="mb-4">Confira alguns dos meus projetos abaixo.</v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>
    <Carousel class="mt-2"/>
  </v-card>
</template>


<script>
import Carousel from '../components/Carousel.vue'
import Sobre from '../components/About.vue'

export default {
  components:{Carousel,Sobre},
}
</script>

<style >
  .main{
    height: 500px;
  }
  .p{
    width: 200px;
    height: 200px;
  }
</style>

