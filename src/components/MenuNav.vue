<template>

    <div class="container">

        <h1 class="tituloNome">Eliel Maia</h1>

        <nav>

            <ul class="listaUl">

                <li class="linkLi"><a href="#experincia">Experiência</a></li>
                <li class="linkLi"><a href="#formacao">Formação</a></li>
                <li class="linkLi"><a href="#contato">Contato</a></li>

            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'MenuNavHome'
}
</script>

<style scoped>
.container {
    display: flex;
    align-items: center;
    flex-direction: column;
    padding: 1.5em 0;
}

.tituloNome {
    padding: .5em 0;
}
.tituloNome::before{
    content: "";
    display: block;
    width: 4em;
    height: 4em;
    background: url(@/assets/imagem-transparente2.png) no-repeat center;
    position: absolute;
    top: 1em;
    left: 3em;
    z-index: -1;
}
.listaUl {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.linkLi {
    list-style: none;
    font-weight: 500;
    font-size: 20px;
    margin: .5em 0;
    padding: .5em 1.5em;
    background: #f5f5f5;
    border-radius: 4px;
}
</style>