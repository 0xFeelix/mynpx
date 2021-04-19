<template>
  <v-card max-width="300" class="ma-3">
    <v-card-text>
      <div>{{ cardsSection.date }}</div>
      <p class="display-1 text--primary">{{ cardsSection.title }}</p>
      <div class="text--primary">
        {{ cardsSection.desc }}
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn text>
        <nuxt-link :to="`${cardsSection.id}`" class="nuxtLink"> Learn more</nuxt-link>
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: ["cardsSection"],
};
</script>

<style scoped>
.nuxtLink{
  text-decoration: none;
  color: #6200EA;
}
</style>

<!-- `/cardPages/${cardsSection.id}` -->