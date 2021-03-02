<template>
  <div>
    <v-row justify="center" align="center">
      <v-col cols="12" sm="8" md="6">
        <v-card>
          <v-card-title class="headline">
            <h2>Welcome to the Fiddlehead Plant</h2>
          </v-card-title>
        </v-card>
      </v-col>
    </v-row>
    <Intro />
  </div>
</template>

<script>
import Intro from '~/components/Intro.vue'

export default {
  components: {
    Intro
  },
  head () {
    return {
      title: 'Home'
    }
  }
}
</script>

<style lang="scss">
</style>
