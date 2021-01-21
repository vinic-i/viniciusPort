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

<section class="text-center" id="about">
	<div class="containear text-center">
		<div data-aos="fade-up" data-aos-delay="100" class="mb-5">
			<h1>Sobre mim</h1>
		</div>
		<div data-aos="fade-up" data-aos-delay="100" class="about-text">
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
	<div class="container">
		<div data-aos="flip-left" data-aos-delay="100" class="my-5 text-center">
			<h1>Projetos</h1>
		</div>
		<!-- PRIMEIRA LINHA -->
		<div class="row p-0 mb-5 mx-0">
			<div data-aos="fade-left" data-aos-delay="100" class="text-size  col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<h2 class="text-content">
					<a
						style="color:black"
						href="https://kiromass.netlify.app/"
						target="_blanck">{sec1Title}</a
					>
					<p style="font-size: 1.2rem">{sec1SubTitle}</p>
					<div data-aos="fade-left" data-aos-delay="100">
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
			<div data-aos="flip-left" data-aos-delay="100" class="col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<img src="img/kiroMass3.jpg" alt="Mula Preta Dashboard/Site" />
			</div>
		</div>
		<!-- SEGUNDA LINHA -->
		<div class="row p-0 mb-5 mx-0">
			<div data-aos="fade-left" data-aos-delay="100" class="text-size  col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<h2 class="text-content">
					<a style="color:black" href="https://mulapreta.com/" target="_blanck"
						>{sec2Title}</a
					>
					<p style="font-size: 1.2rem">{sec2SubTitle}</p>
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
			<div data-aos="flip-left" data-aos-delay="100" class="col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<img src="img/mulaPreta.png" alt="Mula Preta Dashboard/Site" />
			</div>
		</div>
		<!-- TERCEIRA LINHA -->
		<div class="row p-0 mb-5 mx-0">
			<div data-aos="fade-left" data-aos-delay="100" class="text-size  col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<h2 class="text-content">
					<a
						style="color:black"
						href="https://portaldigitalmusic.netlify.app/"
						target="_blanck">{sec3Title}</a
					>
					<p style="font-size: 1.2rem">{sec3SubTitle}</p>
					<div data-aos="fade-left" data-aos-delay="100">
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
			<div data-aos="flip-left" data-aos-delay="100" class="col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<img
					src="DigitalMusic/LoginDM.png"
					alt="Mula Preta Dashboard/Site"
				/>
			</div>
		</div>
		<!-- QUARTA LINHA -->
		<div class="row p-0 mb-5 mx-0">
			<div data-aos="fade-left" data-aos-delay="100" class="text-size  col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<h2 class="text-content">
					<a
						style="color:black"
						href="DigitalMusic/LoginDM.png"
						target="_blanck">{sec4Title}</a
					>
					<p style="font-size: 1.2rem">{sec4SubTitle}</p>
					<div data-aos="fade-left" data-aos-delay="100">
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
			<div data-aos="flip-left" data-aos-delay="100" class="col-lg-6 col-sm-12 col-md-12 p-0 m-0">
				<img src="unity.png" alt="Mula Preta Dashboard/Site" />
			</div>
		</div>
	</div>
</section>

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
<section id="features">
	<LogoShowCase />
</section>

<style>
	.containear {
		display: grid;
		align-content: center;
		justify-content: center;
		background-image: url("footer.png");
		height: 80vh;
	}
	.about-text {
		width: 600px;
	}
	@media only screen and (max-width: 600px) {
		.about-text {
			width: 400px;
		}
	}

	.containear p {
		text-align: justify;
		font-size: 25px;
	}
	img {
		width: 100%;
	}
	.contato {
		font-size: 1rem;
		margin: 0;
		padding: 0;
	}
	 .text-size {
        display: grid;
    align-items: center;

	}
	.text-content {
		padding: 0 10px 0 10px;
	}
</style>
