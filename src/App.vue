<template>
  <Header />
  <div class="mt-5">
    <router-view :lists="lists"></router-view>
  </div>
</template>

<script>
import data from "./data/data";
import Header from "./components/Header.vue";

export default {
  name: "App",
  data() {
    return { lists: data };
  },
  components: { Header },
};
</script>

<style></style>
