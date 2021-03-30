<template>
  <v-app>
    <v-app-bar
      app
      color="secondary"
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

      <v-spacer />

      <h2>Welcome to the Fiddlehead Plant</h2>

      <v-spacer />

      <v-btn
        href="mailto:someone@yoursite.com?subject=A Request from Our Visitor"
        target="_blank"
        text
      >
        <v-icon>mdi-mailbox-open</v-icon>
        <span class="ml-2">Contact Us</span>
      </v-btn>
    </v-app-bar>

    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer
      color="secondary darken-3"
      padless
    >
      <Footer />
    </v-footer>
  </v-app>
</template>

<script>
import Footer from '~/components/Footer'

export default {
  components: {
    Footer
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
#app {
  background: rgb(76,175,80);
  background: linear-gradient(0deg, rgba(46,125,50,1) 0%, rgba(76,175,80,1) 55%, rgba(129,199,132,1) 100%);
}
</style>
