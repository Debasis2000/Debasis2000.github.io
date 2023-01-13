// JavaScript code to detect mobile devices
if ( /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent) ) {
  // Load mobile-specific stylesheet
  var link = document.createElement("link");
  link.href = "mobile.css";
  link.type = "text/css";
  link.rel = "stylesheet";
  document.getElementsByTagName("head")[0].appendChild(link);
}
