<template>
  <section class="container mb-4">
    <section class="offer">
      <img class="offer-image" src="@/assets/5.jpeg" />
      <div class="content-1">
        <h1 class="m-0">Oferta</h1>
      </div>
    </section>
  </section>
  <section class="container-flex mb-4">
    <div class="col-6">
      <div class="pb-2">
        <h2 class="content-2">Fabryka Wnętrz swoim Klientom oferuje:</h2>
      </div>

      <ul class="pl-2">
        <li>projektowanie wnętrz mieszkalnych, biurowych i handlowych</li>
        <li>aranżacja wnętrz</li>
        <li>
          projekty pojedynczych pomieszczeń ( łazienka, kuchnia, salon,
          sypialnia )
        </li>
        <li>
          doradztwo w zakresie doboru materiałów budowlanych i wykończeniowych
        </li>
        <li>doradztwo w zakresie doboru materiałów dekoracyjnych.</li>
      </ul>
    </div>
    <div class="col-6">
      <div class="pb-2">
        <h2 class="content-2">
          W ramach projektu Klient otrzymuje rysunki techniczne uwzględniające:
        </h2>
      </div>

      <ul class="pl-2">
        <li>wizualizację</li>
        <li>
          szczegółowy układ funkcjonalny z zaznaczeniem ewentualnych przeróbek
          ścian
        </li>
        <li>rozrys przyłączy hydraulicznych i elektrycznych</li>
        <li>rozrys sufitów podwieszanych</li>
        <li>rozrys zaprojektowanych zabudów gipsowo-kartonowych</li>
        <li>dobór kolorystyki ścian</li>
        <li>dobór drzwi</li>
        <li>dobór ceramiki i armatury sanitarnej</li>
        <li>dobór lamp i opraw oświetleniowych</li>
        <li>
          projekt mebli indywidualnych wraz z wymiarami ( zabudowy wnęk, szafy,
          szafki łazienkowe, zabudowa kominka, meble kuchenne)
        </li>
        <li>
          dobór okładzin ( szkła, kamienia, płyt laminowanych , płytek ściennych
          i podłogowych)
        </li>
        <li>widoki ścian z rozrysowanym schematem układania płytek</li>
        <li>zestawieni sprzętu AGD</li>
        <li>zestawienie materiałów</li>
      </ul>
    </div>
  </section>
  <section class="container pb-4">
    <p>
      <span class="content-4">Na Państwa życzenie</span> możemy również objąć
      projekt nadzorem autorskim oraz towarzyszyć Państwu w trudach związanych z
      zakupami niezbędnych do stworzenia wymarzonego wnętrz materiałów
      budowlanych czy dekoracyjnych.
    </p>
    <p>
      Projektowanie wnętrz to nie tylko nasz zawód, ale i pasją od wielu lat.
      Nieustannie śledzimy nowe trendy i rozwiązania w wykańczaniu wnętrz oraz
      architekturze. Dzięki temu nasze projekty łączą w sobie autorską
      wizualizację ze współczesnym podejściem do kreowania przestrzeni.
    </p>
    <p>
      Siedziba naszego biura znajduje się w Opocznie, ale dzięki obecnej
      technologii jesteśmy w stanie wykonywać projekty na terenie całego kraju.
    </p>
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
