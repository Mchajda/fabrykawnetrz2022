<template>
  <div class="container">
    <div class="navbar shadow-2 justify-between">
      <div
        class="d-flex d-flex-md d-flex-sm justify-between align-center mr-0 w-100"
      >
        <div class="nav-item m-sm-0">
          <router-link to="/" class="d-flex d-flex-md d-flex-sm"
            ><img src="@/assets/logofw.png" class="logo shadow-2" alt="logo" />
            <div class="d-flex-col" style="margin-top: 0.2rem">
              <img
                src="@/assets/fabrykawnetrz.png"
                class="logo2 shadow-2"
                alt="logo"
              /><img
                src="@/assets/projektowanieiaranzacja.png"
                class="logo2 shadow-2"
                alt="logo"
              />
            </div>
          </router-link>
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
          <div class="nav-item">
            <a href="https://www.facebook.com/fabrykawnetrz.net" target="_blank"
              ><img src="@/assets/facebook.png" class="mr-1 nav__social"
            /></a>
            <a
              href="https://www.instagram.com/fabrykawnetrz.net_/"
              target="_blank"
              ><img src="@/assets/instagram.png" class="nav__social"
            /></a>
          </div>
        </div>
        <div class="nav-item hidden sm-show mr-0">
          <a @click="expand"
            ><img src="@/assets/menu.svg" id="toggleMenuIcon"
          /></a>
        </div>
      </div>
      <div id="expandableMenu" class="transition">
        <div class="wrapper wrapperMenu">
          <ul class="pt-1">
            <li><router-link to="/oferta">Oferta</router-link></li>
            <li>
              <router-link to="/etapy-wspolpracy">Etapy współpracy</router-link>
            </li>
            <li><router-link to="/kontakt">Kontakt</router-link></li>
            <li>
              <a
                href="https://www.facebook.com/fabrykawnetrz.net"
                target="_blank"
                ><img src="@/assets/facebook.png" class="mr-1 nav__social"
              /></a>
            </li>
            <li>
              <a
                href="https://www.instagram.com/fabrykawnetrz.net_/"
                target="_blank"
                ><img src="@/assets/instagram.png" class="nav__social"
              /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    expand: function () {
      const toggleButtonIcon = document.querySelector("img#toggleMenuIcon");
      const expandableMenu = document.getElementById("expandableMenu");

      if (expandableMenu.clientHeight) {
        expandableMenu.style.height = 0;
        toggleButtonIcon.src = "http://fabrykawnetrz.net/img/menu.723604de.svg";
      } else {
        const wrapper = document.querySelector(".wrapper");
        expandableMenu.style.height = wrapper.clientHeight + "px";
        toggleButtonIcon.src =
          "http://fabrykawnetrz.net/img/close.28638fa8.svg";
      }
    },
  },
  mounted: function () {
    if (
      (navigator.userAgent.indexOf("iPhone") !== -1) |
      (navigator.userAgent.indexOf("Macintosh") !== -1)
    ) {
      const expandableMenu = document.getElementById("expandableMenu");
      expandableMenu.removeAttribute("class");
    }
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
