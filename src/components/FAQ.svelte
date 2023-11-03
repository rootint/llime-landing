<script>
	import Question from './Question.svelte';
</script>

<div style="height: 6rem" />
<h1 class="title">Frequently Asked Questions</h1>
<h2 class="subheading">If you have other questions, feel free to contact us at tioluwani@llime.co</h2>

<Question
	question="What are the benefits compared to using ChatGPT?"
	answer="Compared to ChatGPT, LLime offers tailored AI solutions specifically for businesses. While ChatGPT provides general-purpose interactions, LLime fine-tunes models with client data for enhanced relevancy. Additionally, LLime caters to various business departments, delivering a specialized experience for developers, managers, and marketers."
/>
<Question
	question="Who can use the product?"
	answer="
    LLime is designed for businesses aiming to enhance productivity through AI. Developers can streamline coding, managers can make informed decisions faster, and marketers can refine strategies effectively using LLime's specialized ChatGPT-like AI."
/>
<Question
	question="How is the data used?"
	answer="LLime uses your data only to fine-tune your AI models for better accuracy and does not use it for any other purpose."
/>

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
</style>
