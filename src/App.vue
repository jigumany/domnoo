<template>
  <div>
    <compHeader />
    <div>
      <compIndex />
      <compMenu />
      <compCallUs />
      <compNewsLetter />
    </div>
    <compFooter />
  </div>
</template>

<script>
import compHeader from "./components/Header-footer/Header.vue";
import compFooter from "./components/Header-footer/Footer.vue";
import compIndex from "./components/Featured/index.vue";
import compMenu from "./components/Menu/index.vue";
import compCallUs from "./components/CallUs/index.vue";
import compNewsLetter from "./components/NewsLetter/index.vue";

export default {
  components: {
    compHeader,
    compFooter,
    compIndex,
    compMenu,
    compCallUs,
    compNewsLetter
  }
};
</script>

<style>
@import "./assets/style.css";
</style>
