<script lang ts>
	var days: string = '?';
	var hours: string = '?';
	var minutes: string = '?';
	var seconds: string = '?';

	// Set the date we're counting down to
	var countDownDate = new Date('Jan 5, 2024 15:37:25').getTime();

	// Update the count down every 1 second
	var x = setInterval(function () {
		// Get today's date and time
		var now = new Date().getTime();

		// Find the distance between now and the count down date
		var distance = countDownDate - now;

		// Time calculations for days, hours, minutes and seconds
		days = Math.floor(distance / (1000 * 60 * 60 * 24)).toString(10);
		hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60)).toString(10);
		minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60)).toString(10);
		seconds = Math.floor((distance % (1000 * 60)) / 1000).toString(10);
	}, 1000);
</script>

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Anton&display=swap" rel="stylesheet" />
<div>
	<h4 class="timer-desc">Young go loud is over</h4>
	<h2 class="countdown">{days}d {hours}h {minutes}m {seconds}s</h2>

	<p>
		Dit is een omschrijving van Young go loud, er zit ook een goede reden bij om naar young go loud
		te gaan. Lorem ipsum dolor sit amet, consectetur adipiscing elit
	</p>
</div>

<h3>Vind ons op de socials</h3>
<link href="https://css.gg/instagram.css" rel="stylesheet" />
<link href="https://css.gg/facebook.css" rel="stylesheet" />
<div class="socials">
	<a class="logo" style="color:white;" href="https://www.instagram.com/younggoloud.official">
		<i class="gg-instagram" />
	</a>

	<a class="logo" style="color: white;" href="https://nl-nl.facebook.com/BussumCultureel">
		<i class="gg-facebook" />
	</a>
</div>

<style>
	.logo {
		transform: scale(3);
	}

	.socials {
		display: flex;
		gap: 4em;
		justify-content: center;
		margin-top: 10vh;
		margin-bottom: 10vh;
	}

	h3 {
		text-align: center;
		font-family: cacha_personal_useregular, sans-serif;
		color: #feec02;
		font-size: 5vw;
		margin-bottom: vh;
	}

	p {
		line-height: 1em;
		margin-right: 10vw;
		margin-left: 10vw;
		text-align: center;
		font-size: 20px;
		font-family: roboto, sans-serif;
		color: #ff6961;
	}

	.countdown {
		text-align: center;
		margin-top: 1vh;
		font-family: 'Anton', sans-serif;
		letter-spacing: 5px;
		font-size: 10vw;
		color: #4afaae;
	}

	.timer-desc {
		text-align: center;
		font-family: 'cacha_personal_useregular', sans-serif;
		letter-spacing: 5px;
		font-size: 5vw;
		margin-bottom: -2vh;
		color: #0801f9;
	}

	@font-face {
		font-family: 'cacha_personal_useregular';
		src: url('cachapersonaluseregular-gox6g-webfont.woff2') format('woff2'),
			url('cachapersonaluseregular-gox6g-webfont.woff') format('woff');
		font-weight: normal;
		font-style: normal;
	}
</style>
