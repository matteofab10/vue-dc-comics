<template>
  <div>
    <Header />
    <Main />
    <MainContent />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import MainContent from "./components/MainContent.vue";
import Footer from "./components/Footer.vue";


export default {
  name: 'App',
  components: {
    Header,
    Main,
    MainContent,
    Footer
  }
}
</script>

<style lang="scss">
@import "./assets/style/vars.scss";
@import "./assets/style/general.scss";
@import "./assets/style/utilities.scss";
@import url('https://fonts.googleapis.com/css2?family=Teko&display=swap');
</style>
