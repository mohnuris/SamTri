<template>
  <div id="app">
    <!-- <router-link to="/">Home</router-link>|
    <router-link to="/users">Users</router-link>|
    <router-link to="/about">About</router-link>-->
    <router-view />
    <layout />
  </div>
</template>

<script>
import Layout from "../../../api/src/components/Layout.vue";
// import Layout from "./components/Layout.vue";

export default {
  name: "app",
  components: {
    Layout,
    // Layout,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
