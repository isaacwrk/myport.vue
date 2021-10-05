<template>
  <v-container fluid grid-list-md>
    <v-layout row wrap>
      <v-flex d-flex xs12 sm6 md4>
        <v-card color="purple darken-2" dark>
          <v-card-title primary class="title">Skills</v-card-title>
          <v-card-text class="about">{{lorem}}</v-card-text>
          <v-row class="justify-center" style="cursor: pointer">
          <v-card-subtitle v-for="icon in icons" :key="icon" icon dark >
            <v-icon size='24px' :color='icon.color' :title='icon.ph'>
              {{icon.icn}}
            </v-icon>
        </v-card-subtitle>
      </v-row>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md4>
        <v-card color="green darken-1" dark>
          <v-card-title primary class="title">Sobre mim</v-card-title>
            <v-card-text class="about">{{about}}</v-card-text>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 sm6 md4>
        <v-card color="red lighten-1" dark>
          <v-card-title primary class="title">Como posso trabalhar para você?</v-card-title>
            <v-card-text class="about">{{work}}</v-card-text>
            <v-card-text class="about">{{work2}}</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<style>
  .icons{
    white-space: nowrap;
  }
  .about{
    font-weight:600;
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
      lorem: `Já atuei como fullstack contando com experiência em diversos cenários de integração com back-end e front-end com diversas stacks.
              Atualmente trabalho com front-end com as principais stacks Javascript do mercado.`,
      about:`Sou natural e residente da cidade de João Pessoa - Paraíba, amante das duas rodas e apaixonado por animais. Busco em meu tempo livre conhecer novos
      destinos desde praias até cidades antigas!`,
      work:`Possuo experiência em projetos freelancer com HTML, CSS, Javascript, ou caso tenha preferência a um framework, trabalho com ReactJs e Vuejs.`,
      work2:`Pode-me contratar por Regime CLT ou por Contrato para freelas! :D`
    }
  }
}
</script>