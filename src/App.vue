<template>
  <v-app>
    <NavBar />
    <v-main> </v-main>
  </v-app>
</template>

<script>
import NavBar from './components/NavBar.vue';
export default {
  name: "App",
  components: {
    NavBar
  }
};
</script>
