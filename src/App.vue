<template>
  <div id="app">
    <Topbar/>
    <Container/>
  </div>
</template>

<script>
import Topbar from "./components/Topbar.vue";
import Container from "./components/Container.vue";

export default {
  name: "app",
  components: {
    Topbar,
    Container
  }
};
</script>

<style>
#app {
  background: url(./assets/homepage/mark.png) top left repeat;
}
</style>
