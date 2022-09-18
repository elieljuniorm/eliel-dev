<template>
    <div class="containerPricipal">

        <div v-for="curso in cursos" :key="curso.id" class="containerItens">

            <section class="sectionConteudo">

                <h3 class="titulo">{{curso.nome}}</h3>

                <p class="descricao">{{curso.habilidade}}</p>

                <span class="tempo">{{curso.tempo}}</span>

            </section>

        </div>
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
                car: {
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
.containerPricipal {
    display: flex;
    flex-wrap: wrap;
}

.containerItens {
    display: flex;
}

.sectionConteudo {
    background: #000;
    padding: .7em;
    margin: 1em .2em;
    border-radius: 4px;
    display: grid;
}

.titulo {
    font-size: 1.1rem;
    line-height: 1.4;
    margin-bottom: .5em;
    padding-left: .1em;
    color: #a3a3a3;
    border-left: 5px solid var(--cor-linhas);
}

.descricao {
    margin-bottom: .5em;
}

.tempo {
    font-size: 1.1rem;
    color: #a3a3a3;
}
</style>