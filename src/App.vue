<template>
  <v-app>
    <v-header>
      <NavBar />
      <TabBar />
    </v-header>
    <v-main>
      <v-content>
        <router-view></router-view>
        <ItemGroups />
      </v-content>
    </v-main>
    <BottomNavBar />
    <TheFooter />
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import TabBar from "./components/TabBar.vue";
import ItemGroups from "./components/ItemGroups.vue";
import TheFooter from "./components/TheFooter.vue";
export default {
  name: "App",
  components: { NavBar, TabBar, ItemGroups, TheFooter },
  data: () => ({
    //hello
  }),
};
</script>
