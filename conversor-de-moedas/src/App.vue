<template>
  <div id="app">
    <div class="logo">
      <img alt="Vue logo" src="./assets/logo.png" />
      <h1>Conversor de Moedas</h1>
    </div>
    <div class="linha">
      <Conversor moedaA="USD" moedaB="BRL" />
      <Conversor moedaA="BRL" moedaB="USD" />
    </div>
    <div class="linha">
      <Conversor moedaA="CAD" moedaB="BRL" />
      <Conversor moedaA="BRL" moedaB="CAD" />
    </div>
    <div class="linha">
      <Conversor moedaA="EUR" moedaB="BRL" />
      <Conversor moedaA="BRL" moedaB="EUR" />
    </div>
    <h6 class="logo"><i>By Edésio Gonçalves</i></h6>
  </div>
</template>

<script>
//importa o componente criado na pasta "components"
import Conversor from "./components/Conversor.vue";
export default {
  name: "app",
  components: {
    Conversor, //criado na pasta: components
  },
};
</script>

<style>
#app {
  margin: auto;
  max-width: 900px;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
.linha {
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}
.logo {
  text-align: center;
}
</style>