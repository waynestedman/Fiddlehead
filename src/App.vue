<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="mailto:someone@yoursite.com?subject=A Request from Our Visitor"
        target="_blank"
        text
      >
        <span class="mr-2">Contact Us</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HomeContent/>
    </v-main>
    <v-footer
     dark
     padless
    >
      <Footer/>
    </v-footer>
  </v-app>
</template>

<script>
import HomeContent from './components/HomeContent';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    HomeContent,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="sass">
  $color-pack: false

  @import './src/styles/main.scss'
</style>
