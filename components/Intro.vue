<template>
  <v-card
    elevation="2"
    outlined
  >
    <v-container>
      <v-row>
        <v-col>
          <div class="left">
            <img src="https://via.placeholder.com/500x500">
          </div>
          <div class="right">
            <h3>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nesciunt repellat aspernatur odit incidunt blanditiis quae, nobis, a dolores, ducimus amet enim voluptatem id repudiandae itaque illum cupiditate. Debitis, hic consequuntur!</h3>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
export default {
  name: 'Intro'
}
</script>

<style lang="scss" scoped>
  .right {
    vertical-align: top;
  }
</style>
