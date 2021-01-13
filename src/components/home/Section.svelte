<script>
    import { wpLink } from "../../config";

    export let img = "img/mulaPreta.png";
    export let title = "Fully Responsive Design";
    export let subTitle =
        "Everything an account has, except what it doesn't need.";
    export let effectType = "left";
    export let showButton = true;
    export let hasSelo = false;
    export let imgSide = 'right'
    export let link = "#"
</script>

<style>
    section {
        display: grid;
        align-items: center;
        height: 60vh;
    }
    .text-position {
        display:grid;
        align-items: center;
    }
    img {
        max-width: 100%;
    }
    .selo {
        width: 80px;
        position: absolute;
        top: 13%;
        left: 73%;
    }
    a{
        text-decoration: none;
    }
</style>

{#if imgSide=="right"}
<section>
    <div class="row">
        <div class="col-lg-6 text-position">
            <div
                data-aos={`fade-${effectType}`}
                data-aos-delay="100"
                class="px-5 mx-5">
                <h2><a style="color:black" href="{link}" target="_blanck">{title}</a></h2>
                <h2 class="lead mb-0">{subTitle}</h2>
                {#if showButton}
                    <div
                        data-aos="fade-left"
                        data-aos-delay="100"
                        class="mt-2 p-0">
                        <a
                            style="text-decoration:none "
                            class="mx-0"
                            target="_blank"
                            href={wpLink}>Entre em contado
                            <i class="fab fa-whatsapp" /></a>
                    </div>
                {/if}
            </div>
        </div>
        <div class=" wobble-hor-bottom col-lg-6">
            <img src={img} alt="Mula Preta Dashboard/Site" />
            {#if hasSelo}<img class="selo" src="img/selo.png" alt="selo" />{/if}
        </div>
    </div>
</section>
{:else if imgSide=="left"}

<section>
    <div class="row">
        <div class=" wobble-hor-bottom col-lg-6">
            <img src={img} alt="Mula Preta Dashboard/Site" />
            {#if hasSelo}<img class="selo" src="img/selo.png" alt="selo" />{/if}
        </div>
        <div class="col-lg-6 text-position">
            <div
                data-aos={`fade-${effectType}`}
                data-aos-delay="100"
                class="px-5">
                <h2><a style="color:black" href="{link}" target="_blanck">{title}</a></h2>
                <h2 class="lead mb-0">{subTitle}</h2>
                {#if showButton}
                    <div
                        data-aos="fade-left"
                        data-aos-delay="100"
                        class="mt-2 p-0">
                        <a
                            style="text-decoration:none "
                            class="mx-0"
                            target="_blank"
                            href={wpLink}>Entre em contado
                            <i class="fab fa-whatsapp" /></a>
                    </div>
                {/if}
            </div>
        </div>
    </div>
</section>
{/if}
