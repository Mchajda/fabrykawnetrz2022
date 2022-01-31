<template>
  <div :class="['justify-between align-center pb-4', container]">
    <div class="col-6">
      <h1>{{ title }}</h1>
      <p>
        {{ text }}
      </p>
    </div>

    <div
      :class="[
        'col-6 d-flex justify-md-center w-sm-100 d-flex-md',
        container == 'container-flex-reverse' ? '' : 'justify-right',
      ]"
    >
      <img :src="require(`@/assets/${image}`)" class="image w-100 shadow-2" />
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
