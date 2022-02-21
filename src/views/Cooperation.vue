<template>
  <LandingSection title="Etapy współpracy" />

  <section>
    <CooperationStage
      image="ph3.webp"
      container="container-flex"
      title="Etap 1."
      text="Bazą każdego projektu są informacje uzyskane od Klienta. Podczas rozmowy
        dowiadujemy się o jakich wnętrzach marzy, jakie ma przyzwyczajenia, styl
        życia oraz jakie ma oczekiwania do wnętrza. W tym celu prosimy też
        czasem o kilka przykładowych zdjęć dotyczących stylu w jakim ma być
        wykończone mieszkanie lub dom."
    />

    <CooperationStage
      image="1.webp"
      container="container-flex-reverse"
      title="Etap 2."
      text="Ten etap to spotkanie w miejscu, którego wnętrze mamy zaprojektować.
            Robimy tak nie tylko w celu zwymiarowania pomieszczenia, ale także
            po to aby poczuć energię jaka tam panuje, gdyż każde projektowanie
            wnętrz ma dla Nas inny, osobisty charakter."
    />

    <CooperationStage
      image="ph2.webp"
      container="container-flex"
      title="Etap 3."
      text="Przygotowanie wizualizacji. Jest to etap na który Klient najbardziej
            czeka. W tym momencie właśnie zobaczy jak będzie wyglądało jego
            mieszkanie bądź dom. Jest to też moment na dyskusję o kolorach,
            strukturach, podłogach, układzie pomieszczeń lub mebli. Słuchamy
            ewentualnych uwag Klienta i wszystkie poprawki w projekcie nanosimy
            bezpłatnie."
    />

    <CooperationStage
      image="3.webp"
      container="container-flex-reverse"
      title="Etap 4."
      text="Po zaakceptowanym przez Klienta projekcie, przygotowujemy
            dokumentację techniczną zawierającą zestawienie materiałów, rozrys
            przyłączy hydraulicznych i elektrycznych, zwymiarowane zabudowy,
            wizualizację , schemat układnaia płytek oraz inne nie zbędne do
            wykonania prac."
    />
  </section>

  <section class="container">
    <h2>Zaufali nam:</h2>

    <div class="container d-flex">
      <Referral
        v-for="refferalNumber in randomRefferals"
        :key="referrals[refferalNumber].name"
        :name="referrals[refferalNumber].name"
        :text="referrals[refferalNumber].text"
        :stars="referrals[refferalNumber].stars"
      />
    </div>
  </section>

  <router-view></router-view>
</template>

<script>
import CooperationStage from "@/components/CooperationStage/CooperationStage.vue";
import Referral from "@/components/Referral/Referral.vue";
import LandingSection from "@/components/LandingSection/LandingSection.vue";

export default {
  name: "Cooperation",
  components: { CooperationStage, Referral, LandingSection },

  data() {
    return {
      randomRefferals: [0, 1, 2],
      referrals: [
        {
          id: 1,
          name: "Janett Moon",
          text: "Zdecydowanie polecam! Pełen profesjonalizm począwszy od stworzenia oferty aż do odbioru końcowego. Jesteśmy zachwyceni naszym nowym wnętrzem.",
          stars: 5,
        },
        {
          id: 2,
          name: "Piotr Rokicki",
          text: "Polecam zdecydowanie wszystkim szukającym nowych inspiracji na odmianę domowego wnętrza. Sam skorzystałem i jestem bardzo zadowolony.",
          stars: 5,
        },
        {
          id: 3,
          name: "Maciej Macioszek",
          text: "Polecam zdecydowanie. Firma spełniła swoje zadanie.",
          stars: 5,
        },
        {
          id: 4,
          name: "Kaska michalewicz",
          text: "Budowa domu to czysta przyjemność pod okiem Fabryki Wnętrz. Wszystko wykonane wg, projektu. Wyszło pięknie.  Polecam.",
          stars: 5,
        },
        {
          id: 5,
          name: "Marcin Golab",
          text: "Najlepszy fachowiec w swojej dziedzinie... Pełna profesjonalna... Polecam każdemu kto marzy o wyjątkowym i niepowtarzalnym domu Panie Bartku bardzo dziękujemy",
          stars: 5,
        },
        {
          id: 6,
          name: "Sylwia andruszkiewicz",
          text: "Długo się zastanawiałam nad wykonaniem projektu. Zdecydowałam się i NIE żałuje. Projekt super. Polecam wszystkim Fabrykewnetrz chcącym zaoszczędzić sobie przeróbek w trakcie prac. Będę polecać wszystkim !!!",
          stars: 5,
        },
        {
          id: 7,
          name: "marta zdunczyk",
          text: "Gorąco polecam, otrzymałam świetny projekt.  Wszystkim będę polecać.",
          stars: 5,
        },
        {
          id: 8,
          name: "anna gierczak",
          text: "Bardzo polecam ! ! ! Super współpraca !  Jako jedyna firma nie bierze żadnych dodatkowych opłat za poprawki.  Projekt zrobiony dokładnie tak jak chciałam.",
          stars: 5,
        },
        {
          id: 9,
          name: "paweł sobolewski",
          text: "Całą współprace od pomiaru przez projektanta do samej wprowadzi do domu oceniam wzorowo.  Wszystkim polecam !",
          stars: 5,
        },
        {
          id: 10,
          name: "Anna Jędrzejczyk",
          text: "Zleciłam wykonanie projektu kuchni salonu i łazienki. Wyszło SUPER !!!!  Gorąco polecam.",
          stars: 5,
        },
        {
          id: 11,
          name: "Grzegorz Kmita",
          text: "Bardzo polecam. Nie sądziłem że remont może być przyjemny.",
          stars: 5,
        },
        {
          id: 12,
          name: "kasia molinska",
          text: "POLECAM !!!   Jestem bardzo zadowolona z wykonanego projektu.",
          stars: 5,
        },
        {
          id: 13,
          name: "kasia molinska",
          text: "POLECAM !!!   Jestem bardzo zadowolona z wykonanego projektu.",
          stars: 5,
        },
      ],
    };
  },

  methods: {
    toggleMenuInit() {
      const toggleButtonIcon = document.querySelector("img#toggleMenuIcon");
      const expandableMenu = document.getElementById("expandableMenu");

      expandableMenu.style.height = 0;
      toggleButtonIcon.src = "http://fabrykawnetrz.net/img/menu.723604de.svg";
    },

    getRandomRefferals() {
      const min = 0;
      const max = 12;

      for (let i = 0; i < 3; i++) {
        this.randomRefferals[i] = Math.floor(Math.random() * (max - min)) + min;
      }
    },
  },

  mounted: function () {
    this.toggleMenuInit();
    this.getRandomRefferals();
  },
};
</script>

<style>
@import "../styles/app.css";
@import "../styles/offer.css";

.offer-image {
  height: 90%;
  position: absolute;
  right: 0;
  top: 0;
}
</style>
