<template>
  <v-container
    class="flex"
    tile
  >
    <v-row>
      <v-col
        cols="12"
        class="py-2 black--text text-center"
        elevation="4"
      >
        <p>@{{ new Date().getFullYear() }} — <strong> The Fiddlehead Plant</strong></p>

        <v-spacer />

        <p>Made with <v-icon>mdi-heart</v-icon> in the Bay Area</p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Footer',

  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram'
    ]
  })
}
</script>
