<template>
  <div id="app">
    <Nav />
    <About />
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import About from './components/About.vue'

export default {
  name: 'app',
  components: {
    Nav, About
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
  min-height: 100vh;
  color: #222;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
