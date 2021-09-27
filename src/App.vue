<template>
  <div id="app">
    <h1>TESTO DI PROVA</h1>
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">
@import url('./style/generic.scss');
@import url('./style/variables.scss');

h1 {
  background-color: tomato;
  // color: $colorWhite;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}
</style>
