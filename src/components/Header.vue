<template>
  <header>
    <div class="bg-[#ECF2F6] flex flex-row justify-between items-center h-10">
      <img src="../assets/tab-group.png" />
      <div
        id="header_menu"
        class="flex gap-6 justify-around items-center text-[#627184] divide-x divide-[#A3B1C2]"
      >
        <img src="../assets/star.png" class="pl-3" />
        <img src="../assets/settings.png" class="pl-3" />
        <img src="../assets/support.png" class="pl-3" />
        <img src="../assets/mail.png" class="pl-3" />
        <img src="../assets/notification.png" class="pl-3" />
        <img src="../assets/avatar.png" />
      </div>
    </div>
  </header>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Header",
  props: ["title"],

  data() {
    return {};
  },

  methods: {},

  computed: {},
};
</script>

<style></style>
