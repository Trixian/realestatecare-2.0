<template>
  <v-card class="overflow-hidden" style="height: 4em">
    <v-app-bar
      absolute
      src="../assets/header1.png"
      color="grey lighten-4"
      elevate-on-scroll
      scroll-target="#scrolling-techniques-7"
    >
      <v-app-bar-nav-icon> </v-app-bar-nav-icon>
      <v-toolbar-title class="text-uppercase teal--text">
        <span class="font-weight-light">RealEstate</span>
        <span>Care</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon color="white">mdi-magnify</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon color="white">mdi-heart</v-icon>
      </v-btn>
    </v-app-bar>
    <v-sheet id="scrolling-techniques-7" class="overflow-y-auto">
      <v-container> </v-container>
    </v-sheet>
  </v-card>
</template>

<script>
export default {
  name: "NavBar",
  data() {},
};
</script>
