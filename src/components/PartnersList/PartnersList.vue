<template>
  <div class="d-flex-wrap align-center justify-center">
    <a
      :href="partner.url"
      target="_blank"
      v-for="partner in partners"
      :key="partner.name"
      class=""
    >
      <img
        :src="require(`@/assets/partners/${partner.image}`)"
        :alt="partner.name"
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
          url: "https://azzardo.com.pl/",
        },
        {
          image: "barlinek.webp",
          name: "Barlinek",
          url: "https://www.barlinek.com.pl/",
        },
        {
          image: "bloft.webp",
          name: "B-loft",
          url: "http://b-loft.pl/",
        },
        {
          image: "ELita.webp",
          name: "ELita",
          url: "https://elitameble.pl/",
        },
        {
          image: "elmax.pl.webp",
          name: "Elmax",
          url: "https://elmax.pl/",
        },
        {
          image: "fluffo.webp",
          name: "Fluffo",
          url: "https://fluffo.pl/pl/",
        },
        {
          image: "frezo.webp",
          name: "Frezo",
          url: "https://frezo.pl/",
        },
        {
          image: "italux.webp",
          name: "Italux",
          url: "https://www.italux.pl/pl/",
        },
        {
          image: "KERMI.webp",
          name: "Kermi",
          url: "https://www.kermi.pl/",
        },
        {
          image: "kludi.webp",
          name: "Kludi",
          url: "https://www.kludi.com/pl/",
        },
        {
          image: "kolo.webp",
          name: "Koło",
          url: "https://www.kolo.com.pl/",
        },
        {
          image: "labra.webp",
          name: "Labra",
          url: "https://labra.pl/",
        },
        {
          image: "kohlman.webp",
          name: "Kohlman",
          url: "https://kohlman.com.pl/",
        },
        {
          image: "kratkipl.webp",
          name: "Kratki.pl",
          url: "https://kratki.com/pl/",
        },
        {
          image: "logo_mirror.webp",
          name: "Mirror",
          url: "https://www.mirror.com.pl/",
        },
        {
          image: "mebin.webp",
          name: "Mebin",
          url: "https://www.mebin.pl/",
        },
        {
          image: "meble.webp",
          name: "meble.pl",
          url: "https://www.meble.pl/",
        },
        {
          image: "ORISTO.webp",
          name: "Oristo",
          url: "https://www.oristo.pl/",
        },
        {
          image: "paradyz.webp",
          name: "Paradyż",
          url: "https://www.paradyz.com/",
        },
        {
          image: "porta.webp",
          name: "Porta",
          url: "https://www.porta.com.pl/",
        },
        {
          image: "tubadzin.webp",
          name: "Tubadzin",
          url: "https://www.tubadzin.pl/",
        },
      ],
    };
  },
};
</script>

<style scoped>
@import "./style.css";
</style>
