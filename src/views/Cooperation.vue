<template>
  <section class="container mb-4">
    <section class="offer">
      <img class="main-image" src="@/assets/5.jpeg" />
      <div class="content-1">
        <h1 class="m-0">Etapy współpracy</h1>
      </div>
    </section>
  </section>

  <section>
    <CooperationStage
      image="ph3.jpg"
      container="container-flex"
      title="Etap 1."
      text="Bazą każdego projektu są informacje uzyskane od Klienta. Podczas rozmowy
        dowiadujemy się o jakich wnętrzach marzy, jakie ma przyzwyczajenia, styl
        życia oraz jakie ma oczekiwania do wnętrza. W tym celu prosimy też
        czasem o kilka przykładowych zdjęć dotyczących stylu w jakim ma być
        wykończone mieszkanie lub dom."
    />

    <CooperationStage
      image="1.jpeg"
      container="container-flex-reverse"
      title="Etap 2."
      text="Ten etap to spotkanie w miejscu, którego wnętrze mamy zaprojektować.
            Robimy tak nie tylko w celu zwymiarowania pomieszczenia, ale także
            po to aby poczuć energię jaka tam panuje, gdyż każde projektowanie
            wnętrz ma dla Nas inny, osobisty charakter."
    />

    <CooperationStage
      image="ph2.jpg"
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
      image="3.jpeg"
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

    <div class="container-flex">
      <div class="col-3 d-flex justify-center">
        <div class="p-2">
          <h3>Piotr Rokicki</h3>
          <p style="">
            Polecam zdecydowanie wszystkim szukającym nowych inspiracji na
            odmianę domowego wnętrza. Sam skorzystałem i jestem bardzo
            zadowolony.
          </p>
          <div>
            <img
              v-for="n in 5"
              :key="n"
              src="@/assets/star.svg"
              style="padding: 0.5rem"
            />
          </div>
        </div>
      </div>
      <div class="col-3 d-flex justify-center">
        <div class="p-2">
          <h3>Piotr Rokicki</h3>
          <p style="">
            Polecam zdecydowanie wszystkim szukającym nowych inspiracji na
            odmianę domowego wnętrza. Sam skorzystałem i jestem bardzo
            zadowolony.
          </p>
          <div>
            <img
              v-for="n in 5"
              :key="n"
              src="@/assets/star.svg"
              style="padding: 0.5rem"
            />
          </div>
        </div>
      </div>
      <div class="col-3 d-flex justify-center">
        <div class="p-2">
          <h3>Piotr Rokicki</h3>
          <p style="">
            Polecam zdecydowanie wszystkim szukającym nowych inspiracji na
            odmianę domowego wnętrza. Sam skorzystałem i jestem bardzo
            zadowolony.
          </p>
          <div>
            <img
              v-for="n in 5"
              :key="n"
              src="@/assets/star.svg"
              style="padding: 0.5rem"
            />
          </div>
        </div>
      </div>
    </div>
  </section>

  <router-view></router-view>
</template>

<script>
import CooperationStage from "@/components/CooperationStage/CooperationStage.vue";

export default {
  name: "Cooperation",
  components: { CooperationStage },
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
