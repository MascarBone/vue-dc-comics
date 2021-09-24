<template>
  <footer>
      <div class="top-wrapper">
        <div class="row">

         </div>
      </div>
      <div class="bot-wrapper">
        <div class="row">

         </div>
      </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
    // footer {
    //      ../assets/images/dc-logo-bg.jpg
    // }

    .top-wrapper {        
        background-image: url('../assets/images/footer-bg.jpg');
        background-size: cover;
        background-position-x: center;
    
        .row {
        width: 1200px;
        height: 45vh;
    }
    }
    .bot-wrapper {        
        background-color: black;

        .row {            
            width: 1200px;
            height: 10vh;
        }
    }
    
</style>