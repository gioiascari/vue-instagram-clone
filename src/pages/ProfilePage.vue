<template>
  <v-container class="pa-10">
    <stories-section />
    <feed-section />
  </v-container>
</template>

<script>
import StoriesSection from "../components/StoriesSection.vue";
import FeedSection from "../components/FeedSection.vue";
export default {
  components: {
    StoriesSection,
    FeedSection,
  },
};
</script>

<style></style>
