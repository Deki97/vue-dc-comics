<template>
  <div id="app">
      <Header />

      <Main />

      <PreFooter />
      <Footer />
  </div>
</template>


<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import PreFooter from "./components/PreFooter.vue";


export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
    PreFooter
  },
};
</script>


<style lang="scss">
// @import '../style/variables';
// @import '../style/mixins';
// @import '../style/general';
@import '../style/common';

</style>
