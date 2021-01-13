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
    } from "../components";
</script>

<style>
    .container {
        display: grid;
        height: 60vh;
    }
    .heroText {
        align-self: center;
        justify-content: center;
    }
</style>

<!-- <div class="container">
    <div class="heroText">
        <h2>Garanta seu domínio agora.</h2>
        <p>A gente pode te ajudar com isso</p>
    </div>
</div> -->
<Hero
    showButton={false}
    img="img/domainNames.svg"
    title="Garanta seu domínio agora."
    subTitle="A gente pode te ajudar com isso" />
<SearchBox />
