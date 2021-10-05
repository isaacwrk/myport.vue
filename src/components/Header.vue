<template>
<v-toolbar style="background-color:#747875; color:#fff;">
        <v-toolbar-title class="headline text-uppercase mr-4">
            <span>Isaac</span>
            <span class="font-weight-light">Souza</span>
        </v-toolbar-title>
        <v-toolbar-items>
            <v-btn flat to='/'>Início</v-btn>
        </v-toolbar-items>
        <v-spacer></v-spacer>
        <v-toolbar-itens>
            <v-btn
            v-for="icon in icons"
            :key="icon"
            class="mx-4"
            dark
            icon
        >
        <v-icon size="24px">
            {{ icon }}
        </v-icon>
        </v-btn>
        </v-toolbar-itens>
</v-toolbar>
</template>

<script>
export default {
    data: () => ({
    icons: [
        'mdi-gmail',
        'mdi-linkedin',
        'mdi-instagram',
        'mdi-github'
    ],
    }),
}

</script>

<style>

</style>