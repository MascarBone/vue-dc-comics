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
                        <a href="">{{item.link}}</a>
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
                },
                {
                   link: 'comics',
                   url: '#',
                },
                {
                   link: 'movies',
                   url: '#',
                },
                {
                   link: 'tv',
                   url: '#',
                },
                {
                   link: 'games',
                   url: '#',
                },
                {
                   link: 'collectibles',
                   url: '#',
                },
                {
                   link: 'videos',
                   url: '#',
                },
                {
                   link: 'fans',
                   url: '#',
                },
                {
                   link: 'news',
                   url: '#',
                },
                {
                   link: 'shop',
                   url: '#',
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
                color: $colorBlack;
            }
            
        }
    }

</style>>