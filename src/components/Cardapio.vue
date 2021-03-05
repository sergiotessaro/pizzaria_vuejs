<template>
  <div id="cardapio">
    <v-app>
      <v-main>
        <drawer-menu></drawer-menu>
        <cardapio-header></cardapio-header>
        <menu-bar></menu-bar>
      </v-main>
    </v-app>
  </div>
</template>

<script>
import CardapioHeader from "./CardapioHeader.vue";
import DrawerMenu from "./DrawerMenu.vue";
import MenuBar from "./MenuBar.vue";
export default {
  components: { CardapioHeader, MenuBar, DrawerMenu },
};
</script>
,
    DrawerMenu
<style>
</style>