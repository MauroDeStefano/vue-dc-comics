<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Main />
    <Merchandising />
    <Footer />
  </div>
</template>

<script>

  import Header from './components/Header.vue';
  import Jumbotron from './components/Jumbotron';
  import Main from './components/Main.vue';
  import Merchandising from './components/Merchandising.vue';
  import Footer from './components/Footer.vue';

  export default {
    name: 'App',
    components: {
      Header,
      Jumbotron,
      Main,
      Merchandising,
      Footer
    }
  };

</script>

<style >

@import "./assets/style/utilities.scss";

</style>

