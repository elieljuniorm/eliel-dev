<template>

  <Header />
  <Experiencia />
  <Formacao />
  <Contato />

</template>

<script>
import Header from './components/Header.vue';
import Experiencia from './components/Experiencia.vue';
import Formacao from './components/Formacao.vue';
import Contato from './components/Contato.vue';

export default {
  name: 'App',
  components: {
    Header,
    Experiencia,
    Formacao,
    Contato
  }
}
</script>

<style>

</style>
