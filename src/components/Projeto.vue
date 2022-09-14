<template>
    <div v-for="projeto in projetos" :key="projeto.id" class="container">

        <h3>{{projeto.nome}}</h3>

        <ul>
            <li>{{projeto.habilidade}}</li>
        </ul>

        <p>{{projeto.descricao}}</p>

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
                    descricao: "calduladora de frete em react",
                    habilidade: "react"
                },
                foto: {
                    nome: "Maia fotos",
                    descricao: "site de fotografia feito em vue",
                    habilidade: "vue"
                },
                buscador: {
                    nome: "Buscador de endereço",
                    descricao: "Entrega o endereço com base no cep feito em react",
                    habilidade: "react"
                },
            },
        }
    }
}
</script>

<style scoped>
.container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px 20px;
    padding: 20px;
    background: #f5f5f5;
    margin-bottom: 20px;
    border-radius: 4px;
}
</style>