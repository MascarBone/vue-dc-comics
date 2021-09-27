<template>
  <main>
      
        <div class="jumbotron">
            <img src="../assets/images/jumbotron.jpg" alt="">
        </div>
        
        <div class="background">
            <div class="wrapper">
                <div class="top">
                    <span>CURRENT SERIES</span>
                </div>

                <div class="row">
                    <div class="album" v-for="(element, index) in Albums" :key="index">
                        <Card :thumb="element.thumb" :price="element.price" :series="element.series" :type="element.type" />
                    </div>
                </div>

                <div class="bot">
                    <button>LOAD MORE</button>
                </div>
            </div>
        </div>
      
  </main>
</template>

<script>
import Card from './Card.vue'

import Albums from '../data/dc-comics.json'

export default {
    components: {
        Card,
    },

    data: function () {
        return {
            Albums,
        }
    }
}
</script>

<style scoped lang="scss">
    @import '../style/variables.scss';

    .jumbotron {
        height: 40vh;
        overflow: hidden;

        img {
            object-fit: cover;
            object-position: center;
            width: 100%;
        }
    }
    .background {
        background-color: $colorBlackCoal;
    }
    .wrapper {        
        // display: flex;        
        width: 1200px;
        margin: 0 auto;
    }

    .top {
        position: relative;
        padding-bottom: 50px;

        span {
            padding: 5px 20px;
            font-size: 1.5rem;
            font-weight: 600;
            background-color: $colorPrimaryBlue;
            color: $colorWhite;
            position: absolute;
            transform: translateY(-50%);
        }
    }

    .bot {
        text-align: center;
        padding-bottom: 50px;
        button {
            padding: 10px 30px;
            font-size: 1.1rem;
            font-weight: 600;
            background-color: $colorPrimaryBlue;
            color: $colorWhite;
            border: none;
        }
    }

    .row {             
        display: flex;
        flex-wrap: wrap;
        

        h2 {
            color: $colorWhite;
        }
    }

    .album {
        width: calc(100% / 6);
    }
</style>