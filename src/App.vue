<!-- eslint-disable prettier/prettier -->
<!-- eslint-disable vue/valid-template-root -->
<template>
  <div id="App">
    <Layout />

    <section
      class="flex justify-center xl:justify-start flex-wrap-reverse gap-6 bg-[#ECF2F6]"
    >
      <Cards :key="cards.id" :cards="cards" />
    </section>
  </div>
</template>

<script>
import Layout from "./components/Layout.vue";
import Cards from "./components/Cards.vue";

import data from "./data/data.json";

export default {
  name: "App",

  components: {
    Layout,
    Cards,
  },

  data() {
    return {
      cards: data,
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500&display=swap");
</style>
