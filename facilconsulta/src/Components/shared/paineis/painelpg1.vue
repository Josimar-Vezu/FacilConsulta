<template>
  <div class="fundowhite">
    <h1 id="titulo">{{ titulo }}</h1>

    <slot> </slot>
    <div class="painelcadastro">
      <h2 id="subtitulo">{{ subtitle }}</h2>

      <p class="nomecadastro">{{ nome }}</p>
      <input type="text" id="buttomnome" placeholder="Digite o Nome" />

      <p class="cpf">{{ cpf }}</p>
      <input type="text" id="buttomcpf" placeholder="Digite o CPF" />

      <p class="celular">{{ numerocel }}</p>
      <input type="text" id="buttomcel" placeholder="Numero de Telefone" />

      <div class="buttomestado">
        <p id="estadotext">{{ estado }}</p>
        <select name="Estado" class="estadobut">
          <option value="selecione">Selecione</option>
          <option value="Londrina">City1</option>
          <option value="rio grande do sul">City2</option>
          <option value="santa catarina">City3</option>
        </select>
      </div>

      <div class="buttomcidade">
        <p id="cidadetext">{{ cidade }}</p>
        <select name="Cidade" class="cidadebut">
          <option value="selecione">Selecione</option>
          <option value="parana">Paraná</option>
          <option value="rio-grande">Rio Grande do Sul</option>
          <option value="santa-catarina">Santa Catarina</option>
        </select>
      </div>
      <li id="page2buttom"><a href="/Page2" id="textbuttom">PRÓXIMO</a></li>
    </div>
  </div>
</template>

  <script>
export default {
  props: ["fundowhite"],
  name: "app",
  data() {
    return {
      titulo: "Sobre o Profissional",
      subtitle: "Dados do Profissional",
      nome: "Nome completo*",
      cpf: "CPF*",
      numerocel: "Numero de celular",
      estado: "Estado*",
      cidade: "Cidade*",
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
  background-color: white;
  border-style: solid;
  padding: 25px;
  margin-left: 350px;
  margin-top: 50px;
  flex-direction: column;
  justify-content: center;
}
.painelcadastro {
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

#buttomnome {
  border-radius: 7px;
  border-color: #282828;
  margin: 5px;
  width: 390px;
  height: 30px;
}
#buttomcpf {
  border-radius: 7px;
  border-color: #282828;
  margin: 5px;
  width: 290px;
  height: 30px;
}

#buttomcel {
  border-radius: 7px;
  border-color: #282828;
  margin: 5px;
  width: 290px;
  height: 30px;
  display: block;
}
.buttomcidade,
.buttomestado {
  display: inline-block;
}

.cidadebut {
  border-radius: 7px;
  width: 170px;
  height: 35px;
  margin: 15px;
}

.estadobut {
  border-radius: 7px;
  width: 170px;
  height: 35px;
}

#page2buttom {
  width: 350px;
  height: 50px;
  border-radius: 15px;
  margin: 25px;
  background-color: #483698;
}

#textbuttom {
  margin-left: 120px;
  margin-top: 50px;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  color: #ffffff;
  -webkit-font-smoothing: antialiased;
}

#buttomroxo,
#value {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  color: white;
  -webkit-font-smoothing: antialiased;
}
</style>