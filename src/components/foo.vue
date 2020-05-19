<template>
  <v-footer padless>
    <v-col
      class="text-center"
      cols="12"
    >
      {{ new Date().getFullYear() }} — <strong>Eventv | Team Vengix</strong>
      <a class="secondary--text" style="margin:5px;text-decoration:none" href="">fork on <v-icon size="19">mdi-github</v-icon></a>
    </v-col>
  </v-footer>
</template>
<script>
  export default {
    name: 'foo',

    data: () => ({
      
    }),
  }
</script>
<style scoped>
.pad-r8{
  padding-right: 70px;
}
</style>