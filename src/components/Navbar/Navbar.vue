<template>
  <div class="container">
    <div class="navbar shadow-2 justify-between">
      <div class="nav-item">
        <router-link to="/"
          ><img src="@/assets/logofw.png" class="logo shadow-2"
        /></router-link>
      </div>
      <div class="d-flex d-flex-md align-center justify-right sm-hidden">
        <div class="nav-item">
          <router-link to="/oferta">Oferta</router-link>
        </div>
        <div class="nav-item">
          <router-link to="/etapy-wspolpracy">Etapy współpracy</router-link>
        </div>
        <div class="nav-item">
          <router-link to="/kontakt">Kontakt</router-link>
        </div>
      </div>

      <div class="nav-item hidden sm-show mr-0">
        <a @click="expand"
          ><img src="@/assets/menu.svg" id="toggleMenuIcon"
        /></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    expand: function () {
      const navbar = document.querySelector("div.navbar");
      const toggleButtonIcon = document.querySelector("img#toggleMenuIcon");

      if (
        toggleButtonIcon.src === "http://localhost:8080/img/menu.723604de.svg"
      ) {
        toggleButtonIcon.src = "http://localhost:8080/img/close.28638fa8.svg";
        //navbar.setAttribute("class", "red");
        console.log(navbar.getClass);
      } else {
        toggleButtonIcon.src = "http://localhost:8080/img/menu.723604de.svg";
      }
    },
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
