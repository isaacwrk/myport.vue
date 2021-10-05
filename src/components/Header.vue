<template>
<v-toolbar style="background-color:#1e1e1e; color:#fff;">
        <v-toolbar-title class="headline text-uppercase mr-4">
            <span>Isaac</span>
            <span class="font-weight-light">Souza</span>
        </v-toolbar-title>
        <v-toolbar-items>
            <v-btn flat to='/'>Início</v-btn>
        </v-toolbar-items>
        <v-spacer></v-spacer>
    <v-toolbar-itens>
        <v-btn icon dark size='24px' :title='midia.ph' v-for="midia in midias" :key="midia">
            <a :href="midia.link" :target="midia.target" style="text-decoration:none;"><v-icon size="24px" color='white'>{{ midia.icn }}</v-icon></a>
        </v-btn>
    </v-toolbar-itens>
</v-toolbar>
</template>

<script>
export default {
    data: () => ({
    midias:[
        {icn:'mdi-gmail',ph:'Gmail',color:'red',target:'_blank',link:'mailto:isaacsouzawrk@gmail.com'},
        {icn:'mdi-linkedin',ph:'Linkedin',color:'blue darken-2',target:'_blank',link:'https://www.linkedin.com/in/isaac-souza-3942a1114/'},
        {icn:'mdi-instagram',ph:'instagram',color:'purple',target:'_blank',link:'https://www.instagram.com/isaacwrk/'},
        {icn:'mdi-github',ph:'Github',color:'black',target:'_blank',link:'https://github.com/isaacwrk'}
    ],
    }),
}
</script>

<style>

</style>