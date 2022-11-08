<template>
  <button
    id="Button"
    @click="
      onClick();
      addCard();
    "
    class="flex flex-col"
  >
    <img src="../assets/button-2.png" />
  </button>
  <!-- <p class="pl-8">nombre :{{ counter }}</p> -->
</template>

<script>
import data from "../data/data.json";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Button",

  data() {
    return {
      newCard: "",
      cards: data,
    };
  },

  methods: {
    onClick() {
      this.newCard = this.cards[Math.floor(Math.random() * this.cards.length)];
    },
    addCard() {
      this.cards.push(this.newCard);
    },
  },

  // computed: {
  //   counter() {
  //     return this.cards.length;
  //   },
  // },
};
</script>
