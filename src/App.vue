<template>
  <div id="app">
    <div class="container">
      <div class="container__header">
        <HeaderComponent />
      </div>
      <div class="container__main"></div>
      <div class="container__"></div>
    </div>
  </div>
</template>

<script>
import HeaderComponent from "./components/default/header-component.vue";
export default {
  components: { HeaderComponent },
  name: "App",
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>
