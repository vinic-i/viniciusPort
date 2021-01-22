<script>
	import { Hero, LogoShowCase, Section } from "../components";
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

<div class="container">
	<section id="about" class="about-text text-center d-flex align-items-center">
		<div class="">
			<h1 class="mb-5" >SOBRE MIM</h1>

			<p style="font-size: 1.2rem">
				Olá, sou Vinicius, um estudante do 5º período de Ciências e
				Tecnologia pela Universidade Federal do Rio Grande do Norte, fã
				dos jogos e de tecnologia. Desde criança tenho muito interesse
				por computador, tanto hardware como software. Montei meu próprio
				computador e hoje trabalho nele programando sites e aplicações.
			</p>
		</div>
	</section>

	<div id="projects">
		<div class=" text-center">
			<h1>PROJETOS</h1>
		</div>
		<section class="row">
			<div
				class="text-size d-flex align-items-center col-sm-12 col-md-12 col-lg-6  p-0 m-0"
			>
				<h2 class="text-content">
					<a
						
						style="color:black"
						href="https://kiromass.netlify.app/"
						target="_blanck">{sec1Title}</a
					>
					<p class="my-3" style="font-size: 1.2rem">{sec1SubTitle}</p>
					<div>
						<a
							class="contato"
							style="text-decoration:none "
							target="_blank"
							href={wpLink}
							>Entre em contado
							<i class="fab fa-whatsapp" /></a
						>
					</div>
				</h2>
			</div>
			<div
				class="d-flex align-items-center col-sm-12 col-md-12 col-lg-6  p-0 m-0"
			>
				<img src="img/kiroMass3.jpg" alt="Mula Preta Dashboard/Site" />
			</div>
		</section>
		<section class="row">
			<div
				class="text-size d-flex align-items-center col-sm-12 col-md-12 col-lg-6  p-0 m-0"
			>
				<h2 class="text-content">
					<a
					
						style="color:black"
						href="https://mulapreta.com/"
						target="_blanck">{sec2Title}</a
					>
					<p class="mt-3" style="font-size: 1.2rem">{sec2SubTitle}</p>
					<a
						class="contato"
						style="text-decoration:none "
						target="_blank"
						href={wpLink}
						>Entre em contado
						<i class="fab fa-whatsapp" /></a
					>
				</h2>
			</div>
			<div
				class="col-sm-12 d-flex align-items-center col-md-12 col-lg-6  p-0 m-0"
			>
				<img src="img/mulaPreta.png" alt="Mula Preta Dashboard/Site" />
			</div>
		</section>
		<section class="row p-0 mb-5 mx-0">
			<div
				class="text-size d-flex align-items-center col-sm-12 col-md-12 col-lg-6  p-0 m-0"
			>
				<h2 class="text-content">
					<a
					
						style="color:black"
						href="https://portaldigitalmusic.netlify.app/"
						target="_blanck">{sec3Title}</a
					>
					<p class="mt-3" style="font-size: 1.2rem">{sec3SubTitle}</p>
					<div>
						<a
							class="contato"
							style="text-decoration:none "
							target="_blank"
							href={wpLink}
							>Entre em contado
							<i class="fab fa-whatsapp" /></a
						>
					</div>
				</h2>
			</div>
			<div
				class="d-flex align-items-center col-sm-12 col-md-12 col-lg-6 d-flex align-items-center p-0 m-0"
			>
				<img
					src="DigitalMusic/LoginDM.png"
					alt="Mula Preta Dashboard/Site"
				/>
			</div>
		</section>
		<section class="row">
			<div
				class="text-size d-flex align-items-center col-sm-12 col-md-12 col-lg-6  p-0 m-0"
			>
				<h2 class="text-content">
					<a
					
						style="color:black"
						href="DigitalMusic/LoginDM.png"
						target="_blanck">{sec4Title}</a
					>
					<p class="mt-3" style="font-size: 1.2rem">{sec4SubTitle}</p>
					<div>
						<a
							class="contato"
							style="text-decoration:none "
							target="_blank"
							href={wpLink}
							>Entre em contado
							<i class="fab fa-whatsapp" /></a
						>
					</div>
				</h2>
			</div>
			<div
				class="d-flex align-items-center col-sm-12 col-md-12 col-lg-6  p-0 m-0"
			>
				<img src="unity.png" alt="Mula Preta Dashboard/Site" />
			</div>
		</section>
	</div>

	<!-- <section id="projects">
	<div class="container">
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
	</div>
</section> -->
</div>
<section id="features">
	<LogoShowCase />
</section>

<style>
	section {
		min-height: 80vh;
	}

	img {
		width: 100%;
	}
	.contato {
		font-size: 1rem;
		margin: 0;
		padding: 0;
	}

	.text-content {
		padding: 0 10px 0 10px;
	}

	@media (min-width: 600px) {
		.about-text {
			max-width: 50em;
			margin: auto;
		}
	}
</style>
