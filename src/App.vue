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

</style>
