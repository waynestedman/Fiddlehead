<template>
  <v-app>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer
      color="deep-orange lighten-4"
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
