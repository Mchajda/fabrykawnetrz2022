<template>
  <div class="">
    <a class="d-flex-wrap align-center justify-center">
      <img
        v-for="partner in partners"
        :key="partner.name"
        :src="require(`@/assets/partners/${partner.image}`)"
        alt="partner"
        class="partner-image"
    /></a>
  </div>
</template>

<script>
export default {
  name: "PartnersList",
  data() {
    return {
      partners: [
        {
          image: "azzardo.webp",
          name: "Azzardo",
          url: "",
        },
        {
          image: "barlinek.webp",
          name: "Barlinek",
          url: "",
        },
        {
          image: "bloft.webp",
          name: "B-loft",
          url: "",
        },
        {
          image: "ELita.webp",
          name: "ELita",
          url: "",
        },
        {
          image: "elmax.pl.webp",
          name: "Elmax",
          url: "",
        },
        {
          image: "fluffo.webp",
          name: "Fluffo",
          url: "",
        },
        {
          image: "frezo.webp",
          name: "Frezo",
          url: "",
        },
        {
          image: "italux.webp",
          name: "Italux",
          url: "",
        },
        {
          image: "KERMI.webp",
          name: "Kermi",
          url: "",
        },
        {
          image: "kludi.webp",
          name: "Kludi",
          url: "",
        },
        {
          image: "kolo.webp",
          name: "Koło",
          url: "",
        },
        {
          image: "labra.webp",
          name: "Labra",
          url: "",
        },
        {
          image: "kohlman.webp",
          name: "Kohlman",
          url: "",
        },
        {
          image: "kratkipl.webp",
          name: "Kratki.pl",
          url: "",
        },
        {
          image: "logo_mirror.webp",
          name: "Mirror",
          url: "",
        },
        {
          image: "mebin.webp",
          name: "Mebin",
          url: "",
        },
        {
          image: "meble.webp",
          name: "meble.pl",
          url: "",
        },
        {
          image: "ORISTO.webp",
          name: "Oristo",
          url: "",
        },
        {
          image: "paradyz.webp",
          name: "Paradyż",
          url: "",
        },
        {
          image: "porta.webp",
          name: "Porta",
          url: "",
        },
        {
          image: "tubadzin.webp",
          name: "Tubadzin",
          url: "",
        },
      ],
    };
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
