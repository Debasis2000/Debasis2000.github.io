<!DOCTYPE html>
<html>
  <head>
    <title>My Website</title>
  </head>
  <body>
    <script>
      // Create a new element
      var newHeading = document.createElement("h1");

      // Create a text node
      var headingText = document.createTextNode("Welcome to My Website");

      // Append the text node to the heading element
      newHeading.appendChild(headingText);

      // Append the heading element to the body
      document.body.appendChild(newHeading);
    </script>
  </body>
</html>
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
<script>
  // Get the current year
  var currentYear = new Date().getFullYear();

  // Get the copyright element
  var copyright = document.querySelector("footer p");

  // Update the copyright year
  copyright.innerHTML = "Copyright &copy;" + currentYear + " My Website";
</script>
