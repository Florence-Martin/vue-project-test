<template v-if="card">
  <div id="Card" class="w-72 h-96 m-6 bg-white rounded-lg border border-solid">
    <div>
      <div
        id="_card-header"
        class="flex flex-row w-auto h-12 items-center p-4 gap-4"
      >
        <input type="checkbox" />
        <img src="../assets/public.png" />
        <h2 class="">{{ card.userName }}</h2>
      </div>

      <div
        id="_card-media"
        class="bg-[#F5F8FA] flex w-auto h-32 justify-center items-center"
      >
        <div v-if="card.map">
          <img src="../assets/picture.png" alt="picture" />
        </div>
        <div v-else>
          <img src="../assets/map.png" alt="map" class="w-16 h-16" />
        </div>
      </div>

      <div id="_card-content" class="px-4">
        <h2 class="py-4 text-sm font-medium leading-5">
          {{ card.name }}
        </h2>
        <p class="pb-4 text-xs font-normal leading-4 text-[#627184]">
          {{ card.description }}
        </p>
      </div>
      <div class="px-4 flex justify-between">
        <div>
          <h3 class="text-xs font-medium leading-4 text-[#12171B]">
            Modifié le
          </h3>
          <div class="text-[#627184] text-xs font-normal">
            {{ card.modificationDate }}
          </div>
        </div>
        <div class="flex flex-col items-end">
          <h3 class="text-xs font-medium leading-4 text-[#12171B]">
            Application
          </h3>
          <div class="text-[#627184] text-xs font-normal">
            {{ card.application }}
          </div>
        </div>
      </div>
      <div id="actions" class="flex gap-6 p-4 justify-around">
        <img src="../assets/remove_red_eye.png" alt="remove-eye" />
        <img src="../assets/brush.png" alt="brush" />
        <img src="../assets/file_copy.png" alt="file-copy" />
        <img src="../assets/delete.png" alt="delete" />
        <img src="../assets/more_horiz.png" alt="more-horiz" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Card",
  props: {
    card: Object,
  },
};
</script>
