<template>
  <section class="container"><Navbar /></section>
  <router-view></router-view>
</template>

<script>
import Navbar from "@/components/Navbar/Navbar.vue";
export default {
  name: "App",
  components: { Navbar },
};
</script>

<style scoped>
@import "./styles/app.css";

.nav {
  display: flex;
  justify-content: center;
}
</style>
