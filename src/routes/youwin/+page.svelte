<main>
	<div class="background"></div>
	<div class="content">
		<h1 class="title">WOOOOHOOOO!</h1>
		<div class="videos">
			<iframe
				src="https://www.youtube.com/embed/Gnm3hIcjiCQ?autoplay=1"
				title="CAT DANCE!!!"
				frameborder="0"
				class="video square"
				allow="autoplay"
				allowfullscreen
			></iframe>
			<iframe
				src="https://www.youtube.com/embed/dmAfiY7yomo"
				title="I LOVE YOUUUU!"
				frameborder="0"
				class="video"
				allowfullscreen
			></iframe>
		</div>
	</div>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Pixelify+Sans:wght@400..700&display=swap');

	.video {
		border-radius: 12px;
		height: 27rem;
		width: 48rem;
	}

	.video.square {
		width: 27rem;
	}

	.videos {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 2rem;
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
