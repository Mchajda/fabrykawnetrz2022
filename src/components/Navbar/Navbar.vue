<template>
  <div class="navbar">
    <div class="nav-item">
      <router-link to="/"
        ><img src="@/assets/logofw.png" class="logo"
      /></router-link>
    </div>
    <div class="nav-item"><router-link to="/oferta">Oferta</router-link></div>
    <div class="nav-item">Etapy współpracy</div>
    <div class="nav-item">Kontakt</div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
@import "./style.css";
</style>
