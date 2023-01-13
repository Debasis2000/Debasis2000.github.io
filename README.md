// JavaScript code to detect mobile devices
if ( /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent) ) {
  // Load mobile-specific stylesheet
  var link = document.createElement("link");
  link.href = "mobile.css";
  link.type = "text/css";
  link.rel = "stylesheet";
  document.getElementsByTagName("head")[0].appendChild(link);
}
<div id="slider">
  <img src="image1.jpg" alt="image1">
  <img src="image2.jpg" alt="image2">
  <img src="image3.jpg" alt="image3">
</div>

<script>
  var images = document.querySelectorAll("#slider img");
  var current = 0;

  function next() {
    images[current].classList.remove("active");
    current = (current + 1) % images.length;
    images[current].classList.add("active");
  }

  setInterval(next, 5000);
</script>
