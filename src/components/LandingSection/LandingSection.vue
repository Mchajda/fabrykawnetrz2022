<template>
  <section class="container mb-4">
    <section class="offer">
      <img class="main-image" src="@/assets/5.jpeg" />
      <div class="content-1 shadow-2">
        <h1 class="m-0">{{ title }}</h1>
      </div>
    </section>
  </section>
</template>

<script>
export default {
  name: "LandingSection",
  props: {
    title: String,
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
