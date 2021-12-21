<template>
  <div id="app">
      <Header />

      <Banner />

      <Main />


      <PreFooter />

      <Footer />

      <PostFooter />
  </div>
</template>


<script>
import Header from "./components/Header.vue";
import Banner from "./components/Banner.vue";
import Main from "./components/Main.vue";
import PreFooter from "./components/PreFooter.vue";
import Footer from "./components/Footer.vue";
import PostFooter from "./components/PostFooter.vue";


export default {
  name: "App",
  components: {
    Header,
    Banner,
    Main,
    PreFooter,
    Footer,
    PostFooter
  },
};
</script>


<style lang="scss">
// @import '../style/variables';
// @import '../style/mixins';
@import './style/general';
@import './style/common';

</style>
