<template>
  <section class="container-fluid d-flex align-center p-4 p-sm-3 bg-dark">
    <div class="col-3 d-flex justify-center">
      <div>
        <h4 class="company-name pb-1">Fabryka Wnętrz</h4>
        <h4>26-300 Opoczno</h4>
        <h4>ul. Św. Jana 33</h4>
      </div>
    </div>
    <div class="col-3 d-flex justify-evenly align-center">
      <a href="https://www.facebook.com/fabrykawnetrz.net" target="_blank"
        ><img src="@/assets/facebook.png" class="mr-md-2" style="width: 2rem"
      /></a>
      <a href="https://www.instagram.com/fabrykawnetrz.net_/" target="_blank"
        ><img src="@/assets/instagram.png" class="" style="width: 2rem"
      /></a>
    </div>
    <div class="col-3 d-flex justify-center">
      © Copyright FABRYKA WNĘTRZ 2015
    </div>
  </section>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
@import "./style.css";
</style>
