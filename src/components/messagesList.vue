<template>
  <!-- messages list -->
  <div
    class="flex flex-col w-full md:w-64 flex-shrink-0 bg-white overflow-hidden"
  >
    <!-- sort section -->
    <div
      class="
        flex flex-shrink-0
        items-center
        justify-between
        text-xs
        font-semibold
        text-gray-600
        px-4
        py-2
        bg-gray-100
        border border-b
      "
    >
      <button class="flex items-center space-x-2 focus:outline-none">
        <p>Sorted by Date</p>
        <svg
          class="w-4 h-4 text-black ml-auto hidden md:flex"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M19 9l-7 7-7-7"
          ></path>
        </svg>
      </button>
      <button class="focus:outline-none">
        <svg
          class="w-5 h-5"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M3 4h13M3 8h9m-9 4h6m4 0l4-4m0 0l4 4m-4-4v12"
          ></path>
        </svg>
      </button>
    </div>
    <!--  -->
    <!-- list -->
    <div class="flex-1 overflow-auto space-y-0 bg-gray-200">
      <message-tile
        @click="openMessage(message.id)"
        v-for="message in messages"
        :key="message.id"
        :isActive="isActive(message.id)"
        :name="message.name"
        :time="message.time"
        :subject="message.subject"
        :message="message.message"
      ></message-tile>
    </div>
    <!--  -->
  </div>
  <!-- end messages list -->
</template>
<script>
import messageTile from "./messageTile.vue";
export default {
  components: { messageTile },
  data() {
    return {
      activeMessage: null,
      messages: [
        {
          id: 1,
          name: "hawkar hayder othman fattah",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 2,
          name: "hawa",
          time: "2 days ago",
          subject: "Refund on the purchased items last week",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 3,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 4,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 5,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 6,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 7,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 8,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 9,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
        {
          id: 10,
          name: "hawa",
          time: "2 days ago",
          subject: "test",
          message:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. No necessitatibus voluptatibus perspiciatis est ...",
          isActive: false,
        },
      ],
    };
  },
  computed: {},
  methods: {
    isActive(id) {
      // console.log(this.activeMessage);
      if (this.activeMessage)
        return id == this.activeMessage.id
          ? "border-l-4 border-blue-600 pl-3 bg-gray-200 border-t-0"
          : "bg-white";
      return "bg-white";
    },
    openMessage(id) {
      // this.activeMessage
      for (let i = 0; i < this.messages.length; i++) {
        // console.log(this.messages[i]);
        this.messages[i].isActive = false;
        if (this.messages[i].id == id) {
          this.clickedMsg = this.messages[i];
          this.messages[i].isActive = true;
          this.activeMessage = this.messages[i];
        }
      }
      // console.log(this.activeMessage);
      // console.log(this.messages);
    },
  },
};
</script>
