<template>
  <div id="app">
    <NavBar />
    <Main />
  </div>
</template>

<script>
import NavBar from "@/views/NavBar.vue";
import Main from "@/components/Main.vue";

export default {
  name: "App",
  components: {
    NavBar,
    Main,
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
