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
			<button class="header-button">Get Started</button>
		</div>
		<!-- <a class="button-nav" href="https://forms.gle/UBCinUCT8mbeWmwr6">Request A Demo</a> -->
	</nav>
</header>

<style>
	.hide-on-mobile {
		display: flex;
		align-items: center;
	}
	nav {
		color: #fff;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin: 0 0;
		padding-top: 16px;
	}

	.top-row {
		display: flex;
		align-items: center;
	}

	p {
		font-weight: 500;
		font-size: 1rem;
	}

	.header-button {
		padding: 0.66rem 1.8rem;
		background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
		font-weight: 500;
		font-size: 1rem;
		color: #fff;
		border: none;
		border-radius: 8px;
		cursor: pointer;
	}
</style>
