<template>
  <header>
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
    
    .row {
        width: 1200px;
        height: 15vh;
        display: flex;
        align-items: center;
        margin: 0 auto;
        
    }

    .header-logo {
        flex-grow: 1;
    }

    .header-nav {

        
        ul {
            list-style: none;
            display: flex;


            a {
                text-decoration: none;
                margin: 0 10px;
            }
        }
    }

</style>>