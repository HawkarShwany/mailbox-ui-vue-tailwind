<template>
  <div class="bg-white rounded-lg p-6 flex flex-col space-y-4 shadow">
    <!-- name and time and icon -->
    <div class="flex flex-row">
      <div
        class="flex flex-row flex-1 flex-shrink-0 text-lg space-x-2 truncate"
      >
        <h3 class="font-semibold">{{ name }}</h3>
        <span class="text-gray-400">{{ status }}</span>
      </div>
      <div class="flex flex-row flex-shrink-0 space-x-4 items-center">
        <p class="text-gray-400 text-xs">{{ time }}</p>
        <img
          class="w-6 h-6 rounded-full object-cover"
          src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=facearea&w=144&q=80&facepad=3"
          alt=""
        />
      </div>
    </div>
    <!--  -->
    <!-- text -->
    <div class="text-sm text-gray-800">{{ text }}</div>
  </div>
</template>
<script>
export default {
  props: ["name", "status", "time", "text"],
};
</script>
