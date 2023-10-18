<template>
  <div class="search-bar">
    <fieldset class="f">
      <legend class="legenda">Pesquisar</legend>
      <p class="placeholder">Procure uma disciplina</p>
      <img class="ft" src="~/assets/search.jpg">
    </fieldset>
  </div>
</template>

<script>
export default {
  data() {
    return {
      searchQuery: "",
    };
  },
  methods: {
    handleInput() {
      // Este método é chamado sempre que o usuário digita algo na barra de pesquisa.
      // Você pode adicionar lógica adicional aqui, se necessário.
    },
    search() {
      // Este método é chamado quando o botão "Buscar" é clicado.
      // Você pode realizar a lógica de pesquisa aqui, como fazer uma chamada à API.
      // Neste exemplo, apenas exibimos a consulta no console.
      console.log("Pesquisando por: " + this.searchQuery);
    },
  },
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,400;1,500&display=swap');
.f{
  position:absolute;
  margin-left: 200px;
  margin-top: 78px;
  border-radius: 8px;
  border: 2px solid #B2D2B7;
  width: 485px;
  height: 39px;
}
.legenda{
  color: #9AB69E;
  font-family: Poppins;
  font-size: 11px;
  font-style: normal;
  font-weight: 590;
  line-height: normal;
}
.placeholder{
  color: #9AB69E;
  font-family: Poppins;
  font-size: 15px;
  font-style: normal;
  font-weight: 590;
  line-height: normal;
}
.ft{
  position: absolute;
  margin-left: 460px;
  margin-top: 12px;
  width: 16px;
  height: 18.215px;
  flex-shrink: 0;
  }

</style>

