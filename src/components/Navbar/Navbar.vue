<template>
  <div class="container">
    <div class="navbar shadow-2">
      <div class="nav-item">
        <router-link to="/"
          ><img src="@/assets/logofw.png" class="logo"
        /></router-link>
      </div>
      <div class="nav-item"><router-link to="/oferta">Oferta</router-link></div>
      <div class="nav-item">
        <router-link to="/etapy-wspolpracy">Etapy współpracy</router-link>
      </div>
      <div class="nav-item">
        <router-link to="/kontakt">Kontakt</router-link>
      </div>
    </div>
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
