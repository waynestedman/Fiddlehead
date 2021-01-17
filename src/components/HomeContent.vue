<template>
  <v-container>
    <v-row class="text-center mb-4">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col>
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to The Fiddlehead Plant!
        </h1>
      </v-col>
    </v-row>

    <v-row class="mb-8">
      <v-col
        cols="4"
      >
        <v-card elevation="2">
          <v-img 
            src="https://via.placeholder.com/400x350" 
            alt=""
            contain
          ></v-img>
        </v-card>
      </v-col>
      <v-col
        cols="6"
      >
        <h2>Intro</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dignissimos fuga perspiciatis unde nobis dolores adipisci enim ullam. Quae hic autem dignissimos illo facilis numquam quas, consequatur rerum magni placeat vero.</p>
      </v-col>      
    </v-row>

    <v-divider></v-divider>

    <v-row class="text-center">
      <v-col>
        <h2>Gallery of earrings</h2>
      </v-col>
    </v-row>
    <v-row class="mb-12">
      <v-col
        v-for="n in 9"
        :key="n"
        class="d-flex child-flex"
        cols="4"
      >
        <v-card elevation="4">
          <v-img
            :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
            :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
            aspect-ratio="1"
            class="grey lighten-2"
          >
            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
              >
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>
        </v-card>
      </v-col>
    </v-row>

    <v-toolbar
      color="indigo"
      dark
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>Gallery of Earrings</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
    </v-toolbar>

    <v-row dense>
      <v-col
        v-for="earring in earrings"
        :key="earring.title"
        :cols="earring.flex"
      >
        <v-card>
          <v-img
            :src="earring.src"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px"
          >
            <v-card-title v-text="earring.title"></v-card-title>
          </v-img>

          <v-card-actions>
            <v-spacer></v-spacer>

            <v-btn icon>
              <v-icon>mdi-heart</v-icon>
            </v-btn>

            <v-btn icon>
              <v-icon>mdi-bookmark</v-icon>
            </v-btn>

            <v-btn icon>
              <v-icon>mdi-share-variant</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
  export default {
    name: 'HomeContent',

    data: () => ({
      earrings: [
        { title: 'Gummy', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 12 },
        { title: 'Zodiac', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 6 },
        { title: 'Honeycomb', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 6 },
      ],
    }),
  }
</script>
