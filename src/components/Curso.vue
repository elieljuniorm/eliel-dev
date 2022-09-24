<template>
    <div class="containerPricipal">

        <div v-for="curso in cursos" :key="curso.id" class="containerItens">

            <section class="sectionConteudo">

                <h3 class="titulo">{{curso.nome}}</h3>

                <p class="descricao">{{curso.empresa}}</p>

                <span class="tempo">{{curso.tempo}}</span>

            </section>

        </div>

    </div>

    <div class="botaoDrive">
        <a href="https://drive.google.com/drive/folders/1_zHOoao6EbtROksQa2qi63DvYSmeNEI3?usp=sharing" target="_blank"
            rel="noopener noreferrer" class="linkDrive">Baixar Currículo</a>
        <a href="https://drive.google.com/drive/folders/1_jH8zkooMPOthT3OpmfhzPQ6VWA9Fq67?usp=sharing" target="_blank"
            rel="noopener noreferrer" class="linkDrive">Certificados</a>
    </div>

</template>

<script>
export default {
    name: 'CursoSection',
    data() {
        return {
            cursos: {
                react: {
                    nome: 'React Completo',
                    empresa: 'Origamid',
                    tempo: '36 horas'
                },
                reactAlura: {
                    nome: 'Formação React',
                    empresa: 'Alura',
                    tempo: '24 horas'
                },
                vue: {
                    nome: 'Formação Vue.Js',
                    empresa: 'Alura',
                    tempo: '55 horas'
                },
                javascript: {
                    nome: 'Linguagem JavaScript',
                    empresa: 'Alura',
                    tempo: '50 horas'
                },
                front: {
                    nome: 'Formação Front-end - HTML5 e CSS3',
                    empresa: 'Alura',
                    tempo: '52 horas'
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
    background: var(--cor-preto-padrao);
    padding: .7em;
    margin: 1em .2em;
    border-radius: 4px;
    display: grid;
}

.titulo {
    font-size: 1.1rem;
    line-height: 1.4;
    margin-bottom: .5em;
    padding-left: 0.3em;
    color: var(--cor-cinza-padrao);
    border-left: 5px solid var(--cor-linhas);
}

.descricao {
    margin-bottom: .5em;
}

.tempo {
    font-size: 1.1rem;
    color: var(--cor-cinza-padrao);
}

.botaoDrive {
    display: flex;
    margin: 2em 0;
}

.linkDrive {
    background: var(--cor-preto-padrao);
    color: var(--cor-cinza-padrao);
    padding: 0.7em;
    border-radius: 4px;
    font-size: 15px;
    text-transform: uppercase;
    font-weight: bold;
    box-shadow: -2px 2px;
}

.linkDrive:hover {
    background: var(--cor-preto-sombra);
    transition: 200ms;
}

@media only screen and (min-width: 1024px) {
    .containerPricipal {
        max-width: var(--margem);
    }

    .botaoDrive {
        margin: 2em auto;
        max-width: 50%;
    }
}
</style>