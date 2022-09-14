<template>

  <div>
    <img src="https://avatars.githubusercontent.com/u/79880373?v=4" alt="Foto de Perfil">
  </div>

  <section>
    <p>Desenvolvedor Front End</p>
    <p>Localizado em Ananindeu-PA</p>
  </section>

  <section>
    <h2 id="experincia">Experiência</h2>
    <p>Desenvolvo projetos front end utlizando <strong>Vue.Js,</strong> <strong>React.Js</strong> e utlizando apenas
      <strong>HTML , CSS e JavaScript</strong>. Sólida experiência com consumo de <strong>API REST</strong>,
      responsividade mobile first e versionamento de código com <strong>Git e GitHub</strong>.
    </p>
  </section>
  <div class="containerProjeto">
    <Projeto />
  </div>
</template>

<script>
import Projeto from './Projeto.vue';

export default {
  name: "ExperienciaSection",
  components: { Projeto }
}
</script>

<style scoped>
.containerProjeto {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr;
  gap: 50px;
}
</style>
