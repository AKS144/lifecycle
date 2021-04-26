<template>
  <div id="app">
    <!--<Home1 />-->
    <!--For Home3-->
    <div v-if="display">
      <Home3 />
    </div>
    <button v-on:click="toogle">Toggle</button>
  </div>
</template>

<script>
//import Home from './components/Home.vue'
//import Home2 from './components/Home2.vue'
import Home3 from "./components/Home3.vue";

export default {
  name: "App",
  components: {
    Home3,
    //Home,
  },
  //for home3
  data() {
    return { display: true }; //in data function property is defined hide or show
  },
  methods: {
    toogle() {
      this.display = !this.display; //
    },
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
  margin-top: 60px;
}
</style>
*/