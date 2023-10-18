<script>
	import Benefits from '../components/Benefits.svelte';
	import CallToAction from '../components/CallToAction.svelte';
	import Cards from '../components/Cards.svelte';
	import Footer from '../components/Footer.svelte';
	import Hero from '../components/Hero.svelte';
	import { NAME, DESCRIPTION } from '../constants';
</script>

<svelte:head>
	<title>{NAME}</title>
	<meta name="description" content={DESCRIPTION} />
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Roboto+Mono&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<Hero />

<Cards />

<Benefits />

<CallToAction />

<Footer />
