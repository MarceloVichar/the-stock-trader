<template>
    <v-layout row wrap>
        <Stock v-for="stock in stocks" :key="stock.id" :stock="stock" />
    </v-layout>
</template>
<script>
import Stock from "./Stock.vue";

export default {
  components: { Stock },
  data() {
    return {
      stocks: [
        { id: 1, name: "BMW", price: "110" },
        { id: 2, name: "WM", price: "120" },
        { id: 3, name: "APPLE", price: "200" },
        { id: 4, name: "OUTRA", price: "50" },
      ],
    };
  },
};
</script>
<style>
</style>
