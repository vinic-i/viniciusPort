<script>
    import { wpLink } from "../config";
    import {
        Hero,
        Reviews,
        Smallhero,
        Features,
        Services,
        Catalog,
        SearchBox,
        SelectService,
        OurProjects,
    } from "../components";
    let title="Destaque-se \n Online"
</script>

<style>
    .selo {
        width: 80px;
        position: absolute;
        top: 13%;
        left: 73%;
    }

    img {
        max-width: 100%;
    }
    .heroText {
        align-self: center;
        justify-content: center;
    }

    .rounded-lg {
        border-radius: 1rem !important;
    }

    .text-small {
        font-size: 0.9rem !important;
    }

    .custom-separator {
        width: 5rem;
        height: 6px;
        border-radius: 1rem;
    }

    .text-uppercase {
        letter-spacing: 0.2em;
    }
</style>

<!-- <div class="container">
    <img src="img/updates.svg" alt="secure" />
    <div class="heroText">
        <h2>Destaque-se Online</h2>
        <p>A gente pode te ajudar com isso</p>
    </div>
</div> -->
<Hero img="img/updates.svg" {title} subTitle="A gente pode te ajudar com isso"></Hero>
<div class="my-5 text-center">
    <h3>Nossos projetos</h3>
</div>
<OurProjects />
