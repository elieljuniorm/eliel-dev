<template>

    <div v-for="curso in cursos" :key="curso.id" class="container">

        <h3>{{curso.nome}}</h3>

        <ul>
            <li>{{curso.habilidade}}</li>
        </ul>

        <span>{{curso.tempo}}</span>

    </div>

</template>

<script>
export default {
    name: 'CursoSection',
    data() {
        return {
            cursos: {
                alura: {
                    nome: 'Formação React',
                    habilidade: 'react.js',
                    tempo: '24 horas'
                },
                origamid: {
                    nome: 'Curso Completo de Vue',
                    habilidade: 'vue.js',
                    tempo: '34 horas'
                },
                dio: {
                    nome: 'Linguagem JavaScript',
                    habilidade: 'Javascript',
                    tempo: '50 horas'
                },
            }
        }
    }
}
</script>

<style scoped>

</style>