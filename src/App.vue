<template>

  <Header />
  <Experiencia />
  <Formacao />

</template>

<script>
import Header from './components/Header.vue';
import Experiencia from './components/Experiencia.vue';
import Formacao from './components/Formacao.vue';

export default {
  name: 'App',
  components: {
    Header,
    Experiencia,
    Formacao,
  }
}
</script>

<style>

</style>
