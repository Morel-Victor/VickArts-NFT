<template>
  <v-hover>
    <template v-slot:default="{ hover }">
      <v-card class="mx-auto" max-width="325" height="382" elevation="10">
        <v-img class="card white--text" height="200px" :src="img">
          <v-fade-transition>
            <v-overlay v-if="hover" absolute color="overlay">
              <v-btn>Buy On OpenSea</v-btn>
            </v-overlay>
          </v-fade-transition>
          <v-card-title>{{ title }}</v-card-title>
        </v-img>
        <v-card-subtitle class="subtitle pb-2">
          <v-row>
            <v-col cols="7">
              <v-text color="text"> Name : {{ subTitle }} </v-text>
            </v-col>
            <v-col cols="2">
              <v-btn small class="number-btn">{{ categories }}</v-btn>
            </v-col>
            <v-col cols="2">
              <v-btn small class="number-btn">
                <v-text>n° {{ cardNumber }}</v-text>
              </v-btn>
            </v-col>
          </v-row>
        </v-card-subtitle>
        <v-card-text class="text--primary">
          <div>{{ textBody }}</div>
        </v-card-text>
        <v-card-actions>
          <v-btn small class="secondary ml-1">Explore</v-btn>
          <v-spacer></v-spacer>
        </v-card-actions>
      </v-card>
    </template>
  </v-hover>
</template>

<script>
export default {
  name: "Card",
  components: {},
  data() {
    return {
      overlay: false,
      img: "https://cdn.vuetifyjs.com/images/cards/docks.jpg",
      title: "VickArts",
      subTitle: "Fractalicious",
      categories: "UV",
      color: "purple",
      cardNumber: 3,
      textBody:
        "Beautifull card with love eautifull card with love eautifull card with love eautifull card with love ",
    };
  },
};
</script>

<style>
.number-btn {
  border: 2px solid purple;
}
</style>
