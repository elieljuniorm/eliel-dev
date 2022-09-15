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
*{
  max-width: 80vh;
  margin: auto;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
a{
  color: currentColor;
  text-decoration: unset;
  cursor: pointer;
}
</style>
