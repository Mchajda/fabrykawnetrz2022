<template>
  <div class="col-3 d-flex justify-center">
    <div class="p-2">
      <h3 class="">{{ name }}</h3>
      <p class="">
        {{ text }}
      </p>
      <div>
        <img
          v-for="n in stars"
          :key="n"
          src="@/assets/star.svg"
          :style="['padding: 0.5rem', n === 1 ? 'padding-left : 0' : '']"
          class="shadow-1"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Referral",
  props: {
    name: String,
    text: String,
    stars: Number,
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
