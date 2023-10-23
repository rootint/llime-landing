<script>
	import check from '$lib/assets/check.svg';
</script>

<h1 class="title" id="pricing">Pricing</h1>
<h2 class="subheading">Pick the best plan for your team.</h2>
<div style="height: 24px" />
<div class="cards">
	<div class="card-wrapper">
		<div class="another-wrapper">
			<div class="card-inner">
				<h3>Standard</h3>
				<div style="height: 24px" />
				<h4>Limited-time Offer</h4>
				<div class="pricing-row">
					<p class="price">$1499</p>
					<div style="width: 8px" />
					<div class="subtitles">
						<p class="subtitle">per month</p>
						<p class="subtitle">billed annually</p>
					</div>
				</div>
				<div style="height: 8px" />
				<p class="title-grayed">Regular price</p>
				<p class="price-grayed">$2999</p>
				<ul>
					<li>3 departments</li>
					<li>15 employees / dept.</li>
					<li>1 admin</li>
					<li>LLaMa 7B</li>
					<li>Slowest servers</li>
				</ul>
			</div>
		</div>
	</div>
	<div style="width: 24px" />
	<div class="card-wrapper">
		<div class="another-wrapper">
			<div class="card-inner-center">
				<h3>Premium</h3>
				<div style="height: 24px" />
				<h4>Limited-time Offer</h4>
				<div class="pricing-row">
					<p class="price">$2499</p>
					<div style="width: 8px" />
					<div class="subtitles">
						<p class="subtitle">per month</p>
						<p class="subtitle">billed annually</p>
					</div>
				</div>
				<div style="height: 8px" />
				<p class="title-grayed">Regular price</p>
				<p class="price-grayed">$4999</p>
				<ul>
					<li>5 departments</li>
					<li>25 employees / dept.</li>
					<li>2 admins</li>
					<li>LLaMa 13B</li>
					<li>Fast servers</li>
				</ul>
			</div>
		</div>
	</div>
	<div style="width: 24px" />
	<div class="card-wrapper">
		<div class="another-wrapper">
			<div class="card-inner">
				<h3>Custom</h3>
				<div style="height: 24px" />
				<h3>Contact Sales</h3>
                <div style="height: 24px" />
				<ul>
					<li>Unlimited departments</li>
					<li>Unlimited employees / dept.</li>
					<li>Unlimited admins</li>
					<li>Best available models</li>
					<li>Fastest servers</li>
				</ul>
			</div>
		</div>
	</div>
</div>

<style>
	h1.title {
		text-align: center;
		font-size: 2.25rem;
		font-weight: 500;
		margin: 16px 0px;
		margin-top: 24px;
	}
	h2.subheading {
		text-align: center;
		font-size: 1rem;
		font-weight: 300;
		margin: 0;
		margin-bottom: 36px;
		color: rgba(255, 255, 255, 0.9);
	}
	ul {
		list-style-type: none; /* Remove default bullet points */
		padding: 0; /* Remove default padding */
		margin: 0;
		margin-top: 16px;
	}

	li {
		position: relative;
		padding-left: 24px;
		margin-bottom: 16px;
		font-size: 1rem;
	}
	li:last-child {
		margin-bottom: 6;
	}

	/* Pseudo-element for the checkmark */
	li::before {
		content: '✔';
		position: absolute;
		left: 0;
		top: 50%;
		transform: translateY(-50%); /* Center align vertically */
		font-size: 16px; /* Font size of the checkmark */
		color: var(--primary-color);
	}
	p.price-grayed {
		font-size: 2rem;
		color: rgba(255, 255, 255, 0.75);
	}
	p.title-grayed {
		font-size: 0.875rem;
		color: rgba(255, 255, 255, 0.75);
	}
	p.price {
		font-weight: 600;
		font-size: 2.5rem;
	}
	p.subtitle {
		color: rgba(255, 255, 255, 0.5);
		font-size: 0.875rem;
		font-weight: 300;
	}
	.subtitles {
		display: flex;
		flex-direction: column;
	}
	.pricing-row {
		display: flex;
		align-items: center;
	}

	h3 {
		font-size: 1.75rem;
		font-weight: 500;
		margin: 0;
		padding: 0;
	}
	h4 {
		font-size: 1rem;
		font-weight: 400;
		margin: 0;
		padding: 0;
	}
	p {
		font-size: 1rem;
		font-weight: 400;
		margin: 0;
		padding: 0;
		line-height: 140%;
	}
	.cards {
		display: flex;
		margin-bottom: 32px;
	}

	@media (max-width: 768px) {
		.cards {
			display: flex;
			flex-direction: column;
		}
	}

	.card-wrapper {
		padding: 1px;
		background: linear-gradient(91deg, rgb(69, 74, 222, 0.5) 13.45%, rgb(84, 173, 228, 0.5) 68.67%);
		border-radius: 8px;
		flex: 1;
		margin-bottom: 24px;
		box-shadow: 0 0 16px rgba(84, 173, 228, 0.25);
	}

	.card-inner {
		padding: 24px;
		display: block;
		border-radius: 8px;
		background: linear-gradient(
			180deg,
			rgba(69, 74, 222, 0.1) 0%,
			rgba(69, 74, 222, 0.07) 0.01%,
			rgba(84, 173, 228, 0.07) 97.47%
		);
		height: 100%;
	}

	.card-inner-center {
		padding: 24px;
		display: block;
		border-radius: 8px;
		background: linear-gradient(180deg, #454ade 0.02%, #454ade 0.04%, #54ade4 143.02%);

		height: 100%;
	}

	.another-wrapper {
		background-color: var(--background-color);
		border-radius: 8px;
		height: 100%;
	}
</style>
