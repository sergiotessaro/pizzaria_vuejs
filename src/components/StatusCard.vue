<template>
  <v-container class="status-card">
    <v-card outlined max-width="200px" max-height="47px">
      <p class="fechado" :class="{aberto: !fechado}">
        {{ text }}
      </p>
    </v-card>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      text: "",
      hora: {
        type: Number,
      },
      fechado: {
        type: Boolean,
        required: true,
        value: false
      },
    };
  },
  methods: {
    dateTimeSearch() {
      this.hora = new Date().getHours();

      if (this.hora >= 19 && this.hora <= 23) {
        this.text = "Aberto para pedidos";
        this.fechado = false;
      } else {
        this.text = "Fechado para pedidos";
        this.fechado = true;
      }

      console.log(this.fechado);
    },
  },
  beforeMount() {
    this.dateTimeSearch();
  },
};
</script>

<style>

.fechado {
  color: red;
  padding: 10px;
}

.aberto {
  padding: 10px;
  color: green;
} 
</style>