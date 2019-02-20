<template>
  <div id="app">
    <Block></Block> 
  </div>
</template>

<script>
import Block from "./components/Block/Block.vue"

export default {
  name: "app",
  components:{
    Block
  },
  data() {
    return {};
  }
};
</script>

<style>
#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>
