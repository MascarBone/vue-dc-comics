<template>
  <main>
      <div class="wrapper">
            <div class="row">
                <h2>--  Content goes here  --</h2>
                
            </div>
            <Card :source="Cards.thumb"/>
      </div>
      
  </main>
</template>

<script>
import Card from './Card.vue'

import Cards from '../data/dc-comics.json'

export default {

    components: {
        Card,
    },
    data: function () {
        return {
            Cards,
        }
    }
}
</script>

<style scoped lang="scss">
    @import url('../style/generic.scss');
    @import url('../style/variables.scss');

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