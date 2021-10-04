<template>
  <v-container fluid grid-list-md>
    <v-layout row wrap>
      <v-flex d-flex xs12 sm6 md4>
        <v-card color="purple" dark>
          <v-card-title primary class="title">Sobre mim</v-card-title>
          <v-card-text>{{lorem}}</v-card-text>
           <v-row class="justify-center" style="cursor: pointer">
          <v-card-subtitle v-for="icon in icons" :key="icon" icon dark >
            <v-icon size='24px' :color='icon.color' :title='icon.ph'>
              {{icon.icn}}
            </v-icon>
        </v-card-subtitle>
      </v-row>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md3>
        <v-layout row wrap>
          <v-flex d-flex>
            <v-card color="indigo" dark>
              <v-card-title primary class="title">Lorem</v-card-title>
              <v-card-text>{{lorem.slice(0,70)}}</v-card-text>
            </v-card>
          </v-flex>
          <v-flex d-flex>
            <v-layout row wrap>
              <v-flex d-flex xs12 v-for="i in 2" :key="i">
                <v-card color="red lighten-2" dark>
                  <v-card-title>Lorem</v-card-title>
                  <v-card-text>{{lorem.slice(0,40)}}</v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-flex>
        </v-layout>
      </v-flex>
      <v-flex d-flex xs12 sm6 md2 child-flex>
            <v-card color="green lighten-2" dark>
              <v-card-title primary class="title">Lorem</v-card-title>
              <v-card-text>{{lorem.slice(0,90)}}</v-card-text>
            </v-card>
          </v-flex>
          <v-flex d-flex xs12 sm6 md3>
            <v-card color="blue lighten-2" dark>
              <v-card-title primary class="title">Lorem</v-card-title>
              <v-card-text>{{lorem.slice(0,100)}}</v-card-text>
            </v-card>
          </v-flex>
    </v-layout>
  </v-container>
</template>

<style>
  .icons{
    white-space: nowrap;
  }
</style>
<script>
export default {
  data () {
    return {
      icons:[
        {icn:'mdi-language-javascript',color:'yellow',ph:'Javascript'},
        {icn:'mdi-vuejs',color:'green',ph:'Vuejs'},
        {icn:'mdi-vuetify',color:'blue darken-2',ph:'Vuetify'},
        {icn:'mdi-angularjs',color:'red',ph:'Angular'},
        {icn:'mdi-react',color:'teal',ph:'Reactjs'}
      ],
      lorem: `Olá sou Isaac, front-end developer de João Pessoa - Paraíba,
        apaixonado por design e por inovação. Já atuei como fullstack contando com experiência em diversos cenários de integração com back e front-end com diversas stacks.
        Atualmente trabalho com front-end com as principais stacks Javascript do mercado.`
    }
  }
}
</script>