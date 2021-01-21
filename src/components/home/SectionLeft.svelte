<script>
    import { wpLink } from "../../config";

    export let img = "img/mulaPreta.png";
    export let title = "Fully Responsive Design";
    export let subTitle =
        "Everything an account has, except what it doesn't need.";
    export let effectType = "left";
    export let showButton = true;
    export let hasSelo = false;
    export let imgSide = "right";
    export let link = "#";
</script>

<div class="row px-0 mx-0 tamanho">
    {#if imgSide == "right"}
        <div class="col-lg-6 text-position px-0 mx-0">
            <div
                data-aos={`fade-${effectType}`}
                data-aos-delay="100"
                class="px-0 mx-0"
            >
                {#if link == "#"}
                    <h2>{title}</h2>
                {:else}
                    <h2>
                        <a style="color:black" href={link} target="_blanck"
                            >{title}</a
                        >
                    </h2>
                {/if}
                <h2 class="lead mb-0">{subTitle}</h2>
                {#if showButton}
                    <div
                        data-aos="fade-left"
                        data-aos-delay="100"
                        class="mt-2 p-0"
                    >
                        <a
                            style="text-decoration:none "
                            class="mx-0"
                            target="_blank"
                            href={wpLink}
                            >Entre em contado
                            <i class="fab fa-whatsapp" /></a
                        >
                    </div>
                {/if}
            </div>
        </div>
        <div class=" wobble-hor-bottom col-lg-6 px-0 mx-0">
            <img src={img} alt="Mula Preta Dashboard/Site" />
            {#if hasSelo}<img class="selo" src="img/selo.png" alt="selo" />{/if}
        </div>
    {:else if imgSide == "left"}
        <div class=" wobble-hor-bottom col-lg-6 px-0 mx-0">
            <img src={img} alt="Mula Preta Dashboard/Site" />
            {#if hasSelo}<img class="selo" src="img/selo.png" alt="selo" />{/if}
        </div>
        <div class="col-lg-6 text-position px-0 mx-0">
            <div
                data-aos={`fade-${effectType}`}
                data-aos-delay="100"
                class="px-0 mx-0"
            >
                {#if link == "#"}
                    <h2>{title}</h2>
                {:else}
                    <h2>
                        <a style="color:black" href={link} target="_blanck"
                            >{title}</a
                        >
                    </h2>
                {/if}
                <h2 class="lead mb-0">{subTitle}</h2>
                {#if showButton}
                    <div
                        data-aos="fade-left"
                        data-aos-delay="100"
                        class="mt-2 p-0"
                    >
                        <a
                            style="text-decoration:none "
                            class="mx-0"
                            target="_blank"
                            href={wpLink}
                            >Entre em contado
                            <i class="fab fa-whatsapp" /></a
                        >
                    </div>
                {/if}
            </div>
        </div>
    {/if}
</div>

<style>
    .text-position {
        display: grid;
        align-items: center;
    }
    img {
        max-width: 100%;
    }
    .tamanho{
        width: 100%;
    }
</style>
