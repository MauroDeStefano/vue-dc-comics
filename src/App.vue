<template>
  <div id="app">
    <Header />
    <Main />
    <Merchandising />
    <Footer />
  </div>
</template>

<script>

  import Header from './components/Header.vue';
  import Main from './components/Main.vue';
  import Merchandising from './components/Merchandising.vue';
  import Footer from './components/Footer.vue';

  export default {
    name: 'App',
    components: {
      Header,
      Main,
      Merchandising,
      Footer
    }
  };

</script>

<style >

@import "./assets/style/utilities.scss";

</style>

