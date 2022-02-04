<template>
  <section class="container mb-4 mb-md-2">
    <section class="offer">
      <img class="main-image" src="@/assets/5.webp" alt="Główne zdjęcie" />
      <div class="content-1 shadow-2">
        <h1 class="m-0">{{ title }}</h1>
        <p v-if="text" class="about-us-text">
          {{ text }}
        </p>
      </div>
    </section>
  </section>
</template>

<script>
export default {
  name: "LandingSection",
  props: {
    title: String,
    text: String,
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
