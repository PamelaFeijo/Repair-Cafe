<template>
  <v-app-bar>
    <v-toolbar-title>Repair Cafe Zuilen</v-toolbar-title>
    <v-spacer />
    <v-list class="d-flex align-center">
      <v-list-item
        link
        v-for="(menu, index) in menus"
        :key="index"
        :to="menu.route"
      >
        <v-list-item-title>{{ menu.title }}</v-list-item-title>
      </v-list-item>
    </v-list>
  </v-app-bar>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      menus: [
        { title: "Home", route: "home" },
        { title: "About us", route: "about-us" },
        { title: "Gallery", route: "gallery" },
        { title: "Contact", route: "contact" }
      ],
    };
  },
};
</script>
