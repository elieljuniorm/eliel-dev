<template>
    <div class="containerCor">

        <div id="contato" class="container">

            <h2 class="titulo">Contato</h2>
            <p class="descricao">Estou disponível para novos projetos e jobs. Entre em contato comigo e marcamos uma
                conversa 👋</p>

            <div class="contato">
                <a href="https://api.whatsapp.com/send?phone=5591986060649" target="_blank" rel="noopener noreferrer"
                    class="linkContato">+55 (91) 9 8606-0649</a>
                <a href="http://www.linkedin.com/in/eliel-maia/" target="_blank" rel="noopener noreferrer"
                    class="linkContato"><img src="@/assets/iconmonstr-linkedin-3-240.png" alt="Linkedin icone" class="img"> Linkedin</a>
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
    background: #000;
    color: #fff;
    padding-top: 1em;
}

.container {
    margin: 0 1.5em;
    font-size: 1.12rem;
    line-height: normal;
}

.titulo {
    font-size: 3rem;
    font-weight: bold;
    padding: 0.5em 0;
}

.descricao {
    line-height: 1.5;
    border-left: 5px solid var(--cor-linhas);
    padding-left: 0.1rem;
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
    background: #141414;
    padding: 0.7em;
    margin: 1em 0.2em;
    border-radius: 4px;
    border-left: 5px solid var(--cor-linhas);
    padding-left: 0.1rem;
}
.img{
    width: 1em;
    position: relative;
    top: 4px;
    right: 3px;
    margin-left: .3em;
}
</style>