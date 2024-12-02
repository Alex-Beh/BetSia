<script>
export default {
  props: ["points"],
};
</script>

<template>
  <nav
    class="fixed sm:px-20 py-8 bg-neutral bg-opacity-50 backdrop-blur-xl sm:bg-opacity-0 sm:backdrop-blur-0 w-screen flex flex-col sm:flex-row items-center justify-between z-40"
  >

    <!-- Left Section -->
    <div id="menu" class="flex items-center justify-between sm:w-1/3">
        <a class="font-semibold text-4xl" href="/BetSia/"
          >BetSia</a
        >
    </div>

    <!-- Right Section -->
    <div
      id="pointCounter"
      class="flex items-center justify-center gap-2 w-1/6"
    >
      <img
        src="/src/assets/icons/point.svg"
        alt="point"
        class="w-14 white-icon"
      />
      <p id="pointCounterContent" class="text-3xl">
        {{ points.toLocaleString("fi-FI") }}
      </p>
    </div>

  </nav>
</template>

<style scoped>
.white-icon {
  filter: brightness(0) saturate(100%) invert(100%) sepia(100%) saturate(17%)
    hue-rotate(241deg) brightness(105%) contrast(100%);
}
</style>
