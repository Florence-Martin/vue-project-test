<template>
  <div
    id="TopContent"
    class="flex flex-row mt-4 w-60 h-20 pt-2 px-4 pb-4 divide-x divide-[#A3B1C2]"
  >
    <div class="text-[#12171B] px-4 flex flex-col">
      <label class="text-xs font-normal mb-1">Créer</label>
      <Button />
    </div>
    <div class="flex flex-col px-4">
      <label class="text-[#12171B] font-normal text-xs">Rechercher</label>

      <SearchCard />
    </div>
  </div>
  <div
    class="bg-white flex flex-row items-center h-10 border-lightGray border border-solid"
  ></div>
</template>

<script>
import Button from "./Button.vue";
import SearchCard from "./SearchCard.vue";

export default {
  name: "TopContent",
  components: {
    Button,
    SearchCard,
  },
};
</script>
