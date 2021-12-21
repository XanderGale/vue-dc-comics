<template>
  <div id="app">
    <Header/>
    <Main/>
    <Navmain/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Navmain from './components/Navmain.vue';
import Footer from './components/Footer.vue'

export default {
  name: "App",
  components: {
    Header,
    Main,
    Navmain,
    Footer,
  },
};
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';

</style>
