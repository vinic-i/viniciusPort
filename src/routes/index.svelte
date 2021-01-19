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
		LogoShowCase,
		OurProjects,
		Section,
	} from "../components";
	import { wpLink } from "../config";

	let sec1Title = "Site de apresentação do centro de massagem Kiro Mass ";
	let sec1SubTitle =
		"Nesse projeto, participei diretamento no front-end, em maior parte nas cores, design e imagens. Na criação desse projeto aprendi muito sobre gradient, css e animações";
	let sec2Title = "Site da Loja e Dashboard Mula Preta";
	let sec2SubTitle =
		"O site da Mula Preta foi feito com base em um design completo e minimalista. O dashboard + site da mula preta foi um dos maiores projetos em que já trabalhei, e devido a tantas funcionalidades do dashboard desenvolvi muito o trabalho com backend e javascript principalmente";

	let sec3Title = "Dashboard da escola de música DigitalMusic";
	let sec3SubTitle =
		"O dashboard da Digital Music vem trazendo diversas funcionalidades para automatizar a gestão de qualquer escola. A construção dessa aplicação está sendo muito divertida e estou aprendendo muito sobre banco de dados, em especial, o firebase";
	let sec4Title = "Jogo em desenvolvimento";
	let sec4SubTitle = "Nas horas vagas, gosto de criar jogos no unity";
</script>

<svelte:head>
	<title>Vinicius Portfólio</title>
</svelte:head>

<Hero />

<section class="text-center" id="about">
	<div class="containear text-center">
		<div class="mb-5">
			<h1>Sobre mim</h1>
		</div>
		<div class="about-text">
			<p>
				Olá, sou Vinicius, um estudante do 5º período de Ciências e
				Tecnologia pela Universidade Federal do Rio Grande do Norte, fã
				dos jogos e de tecnologia. Desde criança tenho muito interesse
				por computador, tanto hardware como software. Montei meu próprio
				computador e hoje trabalho nele programando sites e aplicações.
			</p>
		</div>
	</div>
</section>

<section id="projects">
	<div class="my-5 text-center">
		<h1>Projetos</h1>
	</div>
	<Section
		title={sec1Title}
		subTitle={sec1SubTitle}
		showButton={true}
		img="img/kiroMass3.jpg"
		link="https://kiromass.netlify.app/"
	/>
	<Section
		title={sec2Title}
		subTitle={sec2SubTitle}
		showButton={true}
		img="img/mulaPreta.png"
		link="https://mulapreta.com/"
	/>

	<Section
		title={sec3Title}
		subTitle={sec3SubTitle}
		showButton={true}
		img="DigitalMusic/LoginDM.png"
		link="https://portaldigitalmusic.netlify.app/"
	/>

	<Section
		title={sec4Title}
		subTitle={sec4SubTitle}
		showButton={true}
		img="unity.png"
			/> 
</section>
<section id="features">
	<LogoShowCase />
</section>
<style>
	.containear {
		display: grid;
		align-content: center;
		justify-content: center;
		background-image: url("footer.png");
		height: 60vh;
	}
	.about-text {
		width: 600px;
	}
	.containear p {
		text-align: justify;
		font-size: 25px;
	}
</style>
