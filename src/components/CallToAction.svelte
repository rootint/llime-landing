<script>
	import EmailButton from './EmailButton.svelte';
</script>

<div class="background" />
<section class="cta">
	<h1 class="title">Unleash Your Team's Potential with LLime</h1>
	<h2 class="subtitle">Boost productivity across all departments.</h2>
	<EmailButton />
	<div style="height: 2rem" />
</section>

<style>
	h1.title {
		text-align: center;
		font-size: 3.75rem;
		margin: 32px 0;
		margin-top: 64px;
		max-width: 40rem;
	}
	@media (max-width: 768px) {
		h1.title {
			font-size: 3rem;
			font-weight: 500;
		}
	}
	h2.subtitle {
		font-size: 1.5rem;
		font-style: normal;
		font-weight: 400;
		margin: 0;
		margin-bottom: 48px;
        text-align: center;
	}
	@media (max-width: 768px) {
		h2.subtitle {
			color: rgba(255, 255, 255, 0.85);
			font-size: 1.25rem;
			font-style: normal;
			font-weight: 400;
            text-align: center;
		}
	}
	section.cta {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin: 0;
		width: 100%;
	}
	.background {
		background: linear-gradient(
			180deg,
			#0c0c0c 3.24%,
			#060723 48.68%,
			#0c0c0c 91.36%,
			#0c0c0c 91.37%
		);
		bottom: 0;
		position: absolute;
		width: 100%;
		z-index: -2;
	}
</style>
