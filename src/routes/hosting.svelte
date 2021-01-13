<script>
    import {
        Hero,
        Reviews,
        Smallhero,
        Features,
        Services,
        Catalog,
        SearchBox,
        SelectService,
    } from "../components";
    import { wpLink } from "../config";
</script>

<style>
    h2 {
        font-size: 2.88651rem;
        line-height: 3.5rem;
    }
    p {
        line-height: 1.5;
        margin-bottom: 1rem;
    }
    .container {
        margin-left: auto;
        margin-right: auto;
        padding-left: 10px;
        padding-right: 10px;
    }
    .main-content {
        display: block;
    }
    .title-section {
        padding-top: 80px;
        padding-bottom: 80px;
        text-align: start;
    }
</style>

<Hero
    img="img/onlineConnection.svg"
    title="Site online e rapidinho?"
    subTitle="Veio no lugar certo!" />

<section class="main-content">
    <div class="title-section">
        <div
            data-aos="fade-left"
            data-aos-delay="100"
            class="container text-center">
            <h2>O que é hospedagem? Como funciona?</h2>
            <p class="lead mb-0">
                O que é hospedagem de site é um questionamento bastante
                recorrente para quem quer começar um blog, um site ou uma loja
                virtual na internet. Hospedagem de site é um serviço online que
                permite a publicação de um site ou aplicação na internet. Quando
                você adquire uma hospedagem, basicamente você está alugando um
                espaço dentro de um servidor. Nele ficam armazenados todos os
                arquivos e dados necessários para o bom funcionamento do site.
                Neste artigo, vamos explicar o que é hospedagem de sites em mais
                detalhes. Então vamos direto ao ponto!
            </p>
        </div>
    </div>
</section>

<Catalog />
