# Chart JS

- Chart.js is a popular open source library that helps us to plot data in web applications. It is highly customizable, but configuring all of its options remains a challenge for some people. Let’s explore it, starting from a simple example and building upon it.

CHARTS :

There are three functions that draw rectangles on the canvas:

- fillRect(x, y, width, height) Draws a filled rectangle.
  strokeRect(x, y, width, height) Draws a rectangular outline.
- clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.

Drawing text

The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth])

Fills a given text at the given (x,y) position.

Optionally with a maximum width to draw. strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

Drawing
fillRect(x, y, width, height) Draws a filled rectangle.

strokeRect(x, y, width, height) Draws a rectangular outline.

clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.

```
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}
```

basic example :

index.html :

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Exploring Chart.js</title>
</head>
<style>
    .container {
        width: 50%;
        height: 50%;
    }
</style>
<body>

    <button id="renderBtn">
        Render
    </button>
    <div class="container">
        <canvas id="myChart"></canvas>
    </div>

</body>

<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.7.2/Chart.js"></script>
<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
<script src="./myChart.js"></script>

</html>
```

chart.js:

```
function renderChart(data, labels) {
    var ctx = document.getElementById("myChart").getContext('2d');
    var myChart = new Chart(ctx, {
        type: 'line',
        data: {
            labels: labels,
            datasets: [{
                label: 'This week',
                data: data,
            }]
        },
    });
}

$("#renderBtn").click(
    function () {
        data = [20000, 14000, 12000, 15000, 18000, 19000, 22000];
        labels =  ["sunday", "monday", "tuesday", "wednesday", "thursday", "friday", "saturday"];
        renderChart(data, labels);
    }
);

```

Setting the type variable, we could change the line chart into a bar chart, or even a pie chart. All of the different types of charts can be seen here.
As you can see, datasets is an array. That means that we can plot two or more data series in the same chart. We will get back to this possibility later on in the article.
The result of our project so far is:

![](https://miro.medium.com/max/686/0*dXiwKGxGJ-mPju_g)
