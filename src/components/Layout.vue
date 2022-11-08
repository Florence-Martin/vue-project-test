<template>
  <div id="Layout">
    <Header />
    <TopContent />
  </div>
</template>

<script>
import Header from "./Header.vue";
import TopContent from "./TopContent.vue";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Layout",
  components: {
    Header,
    TopContent,
  },
};
</script>
