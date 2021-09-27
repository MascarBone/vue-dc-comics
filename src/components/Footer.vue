<template>
    <footer>
        <div class="top-bg">
            <div class="wrapper">
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
        </div>
        
        <div class="bot-bg">
            <div class="wrapper">
                <div class="row">
                    <div class="btn-box">
                        <button>sign-up now!</button>
                    </div>

                    <nav>
                        <a href="">{{followUs.title.toUpperCase()}}</a>
                        <div v-for="(item,index) in followUs.icons" :key="index">
                            <img :src="require('../assets/images/' + item.url)" :alt="item.url">                    
                            

                        </div>
                    </nav>
                </div>
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
            followUs:{
                title: 'follow us',
                icons: [
                    {
                        url: 'footer-facebook.png',
                        alt: 'facebook icon',
                    },
                    {
                        url: 'footer-twitter.png',
                        alt: 'twitter icon',
                    },
                    {
                        url: 'footer-youtube.png',
                        alt: 'youtube icon',
                    },
                    {
                        url: 'footer-pinterest.png',
                        alt: 'pinterest icon',
                    },
                    {
                        url: 'footer-periscope.png',
                        alt: 'periscope icon',
                    },
                ]
            }
        }
    }

}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

    .wrapper {    
        width: 1200px;
        margin: 0 auto;
    } 
    .row {
        display: flex;

        .side {
            width: 50%;
        }
    }

    .top-bg {        
        background-image: url('../assets/images/footer-bg.jpg');
        background-size: cover;
        background-position-x: center;
        overflow: hidden;       
        
        h3 {
            color: white;
            text-transform: uppercase;
            font-size: 1.3rem;
            margin-bottom: 15px;
        }
        ul {
            margin-bottom: 15px;
            line-height: 1.3rem;
        }
        li {
            color: grey;

        }
        .row {
        height: 45vh;
        margin: 0 auto;
        padding: 30px 0;
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
    .footer-logo {
        padding:  0 50px;
        position: relative;
        img {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            
            
        }
    }

    .bot-bg {        
        background-color: black;
        color: white;

        .row {            
            padding: 30px 0;

            .btn-box {
                flex-grow: 1;
            }
            button {
                background-color: transparent;
                padding: 10px 15px;
                text-transform: uppercase;
                color: $colorWhite;
                font-size: 1.2rem;
                border: 2px solid $colorPrimaryBlue;
            }

            nav {
                display: flex;
                align-items: center;

                a {
                    text-decoration: none;
                    color: $colorPrimaryBlue;
                    font-size: 1.4rem;
                    font-weight: 600;
                }

                * {
                    margin-left: 15px;

                }
            }
        }
    }

    
</style>