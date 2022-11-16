<template>
  <v-card class="mx-auto" text-wrap>
    <v-container fluid>
      <v-row justfy="space-around">
        <v-col cols="6">
          <v-card v-sheet class="d-flex justify-content-center mb-2 mt-1 pa-12">
            <v-card-text>
              <v-list-item three-line>
                <v-list-item-content>
                  <v-list-item-title>
                    Toegewezen Rapportages
                  </v-list-item-title>
                  <v-list-item-subtitle
                    >Openstaande &amp; in te vullen
                    rapportages</v-list-item-subtitle
                  >
                </v-list-item-content>
                <v-btn fab x-large dark color="teal" class="mx-2">
                  <v-icon tile size="50">mdi-home-plus</v-icon>
                </v-btn>
              </v-list-item>
            </v-card-text>
          </v-card>
        </v-col>
        <!-- Einde item -->
        <v-col cols="6">
          <v-card v-sheet class="d-flex justify-content-center mb-2 mt-1 pa-12">
            <v-card-text>
              <v-list-item three-line>
                <v-list-item-content>
                  <v-list-item-title class="text-8">
                    Uitgevoerde Rapportages
                  </v-list-item-title>
                  <v-list-item-subtitle
                    >Bestaande rapportages inzien &amp;
                    aanpassen</v-list-item-subtitle
                  >
                </v-list-item-content>
                <v-btn fab x-large dark color="teal" class="mx-2">
                  <v-icon tile size="50">mdi-home-search</v-icon>
                </v-btn>
              </v-list-item>
            </v-card-text>
          </v-card>
        </v-col>
        <!-- Einde item -->
        <v-col cols="6">
          <v-card v-sheet class="d-flex justify-content-center mb-2 mt-1 pa-12">
            <v-card-text>
              <v-list-item three-line>
                <v-list-item-content>
                  <v-list-item-title class="text-8">
                    Kennisbase
                  </v-list-item-title>
                  <v-list-item-subtitle
                    >Kennis &amp; documentatie inzien</v-list-item-subtitle
                  >
                </v-list-item-content>
                <v-btn fab x-large dark color="teal" class="mx-2">
                  <v-icon tile size="50">mdi-folder-home</v-icon>
                </v-btn>
              </v-list-item>
            </v-card-text>
          </v-card>
        </v-col>
        <!-- Einde item -->
        <v-col cols="6">
          <v-card v-sheet class="d-flex justify-content-center mb-2 mt-1 pa-12">
            <v-card-text>
              <v-list-item three-line>
                <v-list-item-content>
                  <v-list-item-title class="text-8"> Beheer </v-list-item-title>
                  <v-list-item-subtitle
                    >Instellingen beheren</v-list-item-subtitle
                  >
                </v-list-item-content>
                <v-btn fab x-large dark color="teal" class="mx-2">
                  <v-icon tile size="50">mdi-cog</v-icon>
                </v-btn>
              </v-list-item>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
      <!-- Einde item -->
    </v-container>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    loading: false,
    selection: 1,
  }),

  methods: {
    reserve() {
      this.loading = true;

      setTimeout(() => (this.loading = false), 2000);
    },
  },
};
</script>
