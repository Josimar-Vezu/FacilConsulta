<template>
  <div class="fundowhite">
    <h1 id="titulo">{{ titulo }}</h1>

    <slot> </slot>
    <div class="painel">
      <h2 id="subtitulo">{{ subtitle }}</h2>

      <p class="especialidade">{{ especialidade }}</p>
      <input
        type="text"
        id="buttomespecialidade"
        placeholder="Selecione a Especialidade"
      />

      <p class="preco">{{ preco }}</p>
      <input type="text" id="buttompreco" placeholder="Informe o valor" />

      <p class="pagamento">{{ pagamento }}</p>
      <div class="backgroundpag">
        <input type="checkbox" class="buttompag" />
        <p id="pagtext">{{ pix }}</p>
      </div>

      <div class="backgroundpag">
        <input type="checkbox" class="buttompag" />
        <p id="pagtext">{{ dinheiro }}</p>
      </div>

      <div class="backgroundpag2">
        <p id="parcelatext1">Parcelamento em:</p>

        <input type="checkbox" id="buttomparcela" />
        <p id="parcelatext">1x, sem juros</p>
        <input type="checkbox" id="buttomparcela" />

        <p id="parcelatext">2x, sem juros</p>

        <input type="checkbox" id="buttomparcela" />
        <p id="parcelatext">3x, sem juros</p>

        <input type="checkbox" id="buttomparcela" />
        <p id="parcelatext">4x, sem juros</p>
      </div>
    </div>
  </div>
</template>

  <script>
export default {
  props: ["fundowhite"],
  name: "app",
  data() {
    return {
      titulo: "Sobre o Atendimento",
      subtitle: "Detalhes do Atendimento",
      especialidade: "Especialidade Principal*",
      preco: "Informe o preço da consulta",
      pagamento: "Formas de Pagamento da Consulta",
      pix: "Pix",
      dinheiro: "Em Dinheiro",
      cartaocredito: "Cartão de Crédito",
    };
  },
};
</script>

<style>
.fundowhite {
  width: 1200px;
  height: 820px;
  border-radius: 20px;
  border-color: #ffffff;
  background-color: #ffffff;
  border-style: solid;
  padding: 25px;
  margin-left: 350px;
  margin-top: 50px;
  flex-direction: column;
  justify-content: center;
}
.painel {
  margin-left: 120px;
  margin-top: -450px;
}
#titulo {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  color: #483698;
  font-size: 50px;
  margin-left: 120px;
}

#subtitulo {
  -webkit-font-smoothing: antialiased;
  font-size: 30px;
  margin-left: 0px;
}

#buttomespecialidade {
  border-radius: 7px;
  border-color: #282828;
  margin: 5px;
  width: 390px;
  height: 30px;
  margin-left: 0px;
}
#buttompreco {
  border-radius: 7px;
  border-color: #282828;
  margin: 5px;
  width: 290px;
  height: 30px;
  margin-left: 0px;
  display: inline-block;
}

.buttompag {
  border-radius: 15px;
  margin-left: 70px;
  margin-top: 5px;
}

.backgroundpag {
  width: 390px;
  height: 40px;
  border-radius: 10px;
  background-color: #f0f0f0;
  border-color: #eeeeee;
  box-shadow: 3px 3px 3px #cfcfcf;
  margin: 15px;
  margin-left: 0px;
}

.backgroundpag2 {
  width: 390px;
  height: 150px;
  border-radius: 10px;
  background-color: #f0f0f0;
  border-color: #eeeeee;
  box-shadow: 3px 3px 3px #cfcfcf;
  margin: 15px;
  margin-left: 0px;
}

#pagtext {
  margin-left: 30px;
  margin-top: 12px;
  display: inline-block;
}

#dinheiro {
  margin-left: 30px;
  margin-top: 12px;
  display: inline-block;
}
#parcelatext1 {
  margin-left: 5px;
  display: block;
}
#parcelatext {
  margin-top: 1px;
  margin: 1px;
}

#buttomparcela {
  margin: 5px;
  display: inline-block;
  margin-left: 25px;
}

#buttomroxo {
  width: 350px;
  height: 50px;
  border-radius: 15px;
  display: block;
  margin: 25px;
  background-color: #483698;
}

#buttomroxo,
#value {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  color: white;
  -webkit-font-smoothing: antialiased;
}
</style>