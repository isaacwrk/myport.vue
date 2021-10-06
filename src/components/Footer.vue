<template>
  <v-footer dark padless>
    <v-card class="flex" flat tile>
      <v-card-text class="py-2 white--text text-center">
        {{ new Date().getFullYear() }} — <a href="https://github.com/isaacwrk" class="text-decoration-none f" target="_blank">Isaacwrk</a>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<style>
.f:hover{ 
  color:white;
}
</style>

<script>
  export default {}
</script>