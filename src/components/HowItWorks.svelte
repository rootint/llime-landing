<script>
	import developer from '$lib/assets/developer.webp';
	import data from '$lib/assets/data.png';
	import manager from '$lib/assets/manager.webp';
	import marketer from '$lib/assets/marketer.webp';
</script>

<div class="title">
	<h1 class="heading">Our process, your solution</h1>
	<h2 class="subheading">
		Delve into the steps we undertake to transform your data into actionable insights.
	</h2>
	<div style="height: 24px" />
	<div class="section">
		<div class="text">
			<p class="monospace">Step 1</p>
			<h1 class="section-heading">Data Collection</h1>
			<p class="text">
				Begin by sharing your data, whether from GitHub, Notion, Google Docs, CRM CSVs, or other
				sources. Outline your specific needs, such as business counts or departments. We prioritize
				understanding your business intimately, ensuring our collaboration yields the best results.
			</p>
		</div>
		<div style="width: 32px" />
		<img src={data} alt="data-arrow" />
	</div>
	<div class="section-second">
		<img src={manager} alt="manager-chat-example" />
		<div style="width: 32px" />
		<div class="text">
			<p class="monospace">Step 2</p>
			<h1 class="section-heading">Model Creation</h1>
			<p class="text">
				Harness the power of LLMs to streamline decision-making and gain deep insights into
				financial reports and resource allocation. Optimize team coordination, enhance employee
				performance, and ensure every decision aligns with the company's objectives.
			</p>
		</div>
	</div>
	<div class="section">
		<div class="text">
			<p class="monospace">Step 3</p>
			<h1 class="section-heading">Product Build</h1>
			<p class="text">
				LLime empowers marketers with instant access to campaign data, audience insights, and
				content strategies. Improve campaign efficiency, tailor content to your target audience, and
				make data-driven decisions effortlessly.
			</p>
		</div>
		<div style="width: 32px" />
		<img src={marketer} alt="marketer-chat-example" />
	</div>
	<div class="section-second">
		<img src={manager} alt="manager-chat-example" />
		<div style="width: 32px" />
		<div class="text">
			<p class="monospace">Step 4</p>
			<h1 class="section-heading">Continuous Feedback</h1>
			<p class="text">
				Harness the power of LLMs to streamline decision-making and gain deep insights into
				financial reports and resource allocation. Optimize team coordination, enhance employee
				performance, and ensure every decision aligns with the company's objectives.
			</p>
		</div>
	</div>
</div>

<style>
	p.monospace {
		font-family: 'Roboto Mono', sans-serif;
		margin: 0;
		margin-bottom: 8px;
		color: rgba(255, 255, 255, 0.75);
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
		width: 100%;
		max-width: 50%;
		height: auto;
		flex: 1;
		align-self: start;
		/* margin: 0;
		padding: 0;
		height: auto;
        max-width: 50%;
        width: 100%; */
		/* max-width: none;
		align-self: center;
		flex-shrink: 0; */
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
		margin-bottom: 32px;
	}
	@media (max-width: 768px) {
		.section {
			display: flex;
			flex-direction: column;
			margin-bottom: 24px;
		}
	}
	.section-second {
		display: flex;
		margin: 0;
		margin-bottom: 32px;
		text-align: right;
	}
	@media (max-width: 768px) {
		.section-second {
			display: flex;
			margin: 0;
			flex-direction: column-reverse;
			margin-bottom: 24px;
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
