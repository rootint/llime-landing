<script>
	import { NAME } from '../constants';
	import linkedin from '$lib/assets/linkedin.svg';
	import twitter from '$lib/assets/twitter.svg';
	import discord from '$lib/assets/discord.svg';
</script>

<footer>
	<div class="top-row">
		<img src="favicon.png" height="24" width="24" alt="logo" />
		<div style="width: 12px" />
		<p>{NAME}</p>
	</div>
	<div class="top-row">
		<a href="https://www.linkedin.com/company/llime">
			<img src={linkedin} width="24" height="24" class="icons" alt="LinkedIn Logo" /></a
		>
		<a href="https://twitter.com/LLIMe_AI"
			><img src={twitter} width="24" height="24" class="icons" alt="Twitter Logo" /></a
		>
		<a href="https://discord.gg/ZdeCBkG3Uj">
			<img src={discord} width="24" height="24" alt="Discord Logo" /></a
		>
	</div>  
</footer>

<style>
	img.icons {
		margin-right: 32px;
	}
	.top-row {
		display: flex;
		align-items: center;
	}
	footer {
		display: flex;
		margin-top: 5rem;
		justify-content: space-between;
	}
</style>
