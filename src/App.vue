<template>
  <MenuNav />
  <Experiencia />
  <Formacao />
  <Contato />
  <Rodape />
</template>

<script>
import MenuNav from './components/MenuNav.vue';
import Experiencia from './components/Experiencia.vue';
import Formacao from './components/Formacao.vue';
import Contato from './components/Contato.vue';
import Rodape from './components/Rodape.vue';

export default {
  name: 'App',
  components: {
    MenuNav,
    Experiencia,
    Formacao,
    Contato,
    Rodape
  }
}
</script>

<style>
:root {
  --cor-linhas: #ffd700;
  --cor-cinza-padrao: #a3a3a3;
  --cor-preto-padrao: #000;
  --cor-preto-sombra: #141414;
  --cor-branco-gelo: #f1f1f1;
  --cor-branco-sombra: #dcdcdc;
  --margem: 100vh;
}

* {
  max-width: 100%;
  margin: auto;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

a {
  color: currentColor;
  text-decoration: unset;
  cursor: pointer;
}
</style>
