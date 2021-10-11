<template>
  <meu-painel class="fundowhite">
    <img id="img1" src="../shared/images/desktop-pagina-2.png" />
  </meu-painel>
</template>

<script>
import painelpg2Vue from "../shared/paineis/painelpg2.vue";
export default {
  components: {
    "meu-painel": painelpg2Vue,
  },
  name: "app",
};
</script>

<style>
html,
body {
  margin: 0 auto;
  background-color: #ffe766;
}
#img1 {
  margin-left: 550px;
  margin-right: 20px;
  margin-top: 150px;
  display: block;
}
</style>