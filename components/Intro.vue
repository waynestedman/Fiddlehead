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
            <h6>*original artwork by the Queen Fiddlehead</h6>
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
  background-color: #fcf8eb !important;

  .left {
    img {
      max-width: 500px;
    }
    h6 {
      text-align: right;
      padding-right: 4rem;
    }
  }
  .right {
    text-align: center;
    padding-top: 2rem;
    vertical-align: top;

    h3 {
      color: #333;
    }
  }
}
</style>
