<template>
  <v-container
    class="flex"
    flat
    tile
  >
    <v-row>
      <v-col cols="12" class="py-2 black--text text-center">
        @{{ new Date().getFullYear() }} — <strong> The Fiddlehead Plant</strong>

        <v-spacer></v-spacer>

        <p>Made with Love</p>
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
        'mdi-instagram',
      ],
    }),
  }
</script>