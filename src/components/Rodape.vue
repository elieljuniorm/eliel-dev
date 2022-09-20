<template>
    <div class="container">
        <span class="copyDescricao">© Copyrigth Eliel Maia Developer 2022</span>
        <span class="copyDescricao">Design by Eliel Maia</span>
    </div>
</template>

<script>
export default {
    name: 'RodapeHome'
}
</script>

<style scoped>
.container{
    background: var(--cor-preto-padrao);
    color: var(--cor-cinza-padrao);
    display: flex;
    flex-direction: column;
    padding: 3em 0 2em 0;
}
.copyDescricao{
    font-style: italic;
    padding: .5em 0;
}
</style>