<template>
  <div id="app">
    <Header/>
    <Products/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Products from './components/Products.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Products,
    Footer
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');

  body{
    font-family: 'Oswald', sans-serif;
  }

</style>
