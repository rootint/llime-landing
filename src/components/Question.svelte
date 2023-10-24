<script>
	import chevron_down from '$lib/assets/chevron_down.svg';
	import chevron_up from '$lib/assets/chevron_up.svg';

	export let question;
	export let answer;

	let expanded = false;
	function toggleExpand() {
		expanded = !expanded;
	}
</script>

<div class="card-wrapper" on:click={toggleExpand} class:expanded>
	<div class="another-wrapper">
		<div class="card-inner">
			<div class="title-div">
				<h1 class="question">{question}</h1>
				<img src={!expanded ? chevron_down : chevron_up} width="24" height="24" alt="chevron" />
			</div>
			{#if expanded}
				<p class="answer">
					{answer}
				</p>
			{/if}
		</div>
	</div>
</div>

<style>
	p.answer {
		font-size: 1rem;
		font-weight: 400;
		margin: 0;
        margin-top: 20px;
		padding: 0;
		line-height: 140%;
	}
	img {
		margin: 0;
		/* background-color: #222; */
		padding: 4px;
		border-radius: 8px;
	}
	.title-div {
		display: flex;
		justify-content: space-between;
		align-items: top;
	}
	h1.question {
		font-size: 1.25rem;
		font-weight: 400;
		margin: 0;
	}
	@media (max-width: 768px) {
		h1.question {
			font-size: 1rem;
			font-weight: 400;
		}
	}
	.card-wrapper {
		padding: 1px;
		background: linear-gradient(91deg, rgb(69, 74, 222, 0.5) 13.45%, rgb(84, 173, 228, 0.5) 68.67%);
		border-radius: 8px;
		flex: 1;
		margin-bottom: 24px;
		/* box-shadow: 0 0 16px rgba(84, 173, 228, 0.25); */
		cursor: pointer;
		/* width: 100%; */
		justify-content: center;
		align-items: center;
		max-width: 70%;
		margin: 0 auto 32px;
		/* max-height: 96px; */
	}
	@media (max-width: 768px) {
		.card-wrapper {
			max-width: 100%;
		}
	}
	.card-inner {
		padding: 20px;
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
