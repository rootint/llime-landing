<script>
	let email = '';
	let isEmailValid = false;
	let buttonText = 'Get Started';

	const handleSubmit = async () => {
		try {
			buttonText = 'Loading...';
			const response = await fetch('https://RNDRandoM.pythonanywhere.com/submit', {
				method: 'POST',
				headers: {
					'Content-Type': 'application/json'
				},
				body: JSON.stringify({ name: 'llime', email: email }) // Modify the data as needed
			});
			if (response.ok) {
				const data = await response.json();
				console.log(data);
				email = '';
				// isPopupVisible = true;
				isEmailValid = false;
				buttonText = 'Get Started';
				alert('Your email was sent successfully! We will contact you soon.');
			} else {
				// Handle error cases
				console.error('POST request failed');
				buttonText = 'Get Started';
				isEmailValid = false;
				alert("Can't send the email, please try again later.");
			}
		} catch (error) {
			console.error('Error:', error);
		}
	};

	// Function to validate the email input
	function validateEmail() {
		const emailRegex = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;
		isEmailValid = emailRegex.test(email);
	}

	function doNothing() {}
</script>

<div class="emailcontainer">
	<div class="gradient-wrapper">
		<input
			type="email"
			bind:value={email}
			on:input={validateEmail}
			class="email-input"
			placeholder="Email address..."
		/>
	</div>
	<button class="email-button" on:click={isEmailValid ? handleSubmit : doNothing}
		>{buttonText}</button
	>
</div>

<style>
	.gradient-wrapper {
		padding: 1px;
		/* max-width: calc(25rem + 4px); */
		background: linear-gradient(91deg, rgb(69, 74, 222, 0.5) 13.45%, rgb(84, 173, 228, 0.5) 68.67%);
		border-radius: 8px;
		margin-right: 1.5rem;
	}
	@media (max-width: 768px) {
		.gradient-wrapper {
			padding: 1px;
			/* max-width: calc(25rem + 4px); */
			background: linear-gradient(
				91deg,
				rgb(69, 74, 222, 0.5) 13.45%,
				rgb(84, 173, 228, 0.5) 68.67%
			);
			border-radius: 8px;
			margin-right: 0;
            margin-bottom: 24px;
            width: 100%;
		}
	}
	.emailcontainer {
		display: flex;
	}
	@media (max-width: 768px) {
		.emailcontainer {
			width: 100%;
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
		}
	}
	.email-input {
		width: 25rem;
		font-weight: 400;
		font-style: normal;
		font-size: 1rem;
		background-color: var(--background-color);
		color: #fff;
		padding: 16px;
		/* margin-right: 1.5rem; */
		border-radius: 8px;
		border: none;
		/* border: 1px solid var(--primary-color); */
	}
	@media (max-width: 768px) {
		.email-input {
			/* width: 10rem; */
			width: 100%;
			font-weight: 400;
			font-style: normal;
			font-size: 1rem;
			background-color: var(--background-color);
			color: #fff;
			padding: 16px;
            margin: 0;
			/* margin: 0 32px; */
			/* margin-right: 1.5rem; */
			border-radius: 8px;
			border: 1px solid rgba(69, 74, 222, 0.5);
		}
	}

	.email-input::placeholder {
		font-weight: 400;
		color: rgba(255, 255, 255, 0.3);
	}

	.email-button {
		padding: 0.25rem 2rem;
		background: linear-gradient(92deg, #454ade 0.43%, #54ade4 124.53%);
		font-weight: 500;
		font-size: 1rem;
		color: #fff;
		border: none;
		border-radius: 8px;
		/* margin-left: 10px; */
		cursor: pointer;
	}
	@media (max-width: 768px) {
		.email-button {
			width: 100%;
			padding: 0.75rem 2rem;
			background: linear-gradient(92deg, #454ade 0.43%, #54ade4 124.53%);
			font-weight: 500;
			font-size: 1rem;
			color: #fff;
			border: none;
			border-radius: 8px;
			/* margin: 16px; */
			/* margin-left: 10px; */
			cursor: pointer;
		}
	}
</style>
