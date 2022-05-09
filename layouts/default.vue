<template>
  <v-app>
    <NavBar />
    <Nuxt />
    <v-footer app>
      <span>&copy; VickArts {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {};
  },
};
</script>
<style scoped>
.main {
  height: 100vh;
}
</style>
