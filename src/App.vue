<template>
  <Navbar />
  <router-view></router-view>
  <Footer />
</template>

<script>
import Navbar from "@/components/Navbar/Navbar.vue";
import Footer from "@/components/Footer/Footer.vue";

export default {
  name: "App",
  components: { Navbar, Footer },
};
</script>

<style scoped>
@import "./styles/app.css";

.nav {
  display: flex;
  justify-content: center;
}
</style>
