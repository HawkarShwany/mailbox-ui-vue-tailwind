<template>
  <div class="flex flex-col flex-1 overflow-hidden">
    <message-action></message-action>
    <message-subject></message-subject>
    <div class="py-4 px-2 space-y-4 overflow-auto">
      <message-card
        v-for="message in messages"
        :key="message.text"
        :name="message.name"
        :status="message.status"
        :text="message.text"
        :time="message.time"
      ></message-card>
    </div>
  </div>
</template>
<script>
import messageAction from "./messageActions.vue";
import messageSubject from "./messageSubject.vue";
import messageCard from "./messageCard.vue";
export default {
  components: {
    messageAction,
    messageSubject,
    messageCard,
  },
  data() {
    return {
      messages: [
        {
          name: "Joe Armstrong",
          status: "wrote",
          time: "Yesterday at 7:24 AM",
          text: "Thanks so much!! Can't wait to try it out :)",
        },
        {
          name: "Joe Armstrong",
          status: "wrote",
          time: "Yesterday at 7:24 AM",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur exercitationem corporis assumenda nam laboriosam reprehenderit quidem veniam quod cupiditate, nihil esse dolore tempore nulla harum? Tenetur consequuntur aut consectetur quos quae est exercitationem nobis qui cupiditate magni, molestias nostrum sint ad, quisquam facere iusto necessitatibus eos porro possimus quaerat delectus! Similique illo dolorum ea numquam cumque,",
        },
        {
          name: "Joe Armstrong",
          status: "wrote",
          time: "Yesterday at 7:24 AM",
          text: "blanditiis, dolorem iusto eius ducimus quo, maiores pariatur nobis officia dicta! Rerum ut labore esse dolorem dolor eius debitis perferendis sapiente, blanditiis, libero voluptatum sunt rem, minima provident officiis? Illum suscipit fugit",
        },
        {
          name: "Joe Armstrong",
          status: "wrote",
          time: "Yesterday at 7:24 AM",
          text: "accusantium, iure voluptate minima sunt, quod nesciunt magnam ab doloremque ipsa quas?\rLorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis laboriosam consectetur ipsa amet quia aperiam saepe inventore, est quo alias magni provident exercitationem, totam aut expedita,",
        },
      ],
    };
  },
};
</script>
