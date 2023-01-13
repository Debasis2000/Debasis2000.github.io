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
