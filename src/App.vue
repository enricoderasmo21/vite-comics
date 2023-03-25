<script>
import AppNav from "./components/AppNav.vue";
import AppMain from "./components/AppMain.vue";
import AppMainSecondSec from "./components/AppMainSecondSec.vue";
import AppFooterFirstSec from "./components/AppFooterFirstSec.vue";
import AppFooterSecondSec from "./components/AppFooterSecondSec.vue";

export default{
  data() {
    return {

    }
  },

  components: {
    AppNav,
    AppMain,
    AppMainSecondSec,
    AppFooterFirstSec,
    AppFooterSecondSec

}
}
</script>

<template>

  <AppNav></AppNav>
  
<main>
  <AppMain></AppMain>
  <AppMainSecondSec></AppMainSecondSec>
</main>

<footer>
  <AppFooterFirstSec></AppFooterFirstSec>
  <AppFooterSecondSec></AppFooterSecondSec>
</footer>

</template>

<style scoped>

</style>
