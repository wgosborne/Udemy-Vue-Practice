<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Wagner Osborne"/>
  <IFELSE />
  <br />
  <br />
  <br />
  <br />
  <PAGES />
  <PAGEONE />
  <INPUTS />
  <FORLOOPS />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import PAGES from './components/NewComponent';
import PAGEONE from './components/pages';
import INPUTS from './components/InputBoxes';
import IFELSE from "./components/IfElsePractice";
import FORLOOPS from "./components/ForLoopPractice";

export default {
  name: 'App',
  components: {
    HelloWorld,
    PAGES,
    PAGEONE,
    INPUTS,
    IFELSE,
    FORLOOPS,
  }
}
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
