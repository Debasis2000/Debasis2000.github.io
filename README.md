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

      const body = document.querySelector("body");
let colorPallete = ["#ff0000", "#00ff00", "#0000ff", "#ff00ff", "#00ffff", "#ffff00"];
let currentIndex = 0;

function changeBodyColor() {
  body.style.backgroundColor = colorPallete[currentIndex];
  currentIndex = (currentIndex + 1) % colorPallete.length;
}

setInterval(changeBodyColor, 2000);
