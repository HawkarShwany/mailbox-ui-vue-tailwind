<template>
  <a class="block px-4 py-3 space-y-1 hover:bg-gray-200" :class="isActive">
    <div class="flex flex-row justify-between">
      <p class="text-sm font-semibold text-gray-900 truncate">{{ name }}</p>
      <p class="text-xs text-gray-600 flex-shrink-0">{{ time }}</p>
    </div>
    <div class="text-xs font-normal text-gray-700 truncate">{{ subject }}</div>
    <div class="text-xs text-gray-500 truncate">
      {{ message }}
    </div>
  </a>
  <!--  -->
</template>

<script>
export default {
  //   props: ["name", "time", "subject", "message"],
  props: {
    name: {
      type: String,
      required: true,
    },
    time: {
      type: String,
      required: true,
    },
    subject: {
      type: String,
      required: true,
    },
    message: {
      type: String,
      required: true,
    },
    isActive: {
      type: String,
    },
  },
  data() {
    return {
      // active: this.isActive,
    };
  },
};
</script>
