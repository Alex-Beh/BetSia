<script>
import GameCard from "../components/GameCard.vue";

export default {
  components: {
    GameCard,
  },
  props: ["games"],
};
</script>

<template>
  <main
    class="flex flex-col gap-14 w-screen min-h-screen items-center justify-center"
  >
    <div
      class="w-full flex flex-wrap items-center sm:justify-center flex-col sm:flex-row gap-10"
    >
      <GameCard v-for="game in games" :key="game.name" :game="game" />
    </div>
  </main>
</template>
