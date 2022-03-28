<template>
  <div id="app">
    
    <Header />

    <main>
      <div>
      <h2>Content goes here...</h2>
      </div>
      <MainBottom />
    </main>

    <footer>
      <FooterTop />
      <FooterBottom />
    </footer>
    
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'
import MainBottom from './components/MainBottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    FooterTop,
    FooterBottom,
    MainBottom
  }
}
</script>

<style lang="scss">
@import "assets/scss/style.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  main{
    background-color: black;
    color: white;

    div{
      @include container;
      padding: 1.5rem 0;
    }
  }

  footer{
    height: 40vh;
    color: white;
  }
}
</style>
