<template>

  <section class="conteudoInicial">
    <img src="https://avatars.githubusercontent.com/u/79880373?v=4" alt="Foto de Perfil" class="fotoPerfil">

    <div>
      <p class="textoFront">Desenvolvedor Front End</p>
      <p class="textoLocalizacao">Localizado em Ananindeu-PA</p>
    </div>
  </section>

  <section>
    <h2 id="experincia">Experiência</h2>
    <p>Desenvolvo projetos front end utlizando <strong>Vue.Js,</strong> <strong>React.Js</strong> e utlizando apenas
      <strong>HTML , CSS e JavaScript</strong>. Sólida experiência com consumo de <strong>API REST</strong>,
      responsividade mobile first e versionamento de código com <strong>Git e GitHub</strong>.
    </p>
  </section>
  <section class="containerProjeto">
    <Projeto />
  </section>
</template>

<script>
import Projeto from './Projeto.vue';

export default {
  name: "ExperienciaSection",
  components: { Projeto }
}
</script>

<style scoped>
.conteudoInicial {
  display: grid;
  grid-template-columns: 2fr 3fr;
  margin: .5em .5em 2em .5em;
}

.fotoPerfil {
  border-radius: 50%;
  display: block;
  margin-left: .5em;
  padding: .5em 0;
  width: 8em;
}

.textoFront {
  font-size: 22px;
  font-weight: bold;
}

.textoLocalizacao {
  font-size: 15px;
}

.containerProjeto {
  max-width: 1200px;
  padding: 40px 20px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr;
  gap: 50px;
}
</style>