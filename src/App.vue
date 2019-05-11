<template>
  <div id="app">
    <h1>H1 Title</h1>
    <nav class="page-nav">
      <app-nav-tab>Tab 1</app-nav-tab>
      <div class="nav-tab">Tab 2</div>
      <div class="nav-tab">Tab 3</div>
    </nav>
    <app-information>
      <p>This is content passed into the slot</p>
    </app-information>
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  </div>
</template>

<script>
import Information from "./components/Information.vue";
import NavTab from "./components/NavTab.vue";

export default {
  name: "app",
  components: {
    appInformation: Information,
    appNavTab: NavTab
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.page-nav {
  display: flex;
  justify-content: left;
}
</style>
