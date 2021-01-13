<script>
    import { goto } from "@sapper/app";
</script>

<style>
    .tableCard {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        column-gap: 2em;
    }
    /* .card {
        margin: 2em 0 2em 0;
        display: grid;
        grid-template-columns: 1fr 1fr;
    } */
    .titleCard {
        align-self: center;
    }
    a {
        text-decoration: none;
    }

    .grid-overlay {
        display: grid;
        grid-template-rows: 1rem 1rem auto;
        grid-template-columns: 2rem 2rem auto;
        overflow-y: visible;
        grid-row-gap: 1rem;
    }

    .a {
        grid-row: 1/4;
        grid-column: 1/4;
    }

    .b {
        grid-row: 2/4;
        grid-column: 2/4;
    }

    .c {
        grid-row: 3/4;
        grid-column: 3/4;
    }

    .a,
    .b,
    .c {
        position: relative;
        height: 15rem;
        width: 30rem;
    }

    .a .card,
    .b .card,
    .c .card {
        height: 15rem;
        width: 30rem;
        transition: 0.5s ease-in-out;
        position: absolute;
        top: 0;
        left: 0;
    }

    .grid-section .image:hover .c .card {
        top: 11rem;
        left: 1rem;
    }
    .grid-section .image:hover .a .card {
        top: -11rem;
        left: -1rem;
    }

    .section {
        min-height: 80vh;
    }

    .card-header {
        /* background: transparent;
        border: none; */
    }
    .grid-a{
        display: grid;
        align-content: center;
        justify-content: center;
    }
</style>

<section class="bg-primary text-white">
    <div class="container">
        <div class="row section">
            <div class="col-lg-6 grid-a">
                <div class="text">
                    <h2>Nossos serviços</h2>
                    <p>
                        Aqui na Mixou você vai encontrar todos os serviços
                        necessários para o seu empreendimento bombar na internet.
                        Contamos com uma equipe de especialistas para desenvolver
                        seu site e/ou aplicação, te ajudamos a encontrar um domínio
                        adequado para sua identidade online, e também conseguimos um
                        espaço para seu site ficar hospedado nesse mundo virtual!
                    </p>
                </div>
               
            </div>
            <div class="col-lg-6 grid-a">
                <div class="image">
                    <div class="grid-overlay">
                        <div class="a">
                            <div class="card bg-dark" on:click={() => goto('site')}>
                                <div class="card-header text-center">
                                    <b>SITE</b>
                                </div>
                                <div
                                    class="card-body"
                                    style="display: grid; grid-template-columns: 1fr 1fr">
                                    <div class="">
                                        <img
                                            src="img/Updates.svg"
                                            style="width:100%"
                                            alt="" />
                                    </div>
                                    <div class="text-center titleCard">
                                        <h5>PRECISO CRIAR MEU SITE</h5>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="b">
                            <div
                                class="card bg-dark"
                                on:click={() => goto('domain')}>
                                <div class="card-header text-center">
                                    <b>DOMÌNIOS</b>
                                </div>
                                <div
                                    class="card-body"
                                    style="display: grid; grid-template-columns: 1fr 1fr">
                                    <div class="">
                                        <img
                                            src="img/domainNames.svg"
                                            style="width:100%"
                                            alt="" />
                                    </div>
                                    <div class="text-center titleCard">
                                        <h5 class="">PRECISO DE UM DOMÍNIO</h5>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="c">
                            <div
                                class="card bg-dark"
                                on:click={() => goto('hosting')}>
                                <div class="card-header text-center">
                                    <b>HOSPEDAGEM</b>
                                </div>
                                <div
                                    class="card-body"
                                    style="display: grid; grid-template-columns: 1fr 1fr">
                                    <img
                                        src="img/onlineConnection.svg"
                                        style="width:100%"
                                        alt="" />
                                    <div class="text-center titleCard">
                                        <h5 class="">PRECISO HOSPEDAR MEU SITE</h5>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

          
        
    </div>
</section>
