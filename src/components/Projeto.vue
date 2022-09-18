<template>

    <div v-for="projeto in projetos" :key="projeto.id" class="container">

        <div>
            <h3 class="textoTitulo">{{projeto.nome}}</h3>
            <p class="textoDescricao">{{projeto.descricao}}</p>
        </div>

        <div>
            <ul class="listaUl">
                <li class="linhaLi" v-for="habilidade in projeto.habilidades" :key="habilidade.id">{{habilidade}}</li>
            </ul>
        </div>

    </div>

    <div>
        <a href="https://github.com/elielm14" target="_blank" rel="noopener noreferrer" class="linkGitHub"><span><img src="@/assets/iconmonstr-github-1-240.png" alt="github" class="img"></span>Repositório Github</a>
    </div>

</template>

<script>
export default {
    name: 'ProjetoExperiencia',

    data() {
        return {
            projetos: {
                foto: {
                    nome: "Maia Fotografia, construído em Vue.Js",
                    descricao: "Maia Fotografia foi pensado para ser uma álbum de fotos de uma empresa fictícia especialista em casamentos(Teste técnico).",
                    habilidades: ["Vue.Js", "API REST", "Progressive Image", "Vue-Router", "Vue Resource"]
                },
                buscador: {
                    nome: "Fácil Consulta, construído em Vue.Js",
                    descricao: "Foi desenvolvido o Front-end de um Cadastro de Profissional da Saúde (médico), para o teste técnico da empresa Fácil Consulta.",
                    habilidades: ["React.js", "HTML", "CSS", "JavaScript", "API REST", "Axios"]
                },
                calculadora: {
                    nome: "Maia Transport, construído em React.Js",
                    descricao: "Maia Transport é uma calculadora de frete padrão de utilização do operador logístico fictício.",
                    habilidades: ["React.js", "HTML", "CSS", "JavaScript"]
                },
            },
        }
    },
}
</script>

<style scoped>
.container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 5px 5px;
    padding: 20px;
    background: #f5f5f5;
    border-radius: 4px;
}

.textoTitulo {
    font-size: 1.2rem;
    line-height: 1.1;
    font-weight: 700;
    margin-bottom: .5em;
}

.textoDescricao {
    text-align: start;
    line-height: 1.4;
}

.listaUl {
    display: flex;
    justify-items: center;
    flex-wrap: wrap;
    justify-content: space-around;
}

.linhaLi {
    list-style: none;
    background: white;
    border-radius: 4px;
    padding: 3px 3px;
    margin: .5em;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.linkGitHub {
    background-image: linear-gradient(to bottom, #8241f9, #4e277b);
    border-color: #150a27;
    color: #fff;
    padding: 0.75em 1.25em;
    border-radius: 6px;
}
.img{
    width: 1.5em;
    position: relative;
    top: 5px;
    right: 5px;
}
</style>