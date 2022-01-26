<template>
  <section class="container mb-4">
    <section class="offer">
      <img class="offer-image" src="@/assets/5.jpeg" />
      <div class="content-1">
        <h1 class="m-0">Etapy współpracy</h1>
      </div>
    </section>
  </section>

  <section class="container-flex pb-4">
    <div class="col-6 d-flex align-center">
      <div>
        <h1>Etap 1.</h1>
        <p>
          Bazą każdego projektu są informacje uzyskane od Klienta. Podczas
          rozmowy dowiadujemy się o jakich wnętrzach marzy, jakie ma
          przyzwyczajenia, styl życia oraz jakie ma oczekiwania do wnętrza. W
          tym celu prosimy też czasem o kilka przykładowych zdjęć dotyczących
          stylu w jakim ma być wykończone mieszkanie lub dom.
        </p>
      </div>
    </div>
    <div class="col-6 d-flex justify-right">
      <img src="@/assets/ph3.jpg" class="image w-75" />
    </div>
  </section>

  <section class="container-flex pb-4">
    <div class="col-6 d-flex justify-left">
      <img src="@/assets/1.jpeg" class="image w-75" />
    </div>
    <div class="col-6 d-flex align-center">
      <div>
        <h1>Etap 2.</h1>
        <p>
          Ten etap to spotkanie w miejscu, którego wnętrze mamy zaprojektować.
          Robimy tak nie tylko w celu zwymiarowania pomieszczenia, ale także po
          to aby poczuć energię jaka tam panuje, gdyż każde projektowanie wnętrz
          ma dla Nas inny, osobisty charakter.
        </p>
      </div>
    </div>
  </section>

  <section class="container-flex pb-4">
    <div class="col-6 d-flex align-center">
      <div>
        <h1>Etap 3.</h1>
        <p>
          Przygotowanie wizualizacji. Jest to etap na który Klient najbardziej
          czeka. W tym momencie właśnie zobaczy jak będzie wyglądało jego
          mieszkanie bądź dom. Jest to też moment na dyskusję o kolorach,
          strukturach, podłogach, układzie pomieszczeń lub mebli. Słuchamy
          ewentualnych uwag Klienta i wszystkie poprawki w projekcie nanosimy
          bezpłatnie.
        </p>
      </div>
    </div>
    <div class="col-6 d-flex justify-right">
      <img src="@/assets/ph2.jpg" class="image w-75" />
    </div>
  </section>

  <section class="container-flex pb-4">
    <div class="col-6 d-flex justify-left">
      <img src="@/assets/3.jpeg" class="image w-75" />
    </div>
    <div class="col-6 d-flex align-center">
      <div>
        <h1>Etap 4.</h1>
        <p>
          Po zaakceptowanym przez Klienta projekcie, przygotowujemy dokumentację
          techniczną zawierającą zestawienie materiałów, rozrys przyłączy
          hydraulicznych i elektrycznych, zwymiarowane zabudowy, wizualizację ,
          schemat układnaia płytek oraz inne nie zbędne do wykonania prac.
        </p>
      </div>
    </div>
  </section>

  <router-view></router-view>
</template>

<script></script>

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
