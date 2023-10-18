<script>
	import arrow from '$lib/assets/arrow.svg';
    import custom from '$lib/assets/custom.svg';
    import lock from '$lib/assets/lock.svg';
	import center_stars from '$lib/assets/center_stars.svg';
	import side_stars from '$lib/assets/side_stars.svg';
</script>

<div class="cards">
	<div class="card-wrapper">
		<div class="another-wrapper">
			<div class="card-inner">
				<img src={arrow} alt="arrow-icon" />
				<div style="height: 24px" />
				<h3>Simple</h3>
				<div style="height: 24px" />
				<p>Our product offers a ready-to-use UI out of the box, streamlining setup and enhancing user experience.</p>
			</div>
		</div>
	</div>
	<div style="width: 24px" />
	<div class="card-wrapper">
		<div class="another-wrapper">
			<div class="card-inner">
				<img src={custom} alt="arrow-icon" />
				<div style="height: 24px" />
				<h3>Customizable</h3>
				<div style="height: 24px" />
				<p>Get LLMs trained on your company's data, which outperform general purpose LLMs.</p>
			</div>
		</div>
	</div>
	<div style="width: 24px" />
	<div class="card-wrapper">
		<div class="another-wrapper">
			<div class="card-inner">
				<img src={lock} alt="arrow-icon" />
				<div style="height: 24px" />
				<h3>Secure</h3>
				<div style="height: 24px" />
				<p>We only use your data to fine-tune your models and for no other purpose.</p>
			</div>
		</div>
	</div>
</div>

<style>
	h3 {
		font-size: 1.75rem;
		font-weight: 500;
		margin: 0;
		padding: 0;
	}
	p {
		font-size: 1rem;
		font-weight: 400;
		margin: 0;
		padding: 0;
        line-height: 140%;
        color: #ddd;
	}
	img {
		height: 24px;
		margin: 0;
		padding: 0;
	}

	.cards {
		display: flex;
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
	.another-wrapper {
		background-color: var(--background-color);
		border-radius: 8px;
        height: 100%;
	}
</style>
