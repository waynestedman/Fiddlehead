<template>
  <v-app>
    <v-header>
      <Header />
    </v-header>
    <v-main>
      <v-container>
        <!-- <nuxt /> -->
        <Home />
      </v-container>
    </v-main>
    <v-footer
      padless
    >
      <Footer />
    </v-footer>
  </v-app>
</template>

<script>
import Header from '@/components/Header'
import Home from '@/pages/Home'
import Footer from '@/components/Footer'

export default {
  components: {
    Header,
    Home,
    Footer
  },
  data () {
    return {
    }
  }
}
</script>
