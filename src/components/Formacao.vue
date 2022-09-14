<template>
    <div>
        <section>
            <h2>Formação</h2>
            <p class="formacao-texto">
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

</style>