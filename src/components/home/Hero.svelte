<script>
    export let img = "heroImg.svg";
    export let title = "Vinicius Henrique";
    export let subTitle =
        "Desenvolvedor web. Sites, dashboards, aplicativos e jogos";
</script>

<section class="hero">
    <div class="hero-image">
        <div class="container">
            <div data-aos="fade-down" data-aos-delay="100" class="over">
                <div class="row">
                    <div data-aos="fade-right" data-aos-delay="300" class="col-lg-6 col-sm-12 over-grid">
                        <h1><span>{title}</span></h1>
                        <span class="des">{subTitle}</span>
                    </div>
                    <div data-aos="fade-left" data-aos-delay="300" class="col-lg-6 col-sm-12">
                        <img src={img} alt="" />
                    </div>
                </div>
            </div>
            <div data-aos="fade-up" data-aos-delay="400">
                <a class="hero-button" href="#about">Saiba mais</a>
            </div>
        </div>
    </div>
</section>

<!-- <div class="gradient" style="height: 100vh" />
<div class="text">
    <div
        style="min-height:40vh"
        class=" container d-flex h-100 align-items-center"
    >
        <div data-aos="fade-in" data-aos-delay="100" class="text-white">
            <h1 class="my-0">{title}</h1>
            <h2
                style="font-size:20px"
                class="text-gradient text-dark-50 mx-auto mt-2 mb-5"
            >
                {subTitle}
            </h2>
            {#if showButton}
                <div data-aos="fade-in" data-aos-delay="300">
                    <a class="btn btn-primary js-scroll-trigger" href="#about"
                        >Saber mais</a
                    >
                </div>
            {/if}
        </div>
        <img src={img} width="600" alt="secure" />
    </div>
</div><style>
    .text {
        background-color: rgb(0, 0, 0); /* Fallback color */
        background-color: rgba(0, 0, 0, 0.4); /* Black w/opacity/see-through */
        color: white;
        font-weight: bold;
        border: 3px solid #f1f1f1;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        z-index: 2;
        width: 80%;
        padding: 20px;
        text-align: center;
    }
</style>-->
