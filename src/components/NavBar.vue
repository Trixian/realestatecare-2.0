<template>
  <v-card class="overflow-hidden" style="height: 4em">
    <v-app-bar
      absolute
      src="../assets/header1.png"
      color="grey lighten-4"
      elevate-on-scroll
      scroll-target="#scrolling-techniques-7"
    >
      <!-- Add Popover menu -->
      <div class="text-center">
        <v-menu
          v-model="menu"
          :close-on-content-click="false"
          :nudge-width="200"
          offset-x
        >
          <template v-slot:activator="{ on, attrs }">
            <v-icon
              v-bind="attrs"
              v-on="on"
              size="24px"
              class="teal--text"
              background-color="transparent"
              left
              padding="1em"
            >
              mdi-menu</v-icon
            >
          </template>

          <v-card>
            <v-list>
              <v-list-item>
                <v-list-item-avatar>
                  <img
                    src="../../public/roundedavatar.png"
                    alt="rounded avatar picture"
                  />
                </v-list-item-avatar>

                <v-list-item-content>
                  <v-list-item-title>Trixian Codes</v-list-item-title>
                  <v-list-item-subtitle
                    >Real Estate Specialist</v-list-item-subtitle
                  >
                </v-list-item-content>

                <v-list-item-action>
                  <v-btn
                    :class="fav ? 'teal--text' : ''"
                    icon
                    @click="fav = !fav"
                  >
                    <v-icon>mdi-home</v-icon>
                  </v-btn>
                </v-list-item-action>
              </v-list-item>
            </v-list>

            <v-divider></v-divider>
            <v-list>
              <v-tooltip bottom>
                <template v-slot:activator="{ on, attrs }">
                  <v-list-item>
                    <v-list-item-action>
                      <v-switch v-model="message" color="teal"></v-switch>
                    </v-list-item-action>
                    <v-list-item-title v-bind="attrs" v-on="on">
                      Locatie</v-list-item-title
                    >
                  </v-list-item></template
                >
                <span
                  >Door locatie actief te zetten worden locatiegegevens
                  automatisch ingevuld.</span
                >
              </v-tooltip>

              <v-list-item>
                <v-list-item-action>
                  <v-switch v-model="hints" color="teal"></v-switch>
                </v-list-item-action>
                <v-list-item-title>Log Uit</v-list-item-title>
              </v-list-item>
            </v-list>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn text @click="menu = false"> Annuleer </v-btn>
            </v-card-actions>
          </v-card>
        </v-menu>
      </div>
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
  data: () => ({
    fav: true,
    menu: false,
    message: false,
    hints: true,
  }),
};
</script>
