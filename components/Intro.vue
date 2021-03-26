<template>
  <v-card
    elevation="2"
    outlined
    class="intro-card"
  >
    <v-container>
      <v-row>
        <v-col>
          <div class="left">
            <img src="fiddlehead-artwork.png">
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
.intro-card {
  margin-top: 2rem;
  margin-bottom: 2rem;

  .left {
    img {
      max-width: 500px;
    }
  }
  .right {
    text-align: center;
    padding-top: 2rem;
    vertical-align: top;
  }
}
</style>
