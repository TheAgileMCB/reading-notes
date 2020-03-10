#### Earthdate 10032020

# Chart.js

## Drawing a Line Chart

Begin with HTML metadata including the script for the Chart.js library in the head:

```html
<!DOCTYPE html>
<html lang="en-us">
  <head>
    <meta charset="utf-8" />
    <title>Chart.js demo</title>
    <script> src='Chart.min.js'></script>
  </head>
  <body>
  </body>
</html>
```

include the *canvas* HTML element in order to lay a foundation for your chart:

```html
<canvas id="buyers" width="600" height="400"></canvas>
```

Then, include a script in the foot of your page that functions to retreive the context of the canvas as well as a function to style the chart:

```html
<script>
  var buyerData = {
    labels: ["January", "February", "March", "April", "May", "June"],
    datasets: [
      {
        fillColor: "rbga(172, 194, 132, 0.4)",
        strokeColor: "#acc26d",
        pointColor: "#fff",
        pointStrokeColor: "#9db86d",
        data: [203, 156, 99, 251, 305, 247]
      }
    ]
  }
  var buyers = document.getElementById('buyers'). getContext('2d');
  new Chart(buyers).Line(buyerData);
</script>
```

And it's that simple! the result will be a stylish animated line graph.

It's important to remember that the canvas element produces a fixed-size element, and if you style it with CSS without thought towards the proportionality of the the surface you will distort your chart. It is also good practice to include an if / else javascript statement for the event that a user has an unsupported browser. The latter part of the statement should include text describing the key points of the chart, because it will be shown to users who cannot see it.