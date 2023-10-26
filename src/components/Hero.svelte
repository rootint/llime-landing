<script>
	import EmailButton from './EmailButton.svelte';
	import example from '$lib/assets/example.png';
	import stars from '$lib/assets/stars.svg';
</script>

<div class="background" />
<!-- <div class="stars" /> -->
<section class="hero" style="background-image: url({stars});">
	<div class="top-padding" />
	<h1 class="hero">
		<span class="supercharge">Supercharge</span>
		your business with LLMs
	</h1>
	<div style="height: 2.5rem;" />
	<h2 class="hero">
		Intuitive and secure custom AI assistants for every department in your enterprise.
	</h2>
	<div style="height: 3.5rem;" />
	<EmailButton />
	<div style="height: 4rem;" />
	<a
		href="https://www.producthunt.com/products/llime?utm_source=badge-follow&utm_medium=badge&utm_souce=badge-llime"
		target="_blank"
		><img
			src="https://api.producthunt.com/widgets/embed-image/v1/follow.svg?product_id=557249&theme=dark"
			alt="LLime - Supercharge&#0032;your&#0032;business&#0032;with&#0032;LLMs | Product Hunt"
			style="width: 250px; height: 54px;"
			width="250"
			height="54"
		/></a
	>
	<div class="image-wrapper">
		<img src={example} alt="UI example" />
	</div>
	<div style="height: 4rem;" />
</section>

<style>
	@keyframes fadeIn {
		from {
			opacity: 0;
		}
		to {
			opacity: 1;
		}
	}
	.background {
		background: linear-gradient(
			180deg,
			#0c0c0c 3.24%,
			#060723 48.68%,
			#0c0c0c 91.36%,
			#0c0c0c 91.37%
		);
		left: 0;
		top: 0;
		position: fixed;
		width: 100%;
		height: 80%;
		z-index: -2;
	}
	img {
		width: 100%;
		margin: 0;
		padding: 0;
		border-radius: 8px;
		display: block;
	}

	.image-wrapper {
		padding: 1px;
		background: linear-gradient(91deg, rgb(69, 74, 222, 1) 13.45%, rgb(84, 173, 228, 1) 68.67%);
		border-radius: 8px;
		margin: 0;
		margin-top: 4rem;
		box-shadow: 0 0 16px rgba(84, 173, 228, 0.25);
		animation: fadeIn 1s ease-out forwards;
	}

	.top-padding {
		height: 8rem;
	}
	@media (max-width: 768px) {
		.top-padding {
			height: 4rem;
		}
	}
	.supercharge {
		background: linear-gradient(91deg, var(--primary-color) 13.45%, var(--secondary-color) 68.67%);
		background-clip: text;
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}
	section.hero {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin: 0;
		width: 100%;
		background-repeat: no-repeat;
	}
	h1.hero,
	h2.hero {
		text-align: center;
		margin: 0;
		padding: 0;
		max-width: 45rem;
	}
	h2.hero {
		max-width: 35rem;
	}
</style>
