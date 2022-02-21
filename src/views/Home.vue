<template>
  <section class="container">
    <section class="home">
      <img class="main-image" src="@/assets/5.webp" alt="Główne zdjęcie" />
      <div class="home-content">
        <h1>Fabryka Wnętrz</h1>
        <!-- <img src="@/assets/fabrykanet.png" class="fw-image" /> -->
        <p class="about-us-text">
          Jesteśmy firmą, która od wielu lat zajmuje się projektowaniem wnętrz.
          Każde zlecenie traktujemy jak nowe wyzwanie, które pozwala nam na
          wdrażanie kolejnych unikatowych inspiracji. Zespół Fabryki Wnętrz to
          młodzi ludzie z pasją, dla których zadowolenie Klienta jest najwyższą
          wartością. Podczas współpracy dzielimy się z Państwem swoim
          doświadczeniem zdobywanym przez cały okres naszej działalności. W
          związku z czym mają Państwo pewność, że zaproponowane przez nas
          rozwiązania są oparte o rzetelną wiedzę oraz najnowsze techniki
          zdobnicze.
        </p>
      </div>
    </section>
  </section>

  <section class="container mt-4 mb-4 m-sm-1">
    <h2>Nasi partnerzy:</h2>

    <div class="w-100"><PartnersList /></div>
  </section>
</template>

<script>
// @ is an alias to /src
import PartnersList from "@/components/PartnersList/PartnersList.vue";

export default {
  name: "Home",

  components: { PartnersList },
  methods: {
    toggleMenuInit() {
      const toggleButtonIcon = document.querySelector("img#toggleMenuIcon");
      const expandableMenu = document.getElementById("expandableMenu");

      console.log(toggleButtonIcon, toggleButtonIcon.src);

      expandableMenu.style.height = 0;
      toggleButtonIcon.src = "http://fabrykawnetrz.net/img/menu.723604de.svg";
    },
  },
  mounted: function () {
    this.toggleMenuInit();
  },
};
</script>

<style scoped>
@import "../styles/app.css";
@import "../styles/home.css";
</style>
