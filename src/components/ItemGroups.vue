<template>
  <v-item-group active-class="primary">
    <v-container>
      <v-row>
        <v-col v-for="n in 4" :key="n" cols="8" md="6">
          <v-item v-slot="{ active, toggle }">
            <v-card
              class="d-flex align-center"
              dark
              height="200"
              @click="toggle"
            >
              <v-scroll-y-transition>
                <div v-if="active" class="text-h2 flex-grow-1 text-center">
                  Active
                </div>
              </v-scroll-y-transition>
            </v-card>
          </v-item>
        </v-col>
      </v-row>
    </v-container>
  </v-item-group>
</template>

<script>
export default {
  name: "ItemGroups",
  data() {},
};
</script>
