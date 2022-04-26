<template>
  <div class="row">
    <div class="col-8">
      <instagram-card v-for="card in cards" :key="card" :info="card" />
    </div>
    <div class="col-4"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import InstagramCard from "@/components/InstagramCard.vue";

let cards = [];

cards = [
  "https://picsum.photos/id/1/400/400",
  "https://picsum.photos/id/2/400/400",
  "https://picsum.photos/id/3/400/400",
  "https://picsum.photos/id/4/400/400",
];

export default {
  name: "HomeView",
  data: function () {
    return {
      cards: cards,
    };
  },
  components: {
    InstagramCard,
  },
};
</script>
