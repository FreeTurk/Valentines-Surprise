<script>
	import { goto } from '$app/navigation';
	const prompts = ['Fuck no', 'Why', 'Just accept', 'You mean: yes?', 'Awww 😪'];
	let defaultPrompt = 'No :[';

	let scale = 1;
</script>

<main>
	<div class="background"></div>
	<div class="content">
		<div class="title">Will you be my valentine?</div>
		<div class="options">
			<button
				class="no"
				style={`padding: ${1.5 / scale}rem ${4 / scale}rem;`}
				on:click={() => {
					scale *= 1.1;
					defaultPrompt = prompts[Math.floor(Math.random() * prompts.length)];
				}}>{defaultPrompt}</button
			>
			<button
				class="yes"
				style={`padding: ${1.5 * scale}rem ${4 * scale}rem;`}
				on:click={() => {
					goto('/youwin');
				}}>Yes ❤️</button
			>
		</div>
	</div>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Pixelify+Sans:wght@400..700&display=swap');

	button {
		margin: 0;
		box-shadow: 0px 0px 4px 4px rgb(0, 0, 0, 0.2);
		background-color: pink;
		border: 4px solid plum;
		font-family: 'Pixelify Sans';
		font-size: larger;
		height: fit-content;
		border-radius: 12px;
		cursor: pointer;
		box-sizing: border-box;

		transition: all ease-in-out;
	}

	.title {
		font-family: 'Pixelify Sans';
		font-size: 4rem;
		font-weight: 700;
		color: pink;
		text-shadow: 0 0 4px black;
		background-color: plum;
		box-shadow: 0px 0px 4px 4px rgb(0, 0, 0, 0.2);
		padding: 1rem 3rem;
		border-radius: 12px;
	}

	.options {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 12px;
	}

	.content {
		height: 100%;
		width: 100%;

		display: flex;
		gap: 2rem;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.background {
		height: 100%;
		width: 100%;
		z-index: -99;
		position: absolute;

		background-color: rgba(255, 192, 203, 0.4);
		box-shadow: inset 0 0 28px 40px pink;
	}
	main {
		height: 100vh;
		width: 100vw;
		overflow: hidden;
		box-sizing: border-box;
		background-image: url('/hearts.svg');
		background-color: pink;
		background-size: 8rem;
		backdrop-filter: opacity(0.5);
		background-position: center;
		background-repeat: repeat;
	}
</style>
