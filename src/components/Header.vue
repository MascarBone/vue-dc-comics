<template>
  <header>
      <div class="wrapper">
        <div class="row">
            <div class="header-logo">
                <img src="../assets/images/dc-logo.png" alt="dc-logo">
            </div>
            <nav class="header-nav">
                <ul>
                    <li v-for="(item, index) in navList" :key="index" >                        
                        <a href="">{{item.link}}<span v-if="item.selected"></span></a>
                        
                    </li>
                </ul>
            </nav>
        </div>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data: function() {
        return {
            navList:[
                {
                   link: 'characters',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'comics',
                   url: '#',
                   selected: true,
                },
                {
                   link: 'movies',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'tv',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'games',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'collectibles',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'videos',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'fans',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'news',
                   url: '#',
                   selected: false,
                },
                {
                   link: 'shop',
                   url: '#',
                   selected: false,
                },                
            ]
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
        height: 15vh;
        display: flex;
        align-items: center;
        
    }

    .header-logo {
        flex-grow: 1;
    }

    .header-nav {

        
        ul {
            display: flex;

            a {
                text-decoration: none;
                margin: 0 10px;
                text-transform: uppercase;
                font-size: 1.1rem;
                font-weight: 500;
                color: $colorBlack;

                position: relative;
            }

            a > span {
                height: 7px;
                width: 100%;
                left: 0;
                bottom: -300%;
                background-color: $colorPrimaryBlue;
                position: absolute;
            }
            
            :hover a {
                color: $colorPrimaryBlue;
            }
        }
    }

</style>>