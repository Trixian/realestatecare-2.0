<template>
  <v-footer color="grey" padless>
    <v-card class="flex" flat tile>
      <v-card-title>
        <v-tabs v-model="tab" grow dark background-color="white">
          <v-tab
            v-for="icon in icons"
            :key="icon"
            class="mx-15"
            style="teal"
            dark
            icon
          >
            <v-icon size="24px" class="teal--text">
              {{ icon }}
            </v-icon>
          </v-tab>
        </v-tabs>
      </v-card-title>

      <v-card-text class="py-2 text-center">
        <strong>
          <v-footer-title class="text-uppercase teal--text">
            <span class="font-weight-light">RealEstate</span>
            <span>Care</span>
          </v-footer-title>
        </strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    icons: ["mdi-facebook", "mdi-linkedin"],
  }),
};
</script>
