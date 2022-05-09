<template>
  <v-app-bar app dark collapse-on-scroll>
    <v-app-bar-nav-icon> </v-app-bar-nav-icon>
    <v-toolbar-title>VickArts</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn icon>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>
    <v-menu left bottom>
      <template v-slot:activator="{ on, attrs }">
        <v-btn icon v-bind="attrs" v-on="on">
          <v-icon>mdi-dots-vertical</v-icon>
        </v-btn>
      </template>
      <v-list>
        <v-list-item v-for="n in 4" :key="n" @click="() => {}">
          Option {{ n }}
        </v-list-item>
      </v-list>
    </v-menu>
  </v-app-bar>
</template>

<script>
export default {
  name: "NavBar",
  components: {},
  data() {
    return {
      title: "VickArts",
    };
  },
};
</script>

<style></style>
