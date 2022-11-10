<div class=top-bar>
    <img style="margin-right: 5%" src="logo.png" alt="young go loud logo">
    <h1 class=glow>Young go loud</h1>
</div>

<slot></slot>

<style>
    .top-bar {
        height: 10vh;
        display: flex;
    }

    h1 {
		font-family: 'Rubik Bubbles', cursive;
	}

    .glow {
		color: #FD60F5;
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
			text-shadow: 0 0 20px #fff, 0 0 30px #D6E05E, 0 0 40px #D6E05E, 0 0 50px #D6E05E,
				0 0 60px #D6E05E, 0 0 70px #D6E05E, 0 0 80px #D6E05E;
		}
	}
</style>