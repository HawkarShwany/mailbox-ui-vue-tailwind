<template>
  <div class="flex flex-col h-screen">
    <the-header></the-header>
    <div class="flex flex-1 bg-gray-200 overflow-hidden">
      <side></side>
      <msg-list></msg-list>
      <message-section></message-section>
    </div>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import side from "./components/sidebar.vue";
import msgList from "./components/messagesList.vue";
import messageSection from "./components/messageSection.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    side,
    msgList,
    messageSection,
  },
};
</script>

<style></style>
