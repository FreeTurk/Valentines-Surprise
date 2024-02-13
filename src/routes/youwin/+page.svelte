<main>
	<div class="background"></div>
	<div class="content">
		<h1 class="title">WOOOOHOOOO!</h1>
		<div class="videos">
			<iframe
				width="1280"
				height="745"
				src="https://www.youtube.com/embed/Gnm3hIcjiCQ?autoplay=1"
				title="(*´∇`)ﾉ"
				class="video square"
				frameborder="0"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
				allowfullscreen
			></iframe>
			<iframe
				width="1280"
				height="720"
				src="https://www.youtube.com/embed/dmAfiY7yomo"
				title="send this to your crush (100% WORKING METHOD)"
				class="video"
				frameborder="0"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
				allowfullscreen
			></iframe>
		</div>
	</div>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Pixelify+Sans:wght@400..700&display=swap');

	.video {
		border-radius: 12px;
		width: 48rem;
		height: 27rem;
	}

	.video.square {
		width: 27rem;
		height: 27rem;
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
