<template>

    <div id="formacao" class="containerCor">

        <section class="formacaoContainer">

            <h2 class="tituloFormacao">Formação</h2>

            <p class="formacaoTexto">
                Cursando <strong>Análise e Desenvolvimento de Sistemas</strong> na <strong>Estácio</strong>. Sou
                desesnvolvedor web extremamente motivado, e sempre estou em constante desenvolvimento de minhas
                habilidades.
            </p>

        </section>

        <section>
            <Curso />
        </section>

    </div>

</template>

<script>
import Curso from './Curso.vue';
export default {
    name: "FormacaoSection",
    components: { Curso }
}
</script>

<style scoped>
.containerCor {
    background: var(--cor-preto-sombra);
    color: var(--cor-branco-gelo);
    grid-template-columns: 1fr;
    padding: .2em 0;
    gap: 40px;
}

.formacaoContainer {
    padding-bottom: 1.5em;
    margin: 1em 1.5em;
    font-size: 1.12rem;
    line-height: normal;
}

.tituloFormacao {
    font-size: 3rem;
    font-weight: bold;
    padding: 0.5em 0;
}

.formacaoTexto {
    line-height: 1.5;
    border-left: 5px solid var(--cor-linhas);
    padding-left: 0.1rem;
}

@media only screen and (min-width: 1024px) {

    .tituloFormacao,
    .formacaoTexto {
        max-width: var(--margem);
    }
}
</style>