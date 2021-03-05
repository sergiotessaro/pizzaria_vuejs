<template>
  <div id="app">
    <cardapio></cardapio>
  </div>
</template>

<script>
import Cardapio from "./components/Cardapio.vue";

export default {
  components: { Cardapio },
};
</script>

<style>
#app {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  text-align: center;
  color: #2c3e50;
}
</style>
