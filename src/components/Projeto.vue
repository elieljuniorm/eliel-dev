<template>
    <div v-for="projeto in projetos" :key="projeto.id">

        <h3>{{projeto.nome}}</h3>

        <p>{{projeto.descricao}}</p>

        <ul>
            <li>{{projeto.habilidade}}</li>
        </ul>

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

</style>