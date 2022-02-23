<template>
  <section class="container-flex h100vh" style="padding-top: 10rem">
    <div class="d-flex d-flex-md justify-md-center w-100 pt-1">
      <div class="col-3 col-md-3 col-sm-12 d-flex-md justify-sm-center">
        <img
          src="@/assets/bartek.webp"
          class="profile-image shadow-3"
          alt="Bartłomiej Chajda"
        />
      </div>
      <div
        class="col-9 col-md-9 d-flex align-center d-flex-sm justify-sm-center"
      >
        <div>
          <h1>Bartłomiej Chajda</h1>
          <h3>biuro@fabrykawnetrz.net</h3>
          <h3>tel. 502-445-239</h3>
        </div>
      </div>
    </div>
  </section>

  <section>
    <div style="height: 50vh">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2489.8594739767163!2d20.2850175159827!3d51.38726072730092!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4719bc684da25ee1%3A0x3b6bcf2ec1d22486!2s%C5%9Bw.Jana+33%2C+26-300+Opoczno!5e0!3m2!1spl!2spl!4v1459836310007"
        width="100%"
        height="100%"
        frameborder="0"
        style="border: 0"
        allowfullscreen
      ></iframe>
    </div>
  </section>

  <router-view></router-view>
</template>

<script>
export default {
  name: "Contact",
  components: {},

  mounted: function () {
    const toggleButtonIcon = document.querySelector("img#toggleMenuIcon");
    const expandableMenu = document.getElementById("expandableMenu");

    expandableMenu.style.height = 0;
    toggleButtonIcon.src = "http://fabrykawnetrz.net/img/menu.723604de.svg";
  },
};
</script>

<style>
@import "../styles/app.css";
@import "../styles/offer.css";
</style>
