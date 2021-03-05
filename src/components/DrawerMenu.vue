<template>
  <v-app>
    <v-app-bar app clipped-left fixed color="#E0E0E0" dense>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>PizzaJá</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer
      app
      clipped
      left
      v-model="drawer"
      fixed
    >
      <v-list nav dense>
        <v-list-item-group
          active-class="dark-grey--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title>Telefone de Contato</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Endereço</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Sobre</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-app>
</template>
<script>
export default {
  data: () => ({
    drawer: false,
  }),
};
</script>

<style>
</style>