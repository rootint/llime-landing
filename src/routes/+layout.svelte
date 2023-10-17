<script>
	import Header from '../components/Header.svelte';
	import { NAME } from '../constants';
	import './styles.css';
</script>

<div class="app">
	<Header />
	<main>
		<slot />
	</main>
</div>
