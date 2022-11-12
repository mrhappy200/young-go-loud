<div class="top-bar">
	<a style="margin-right: 5%" class="top-bar" href="http://example.com">
		<img style="margin-right: 5%" src="logo.png" alt="young go loud logo" />
	</a>
	<h1 class="glow">Young go loud</h1>
</div>

<slot />

<style>
	.top-bar {
		height: 10vh;
		display: flex;
		margin-bottom: 7vh;
	}

	h1 {
		font-family: 'Rubik Bubbles', cursive;
	}

	.glow {
		color: #fd60f5;
		text-align: center;
		-webkit-animation: glow 2s ease-in-out infinite alternate;
		-moz-animation: glow 2s ease-in-out infinite alternate;
		animation: glow 2s ease-in-out infinite alternate;
	}

	@-webkit-keyframes glow {
		from {
			text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px #effb6a, 0 0 40px #effb6a,
				0 0 50px #effb6a, 0 0 60px #effb6a, 0 0 70px #effb6a;
		}
		to {
			text-shadow: 0 0 20px #fff, 0 0 30px #d6e05e, 0 0 40px #d6e05e, 0 0 50px #d6e05e,
				0 0 60px #d6e05e, 0 0 70px #d6e05e, 0 0 80px #d6e05e;
		}
	}
</style>
