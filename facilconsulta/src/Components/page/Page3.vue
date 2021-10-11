<template>
  <meu-painel class="fundowhite">
    <img id="img1" src="../shared/images/desktop-pagina-2.png" />
  </meu-painel>
</template>

<script>
import painelpg3Vue from "../shared/paineis/painelpg3.vue";
export default {
  components: {
    "meu-painel": painelpg3Vue,
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