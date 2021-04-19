<template>
  <v-row>
    <CardDisplay v-for="card in allCards" :key="card.id" :cardsSection="card" />
  </v-row>
</template>

<script>
import { cardDisplay } from "@/assets/data.js";
export default {
  data() {
    return {
      allCards: cardDisplay,
    };
  },
};
</script>

<style>
</style>
