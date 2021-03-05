<template>
  <div id="cardapio_header">
    <img class="icon" src="@/assets/icon.jpeg" />
    <h2>PizzaJá</h2>
    <div class="cartao">
      <status-card></status-card>
    </div>
    <v-row class="content">
      <v-icon dense class="icone-relogio">mdi-clock</v-icon>
      <h3><strong>60 min</strong></h3>
    </v-row>
  </div>
</template>

<script>
import StatusCard from "./StatusCard.vue";
export default {
  components: { StatusCard },
};
</script>

<style>
#cardapio_header {
  top: 0;
  left: 0;
  height: 460px;
  width: 100vw;
  background-image: url("../assets/pizza.png");
  position: absolute;
  justify-content: center;
  overflow-x: hidden;
  display: flex;
}

h2 {
  position: absolute;
  top: 280px;
  justify-content: center;
  letter-spacing: 3px;
  /* left: 684px; */
  color: white;
}

h3 {
  color: rgb(0, 0, 0);
}

.cartao {
  position: absolute;
  top: 340px;
  display: flex;
}
/* h3 {
  margin-left: 4px;
  justify-content: center;
} */

.icon {
  width: 150px;
  height: 150px;
  border: black;
  border-style: double;
  border-radius: 4px;
  position: absolute;
  display: flex;
  justify-content: center;
  top: 100px;
}

.content {
  position: absolute;
  top: 420px;
  justify-content: center;
  /* left: 680px; */
}

.icone-relogio {
  position: absolute;
}
</style>