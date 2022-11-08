<template>
  <div class="flex">
    <input
      type="text"
      v-model="searchValue"
      class="justify-end pl-2 mt-1 w-48 h-8 rounded-md border-[#A3B1C2] border border-solid italic text-xs text-[#A2A9B1]"
      placeholder="Nom d'une ressource"
    />

    <img src="../assets/button-3.png" class="h-8 mt-1 -ml-2" />
    <div>
      <!-- <div v-for="card in filteredCards" :key="card.id">
        {{ card.name }}
      </div> -->
    </div>
  </div>
</template>

<script>
import data from "../data/data.json";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "SearchCard",

  data: () => ({
    searchValue: "",
    cards: data,
  }),
  // computed: {
  //   filteredCards() {
  //     return this.cards.filter((card) => {
  //       return card.name.toLowerCase().includes(this.searchValue.toLowerCase());
  //     });
  //   },
  // },
};
</script>
