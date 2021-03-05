<template>
  <div id="app">
    <h1>Ian Malcolm</h1>
    <h2>Building things for the web</h2>
    <nav class="page-nav">
      <app-nav-tab>About Me</app-nav-tab>
      <div class="nav-tab">Projects</div>
      <div class="nav-tab">Contact</div>
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
  data() {
    return {
      aboutMeText: "Something about me."
    };
  },
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
