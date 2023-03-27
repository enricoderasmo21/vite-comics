<script>
import AppNav from "./components/AppNav.vue";
import AppMain from "./components/AppMain.vue";
import AppBuy from "./components/AppBuy.vue";
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
    AppBuy,
    AppFooterFirstSec,
    AppFooterSecondSec

}
}
</script>

<template>

  <AppNav></AppNav>

<main>
  <AppMain></AppMain>
  <AppBuy></AppBuy>
</main>

<footer>
  <AppFooterFirstSec></AppFooterFirstSec>
  <AppFooterSecondSec></AppFooterSecondSec>
</footer>

</template>

<style scoped>

</style>
