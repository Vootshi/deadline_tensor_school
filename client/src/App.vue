<template>
  <div id="app">
    <main-container></main-container>
  </div>
</template>

<script>
import MainContainer from "./components/Main/Main";
import axios from "axios";
import store from "./store";

export default {
  components: {MainContainer},
  name: "App",
  mounted() {
    // axios.defaults.headers.common['Authorization'] = this.$store.getters.getToken
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
  font-weight: 1000;
}

/*#app {*/
/*  font-family: Avenir, Helvetica, Arial, sans-serif;*/
/*  -webkit-font-smoothing: antialiased;*/
/*  -moz-osx-font-smoothing: grayscale;*/
/*  text-align: center;*/
/*  color: #2c3e50;*/
/*}*/
</style>