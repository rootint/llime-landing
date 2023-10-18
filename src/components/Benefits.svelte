<script>
	import developer from '$lib/assets/developer.png';
	import manager from '$lib/assets/manager.png';
	import marketer from '$lib/assets/marketer.png';
</script>

<div class="title">
	<h1 class="heading">Maximize your team's impact</h1>
	<h2 class="subheading">Shape workflows effortlessly with custom LLM capabilities.</h2>
	<div style="height: 24px" />
	<div class="section">
		<div class="text">
			<p class="monospace">Developers</p>
			<h1 class="section-heading">Intuitive Development</h1>
			<p class="text">
				LLime offers an in-depth exploration of your company's code and tech docs, providing
				developers with clear insights. This not only elevates coding efficiency but also becomes an
				invaluable tool for seamless onboarding of new team members.
			</p>
		</div>
		<div style="width: 32px" />
		<img src={developer} alt="developer-chat-example" />
	</div>
	<div class="section-second">
		<img src={manager} alt="manager-chat-example" />
		<div style="width: 32px" />
		<div class="text">
			<p class="monospace">Managers</p>
			<h1 class="section-heading">Strategic Excellence</h1>
			<p class="text">
				Harness the power of LLMs to streamline decision-making and gain deep insights into
				financial reports and resource allocation. Optimize team coordination, enhance employee
				performance, and ensure every decision aligns with the company's objectives.
			</p>
		</div>
	</div>
	<div class="section-last">
		<div class="text">
			<p class="monospace">Marketers</p>
			<h1 class="section-heading">Dynamic Engagement</h1>
			<p class="text">
				LLime empowers marketers with instant access to campaign data, audience insights, and
				content strategies. Improve campaign efficiency, tailor content to your target audience, and
				make data-driven decisions effortlessly.
			</p>
		</div>
		<div style="width: 32px" />
		<img src={marketer} alt="marketer-chat-example" />
	</div>
</div>

<style>
	p.monospace {
		font-family: 'Roboto Mono', sans-serif;
		margin: 0;
		margin-bottom: 8px;
		color: rgba(255, 255, 255, 0.66);
	}
	h1.section-heading {
		font-size: 2rem;
		font-weight: 500;
		margin: 0;
		margin-bottom: 24px;
	}

	p.text {
		max-width: 90%;
		font-size: 1rem;
		margin: 0;
		line-height: 140%;
	}
	@media (max-width: 768px) {
		p.text {
			font-size: 1rem;
			margin: 0;
			line-height: 140%;
			margin-bottom: 24px;
		}
	}

	.text {
		margin: 0;
		padding: 0;
		flex: 1;
		text-align: left;
	}
	img {
		margin: 0;
		padding: 0;
		flex: 1;
		max-width: 50%;
	}
	@media (max-width: 768px) {
		img {
			margin: 0;
			padding: 0;
			width: 100%;
			max-width: 100%;
			margin-bottom: 32px;
		}
	}
	.section {
		display: flex;
		margin: 0;
		margin-bottom: 240px;
	}
	@media (max-width: 768px) {
		.section {
			display: flex;
			flex-direction: column;
			margin-bottom: 48px;
		}
	}
	.section-second {
		display: flex;
		margin: 0;
		margin-bottom: 240px;
	}
	@media (max-width: 768px) {
		.section-second {
			display: flex;
			margin: 0;
			flex-direction: column-reverse;
            margin-bottom: 48px;
		}
	}
	.section-last {
		display: flex;
		margin: 0;
		margin-bottom: 64px;
	}
	@media (max-width: 768px) {
		.section-last {
			display: flex;
            flex-direction: column;
			margin: 0;
            margin-bottom: 64px;
		}
	}
	h1.heading {
		font-size: 2.25rem;
		font-weight: 500;
		margin: 16px 0px;
	}
	h2.subheading {
		font-size: 1rem;
		font-weight: 300;
		margin: 0;
		margin-bottom: 36px;
		color: rgba(255, 255, 255, 0.9);
	}
	h2.last-heading {
		font-size: 1rem;
		font-weight: 400;
		margin: 0;
		color: rgba(255, 255, 255, 0.9);
	}
	.title {
		display: flex;
		flex-direction: column;
		align-content: center;
		text-align: center;
	}

	@media (max-width: 768px) {
		.title {
			display: flex;
			flex-direction: column;
			align-content: center;
			text-align: left;
		}
	}
</style>
