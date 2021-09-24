<template>
  <footer>
      <div class="top-wrapper">
        <div class="row">
            <div class="side footer-list">
                <div v-for="(item,index) in listFooter" :key="index" class="">
                    <h3>{{item.title}}</h3>
                    <ul>
                        <li v-for="(el,yndex) in item.list" :key="yndex">{{el.link}}</li>
                    </ul>
                </div>
                
            </div>
            <div class="side footer-logo">
                <img src="../assets/images/dc-logo-bg.png" alt="dc-logo-bg">
            </div>
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
    data: function() {
        return {
            listFooter: [
            {
                title: 'dc comics',
                list:[
                    {
                        link: 'Characters',
                        url: '#',                        
                    },
                    {
                        link: 'Comics',
                        url: '#',                        
                    },
                    {
                        link: 'Movies',
                        url: '#',                        
                    },
                    {
                        link: 'TV',
                        url: '#',                        
                    },
                    {
                        link: 'Games',
                        url: '#',                        
                    },
                    {
                        link: 'Videos',
                        url: '#',                        
                    },
                    {
                        link: 'News',
                        url: '#',                        
                    },
                ],
            },
            {
                title: 'shop',
                list:[
                    {
                        link: 'Shop DC',
                        url: '#',                        
                    },
                    {
                        link: 'Shop DC Collectibles',
                        url: '#',                        
                    }
                ],
            },
            {
                title: 'dc',
                list:[
                    {
                        link: 'Terms Of Use',
                        url: '#',                        
                    },
                    {
                        link: 'Privacy policy (New)',
                        url: '#',                        
                    },
                    {
                        link: 'Ad Choiches',
                        url: '#',                        
                    },
                    {
                        link: 'Advertising',
                        url: '#',                        
                    },
                    {
                        link: 'Jobs',
                        url: '#',                        
                    },
                    {
                        link: 'Subscriptions',
                        url: '#',                        
                    },
                    {
                        link: 'Talent Workshop',
                        url: '#',                        
                    },
                    {
                        link: 'CPSC Certifactes',
                        url: '#',                        
                    },
                    {
                        link: 'Ratings',
                        url: '#',                        
                    },
                    {
                        link: 'Shop Help',
                        url: '#',                        
                    },
                    {
                        link: 'Contact Us',
                        url: '#',                        
                    },
                ],
            },
            {
                title: 'sites',
                list:[
                    {
                        link: 'DC',
                        url: '#',                        
                    },
                    {
                        link: 'MAD Magazine',
                        url: '#',                        
                    },
                    {
                        link: 'DC Kids',
                        url: '#',                        
                    },
                    {
                        link: 'DC Universe',
                        url: '#',                        
                    },
                    {
                        link: 'DC Power Visa',
                        url: '#',                        
                    }
                ],
            },
            ],          

        }
    }

}
</script>

<style scoped lang="scss">
    // footer {
    //      
    // }

    .top-wrapper {        
        background-image: url('../assets/images/footer-bg.jpg');
        background-size: cover;
        background-position-x: center;

        
        h3 {
            color: white;
        }
        li {
            color: grey;
        }
        .row {
        width: 1200px;
        height: 45vh;
        margin: 0 auto;
    }
    }
    .bot-wrapper {        
        background-color: black;

        .row {            
            width: 1200px;
            height: 10vh;
        }
    }

    .footer-list {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;

        div {
            width: calc(100% / 4);
        }
    }
    
    .row {
        display: flex;

        
        .side {
            width: 50%;
    }
    }

    // .footer-logo {
        // display: flex;
        // justify-content: center;

        // img {
            // vertical-align: middle;
        // }
    // }
    
</style>