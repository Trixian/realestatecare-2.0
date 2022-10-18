<template>
  <v-app>
    <NavBar />
    <TabBar />
    <v-content>
      <ItemGroups />
    </v-content>
    <BottomNavBar />
    <TheFooter />
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import TabBar from "./components/TabBar.vue";
import BottomNavBar from "./components/BottomNavBar.vue";
import ItemGroups from "./components/ItemGroups.vue";
import TheFooter from "./components/TheFooter.vue";
export default {
  name: "App",
  components: { NavBar, TabBar, BottomNavBar, ItemGroups, TheFooter },
  data: () => ({
    //hello
  }),
};
</script>
