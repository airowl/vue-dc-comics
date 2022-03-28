<template>
  <div id="app">
    
    <Header />

    <main>
      <div>
      <h2>Content goes here...</h2>
      </div>
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

export default {
  name: 'App',
  components: {
    Header,
    FooterTop,
    FooterBottom
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
    height: 10vh;
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
