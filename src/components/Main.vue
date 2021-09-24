<template>
  <main>
      <div class="wrapper">
            <div class="row">
                <h2>--  Content goes here  --</h2>
            </div>
      </div>
      
  </main>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
    @import url('../scss/generic.scss');

    .wrapper {        
        // display: flex;
        background-color: rgba(27, 30, 44, 0.918);
    }

    .row {    
        width: 1200px;
        height: 30vh;        
        margin: 0 auto;            
        display: flex;
        align-items: center;
        

        h2 {
            // color: $colorWhite;
            color: white;
        }
    }
</style>