<template>
  <div>
    <v-container fluid class="video-container mb-1">
      <v-card>
        <v-card-title>zdz</v-card-title>
        <video autoplay loop muted id="bgvid">
          <source src="@/assets/background-video.mp4" type="video/mp4" />
          <p class="text">HUZEQILdilzdjil</p>
        </video>
      </v-card>
    </v-container>
    <v-container style="height: 1000px">
      <v-row>
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
        <Card />
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>

<style>
.video-container {
  margin-top: 0px;
  width: 100vw;
}
video#bgvid {
  opacity: 10%;
  width: 100%;
  height: 70vh;
  margin: 0;
  padding: 0;
  background: url(@/assets/background.png) no-repeat;
  background-size: cover;
}
</style>
