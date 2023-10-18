<script>
	import { NAME } from '../constants';
</script>

<header>
	<nav>
		<div class="top-row">
			<img src="favicon.png" height="24" width="24" alt="logo" />
			<div style="width: 12px" />
			<p>{NAME}</p>
		</div>
		<div class="top-row">
			<div class="hide-on-mobile">
				<p>Home</p>
				<div style="width: 3rem" />
				<p>Pricing</p>
				<div style="width: 3rem" />
			</div>
			<div class="gradient-wrapper">
				<a class="header-button" href="#top">Get Started</a>
			</div>
		</div>
	</nav>
</header>

<style>
	.hide-on-mobile {
		display: flex;
		align-items: center;
	}
	@media (max-width: 768px) {
		.hide-on-mobile {
			display: none;
		}
	}
	nav {
		color: #fff;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin: 0 0;
		padding-top: 0px;
	}

	@media (max-width: 768px) {
		nav {
			color: #fff;
			display: flex;
			justify-content: space-between;
			align-items: center;
			margin: 0 0;
			padding-top: 0px;
		}
	}

	.top-row {
		display: flex;
		align-items: center;
	}

	p {
		font-weight: 500;
		font-size: 1rem;
	}

	.gradient-wrapper {
		padding: calc(0.66rem + 1px) 1px;
		/* max-width: calc(25rem + 4px); */
		background: linear-gradient(91deg, rgb(69, 74, 222, 0.5) 13.45%, rgb(84, 173, 228, 0.5) 68.67%);
		border-radius: 8px;
		/* margin-right: 1.5rem; */
	}
	.header-button {
		padding: 0.66rem 1.8rem;
        /* background-color: var(--background-color); */
        background-color: #111;
        /* background-color: white; */
		/* background: linear-gradient(92deg, #454ade 0.43%, #54ade4 124.53%); */
		font-weight: 500;
		font-size: 1rem;
		text-decoration: none;
		color: #fff;
		border: none;
		border-radius: 8px;
		cursor: pointer;
	}
</style>
