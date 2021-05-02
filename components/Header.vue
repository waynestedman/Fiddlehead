<template>
  <v-app-bar app>
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
      color="#333"
    >
      <v-icon>mdi-mailbox-open</v-icon>
      <span class="ml-2">Contact Us</span>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {}
</script>
