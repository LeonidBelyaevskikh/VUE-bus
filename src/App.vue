<template>
  <div id="app">
    <Component1 class="component"/>
    <Component2 class="component"/>
    <Component3 class="component"/>
  </div>
</template>

<script>
import Component1 from "./components/Component1";
import Component2 from "./components/Component2";
import Component3 from "./components/Component3";

export default {
  name: 'App',
  components: {
    Component3,
    Component2,
    Component1
  }
}
</script>

<style>
  #app {
    width: 100%;
    display: flex;
    justify-content: space-around;
  }
  .component {
    width: 30%;
    height: 150px;
    background-color: gold;
    font-size: 50px;
    color: black;
    text-align: center;
    line-height: 150px;
  }
</style>
