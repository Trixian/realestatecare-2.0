<template>
  <v-card>
    <v-tabs v-model="tab" background-color="transparent" color="basil" grow>
      <v-tab v-for="item in items" :key="item">
        <v-parallax
          img
          src="../../public/logoRealEstatesmall.svg"
          style="padding: 1em"
        />
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in items" :key="item"> </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
export default {
  name: "TabBar",
  data() {
    return {
      tab: null,
      items: ["Home", "Foto toevoegen", "Locatie/Netwerk", "Profiel"],
    };
  },
};
</script>
