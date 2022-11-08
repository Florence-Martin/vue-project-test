<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="Cards" :key="card.id" v-for="card in cards">
    <Card :card="card" />
  </div>
</template>

<script>
import Card from "./Card";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Cards",
  props: {
    cards: Array,
  },
  components: {
    Card,
  },
};
</script>
