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
    background: var(--cor-branco-gelo);
}

.tituloNome {
    padding: .5em 0;
    font-size: 2.5em;
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
    background: var(--cor-branco-sombra);
    border-radius: 4px;
}
</style>