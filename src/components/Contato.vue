<template>
    <div class="containerCor">

        <div id="contato" class="container">

            <h2 class="titulo">Contato</h2>
            <p class="descricao">Estou disponível para novos projetos e jobs. Entre em contato comigo e marcamos uma
                conversa 👋</p>

            <div class="contato">
                <a href="https://api.whatsapp.com/send?phone=5591986060649" target="_blank" rel="noopener noreferrer"
                    class="linkContato hoverlink">+55 (91) 98606-0649</a>
                <a href="http://www.linkedin.com/in/eliel-maia/" target="_blank" rel="noopener noreferrer"
                    class="linkContato hoverlink"><img src="@/assets/iconmonstr-linkedin-3-240.png" alt="Linkedin icone"
                        class="img"> Linkedin</a>
                <p class="linkContato">elieljuniorm@gmail.com</p>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: 'ContatoSection'
}
</script>

<style scoped>
.containerCor {
    background: var(--cor-preto-sombra);
    color: var(--cor-branco-gelo);
    padding-top: 1em;
}

.container {
    margin: 0 1.5em;
    font-size: 1.12rem;
    line-height: normal;
}

.titulo {
    font-size: 2em;
    font-weight: bold;
    padding: 0.5em 0;
}

.descricao {
    line-height: 1.5;
    border-left: 5px solid var(--cor-linhas);
    padding-left: 0.3em;
    margin: 1em 1.5em 2.5em 1.5em;
    font-size: 1.12rem;
    line-height: normal;
}

.contato {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.linkContato {
    margin: 1em 0;
    background: var(--cor-preto-padrao);
    padding: 0.7em;
    margin: 1em 0.2em;
    border-radius: 4px;
    border-left: 5px solid var(--cor-linhas);
    padding-left: 0.3em;
}

.hoverlink:hover {
    border: none;
    padding-left: 7px;
}

.img {
    width: 1em;
    position: relative;
    top: 4px;
    right: 3px;
    margin-left: .3em;
}

@media only screen and (min-width: 1024px) {
    .titulo {
        max-width: var(--margem);
    }

    .descricao {
        max-width: var(--margem);
        margin: 0 auto;
    }

    .contato {
        flex-wrap: nowrap;
        flex-direction: row;
        justify-content: center;
    }
    .linkContato{
        margin: 3em 1em;
    }
}
</style>