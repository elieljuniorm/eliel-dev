<template>

    <div v-for="projeto in projetos" :key="projeto.id" class="container">

        <h3 class="textoTitulo">{{projeto.nome}}</h3>

        <ul class="listaUl">
            <li class="linhaLi">{{projeto.habilidade}}</li>
        </ul>

        <p class="textoDescricao">{{projeto.descricao}}</p>

    </div>

</template>

<script>
export default {
    name: 'ProjetoExperiencia',

    data() {
        return {
            projetos: {
                calculadora: {
                    nome: "Calculadora",
                    descricao: "calduladora de frete em react, uahauhasuha m auhauhaua mkajaua iauahuan uiahuahuaha  uahuahuah",
                    habilidade: ["React.js", "HTML", "CSS", "JavaScript"]
                },
                foto: {
                    nome: "Maia fotos",
                    descricao: "site de fotografia feito em vue, uahaua , aauaunsa, auhauhau,,iunaunaunauass iauiauaunm",
                    habilidade: ["React.js", "HTML", "CSS", "JavaScript"]
                },
                buscador: {
                    nome: "Buscador de endereço",
                    descricao: "Entrega o endereço com base no cep feito em react, aybabaa aauhauhauah ahauyayhba uhauauybaa y",
                    habilidade: ["React.js", "HTML", "CSS", "JavaScript"]
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
    gap: 10px 20px;
    padding: 20px;
    margin-bottom: 20px;
    background: #f5f5f5;
    border-radius: 4px;
}

.textoTitulo {
    font-size: 1.2rem;
    line-height: 1.1;
    font-weight: 700;
    margin: 0;
}
.linhaLi{
    list-style: none;
    background: white;
    border-radius: 4px;
    padding: .8em;
}
</style>