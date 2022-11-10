<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Anton&display=swap" rel="stylesheet">

<h2>{days}d {hours}h {minutes}m {seconds}s</h2>
<style>
h2 {
    text-align: center;
    font-family: 'Anton', sans-serif;
    letter-spacing: 5px;
    font-size: 20vw;
    color: #4AFAAE;
}
@font-face {
    font-family: 'cacha_personal_useregular';
    src: url('cachapersonaluseregular-gox6g-webfont.woff2') format('woff2'),
         url('cachapersonaluseregular-gox6g-webfont.woff') format('woff');
    font-weight: normal;
    font-style: normal;

}
</style>

<script lang=ts>
    var days: number;
    var hours: number;
    var minutes: number;
    var seconds: number;

    // Set the date we're counting down to
    var countDownDate = new Date("Jan 5, 2024 15:37:25").getTime();
    
    // Update the count down every 1 second
    var x = setInterval(function() {
    
      // Get today's date and time
      var now = new Date().getTime();
    
      // Find the distance between now and the count down date
      var distance = countDownDate - now;
    
      // Time calculations for days, hours, minutes and seconds
      days = Math.floor(distance / (1000 * 60 * 60 * 24));
      hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      seconds = Math.floor((distance % (1000 * 60)) / 1000);
    }, 1000);
</script>