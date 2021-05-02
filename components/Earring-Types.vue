<template>
  <v-card
    elevation="2"
    outlined
    class="earring-cards"
  >
    <v-container fluid>
      <v-row dense>
        <v-col
          v-for="card in cards"
          :key="card.title"
          :cols="card.flex"
        >
          <v-card
            elevation="2"
            outlined
            class="earring-card"
          >
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
            />

            <v-card-actions>
              <v-spacer />

              <!-- <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn> -->
              <v-card-title v-text="card.title" />
              <v-btn icon>
                <v-icon>mdi-email-edit-outline</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
// import { gsap } from "gsap";
// import { ScrollTrigger } from "gsap/ScrollTrigger";

export default {
  name: 'EarringTypes',

  // gsap.registerPlugin(ScrollTrigger);

  data: () => ({
    cards: [
      { title: 'Mix-N-Match Earrings', src: 'boba-mixed.jpg', flex: 2 },
      { title: 'Beaded Earrings', src: 'colored-beads.jpg', flex: 2 },
      { title: 'Honeycomb Earrings', src: 'honeycomb.jpg', flex: 2 },
      { title: 'Gummy Bear Earrings', src: 'pink-bears.jpg', flex: 2 },
      { title: 'Zodiac Earrings', src: 'scorpio.jpg', flex: 2 },
      { title: 'Boba Earrings', src: 'brown-boba.jpg', flex: 2 }
    ]
  })
}
</script>

<style lang="scss" scoped>
.earring-cards {
  margin: 2rem 0;

  .earring-card {
    background-color: #FFE57F;
    // white-space: nowrap;
  }
}
</style>
