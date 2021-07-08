<template>
  <div id="app">
    <NavBar />
  </div>
</template>

<script>
import NavBar from "@/views/NavBar.vue";
export default {
  name: "App",
  components: {
    NavBar,
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Roboto", sans-serif;
  font-size: 16px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $main-color;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: $main-color;

    &.router-link-exact-active {
      color: $main-color;
    }
  }
}
</style>
