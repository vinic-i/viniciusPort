<script>
    import { Card, ContainerFluid } from "../core";

    const cards = [
        {
            title: `Massagem Modeladora`,
            text: `A massagem modeladora possui a finalidade de definir as curvas do corpo reduzindo medidas através da eliminação de gordura localizada.`,
        },
        {
            title: `Drenagem Linfática`,
            text: `A drenagem linfática pode beneficiar a saúde e a beleza do corpo eliminando inchaço, toxinas e nódulos gordurosos.`,
        },
        {
            title: `Massagem Relaxante`,
            text: `Oferecemos tanto massagens relaxates direcionadas quanto de corpo inteiro`,
        },
        {
            title: `Massagem Facial`,
            text: `A massagem facial suavisa as linhas de expressões, diminuindo inchanço, relaxando os músculos e estimulando a circulação sanguínea do rosto.`,
        },
        {
            title: "Reflexologia Podal",
            text: `Conheça os resultados de uma pesquisa realizada com 43 pessoas com dores lombares que tiveram ótimos resultados após o tratamento com as pastilhas.`,
        },
        {
            title: "Ventosaterapia",
            text: `A ventosaterpia reduz dores de cabeça, dores nas costas e dores lombares, liberando a circulação nos tecidos musculares e melhorando a circulação sanguínea.`,
        },
    ];
</script>

<style>
    .grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        grid-gap: 2em;
    }
    .bg-img {
        position: relative;
        overflow: hidden;
    }
    .bg-img img {
        position: absolute;
        right: -50%;
        max-height: 100%;
    }

</style>

<div class="feature-section" id="features">
    <ContainerFluid style="" p="px-0" height="screen-height">
        <div class="bg-img" style="padding: 5rem 0;">
            <div class="container" data-aos="zoom-in" data-aos-delay="100">
                <h2 class="text-gradient mb-4 text-center">
                    Benefícios
                </h2>

                <div class="grid feature-section">
                    {#each cards as card, index}
                        <div
                            style="display: grid;"
                            on:mouseenter={() => {
                                cards[index].hover = true;
                            }}
                            on:mouseleave={() => {
                                cards[index].hover = false;
                            }}>
                            <Card
                                shadow={false}
                                animation="fade-in"
                                delay={(index+1) * 300}
                                className="p-4 py-5">

                                <h4 class="text-uppercase m-0">{card.title}</h4>
                                <hr class="my-4" />
                                <div class="small text-black-50">
                                    {card.text}
                                </div>
                            </Card>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </ContainerFluid>
</div>
