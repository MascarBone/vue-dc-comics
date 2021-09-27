<template>
  <div class="card">
      <div class="card-image">
          <img :src="thumb" alt="">
      </div>

      <p>{{series}}</p>
  </div>
</template>

<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    .card {
        padding: 20px;

        
        p {
            margin-bottom: 30px;
            color: $colorWhite;
            text-transform: uppercase;
        }
    }
    .card-image {
        height: 180px;
        background-color: teal;
        overflow: hidden;
        margin-bottom: 15px;

        img {
            width: 100%;
        }

    }

</style>