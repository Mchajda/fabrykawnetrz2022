<template>
  <div :class="[container, 'justify-between align-center pb-2 pb-sm-0 pt-1']">
    <div class="col-6">
      <h2>{{ title }}</h2>
      <p>
        {{ text }}
      </p>
    </div>

    <div
      :class="[
        'col-6 d-flex d-flex-md justify-md-center w-sm-100',
        container == 'container-flex-reverse' ? '' : 'justify-right',
      ]"
    >
      <img
        :src="require(`@/assets/${image}`)"
        class="image w-100 shadow-2"
        alt="zdjęcie etapu"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "CooperationStage",
  props: {
    image: String,
    container: String,
    title: String,
    text: String,
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
