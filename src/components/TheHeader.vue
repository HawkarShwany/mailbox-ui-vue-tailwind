<template>
  <header class="flex text-white">
    <!-- name and icon -->
    <name></name>
    <!-- main side  -->
    <div
      class="
        flex flex-row flex-shrink-0 flex-1
        bg-gray-700
        items-center
        px-4
        ml-auto
      "
    >
      <links></links>

      <!-- search and icons -->
      <search></search>
    </div>
  </header>
</template>

<script>
import name from "./nameandicon.vue";
import links from "./nav.vue";
import search from "./searchandicons.vue";

export default {
  components: {
    name,
    links,
    search,
  },
};
</script>
