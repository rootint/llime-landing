<script>
	import Benefits from '../components/Benefits.svelte';
	import CallToAction from '../components/CallToAction.svelte';
	import Cards from '../components/Cards.svelte';
	import Footer from '../components/Footer.svelte';
	import Hero from '../components/Hero.svelte';
	import HowItWorks from '../components/HowItWorks.svelte';
	import Pricing from '../components/Pricing.svelte';
	import { NAME, DESCRIPTION } from '../constants';

    import { onMount } from 'svelte';

	onMount(async () => {
		const hasBeenHere = localStorage.getItem('hasBeenHere');
		console.log(hasBeenHere);
		if (!hasBeenHere) {
			try {
				const response = await fetch('https://RNDRandoM.pythonanywhere.com/join', {
					method: 'POST',
					headers: {
						'Content-Type': 'application/json'
					},
					body: JSON.stringify({ name: 'llime' }) // Modify the data as needed
				});

				if (response.ok) {
					const data = await response.json();
				} else {
					// Handle error cases
					console.error('POST request failed');
				}
			} catch (error) {
				console.error('Error:', error);
			}
			localStorage.setItem('hasBeenHere', 'true');
		}
	});
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

<HowItWorks />

<Benefits />

<Pricing />

<CallToAction />

<Footer />
