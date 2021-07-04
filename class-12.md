# Docs for the HTML `<canvas>` Element & Chart\.js

## Chart.js

**- Chart.js:** Chart.js is an open source JavaScript library that makes it easy to include charts in your website. The charts are animated and responsive so we can show it on any device.

**- How to Use Chart.js?** 
* First, add a link to the providing *CDN* (**C**ontent **D**elivery **N**etwork):

```
<script
src="https://.js">
</script>
```


* Then, add a `<canvas>` to where you want to draw the chart:

```
<canvas id="myChart" style="width:100%;max-width:700px"></canvas>
```


* The canvas element must have a unique **id**.



**- Chart.js comes with the following built-in chart types:**

1. Scatter
2. Line
3. Bar
4. Radar
5. Pie and Doughnut
6. Polar Area
7. Bubble


* Typical Scatter Chart Syntax:


```
var myChart = new Chart("myChart", {
  type: "scatter",
  data: {},
  options: {}
});
```


* Typical Line Chart Syntax:

```
var myChart = new Chart("myChart", {
  type: "line",
  data: {},
  options: {}
});
```


* Typical Bar Chart Syntax:

```
var myChart = new Chart("myChart", {
  type: "bar",
  data: {},
  options: {}
});
```


## Canvas

**- What is the HTML Canvas:** 
* A canvas is a rectangular area on an HTML page. By default, a canvas has no border and no content.

* The markup looks like this:

```
<canvas id="myCanvas" width="200" height="100"></canvas>
```


* The HTML `<canvas>` element is used to draw graphics, on the fly, via JavaScript.

* The `<canvas>` element is only a container for graphics. You must use JavaScript to actually draw the graphics.

* **Canvas** has several methods for drawing paths, boxes, circles, text, and adding images.


**- Drawing shapes with canvas:** First let's look at the rectangle. There are three functions that draw rectangles on the canvas:

* fillRect(x, y, width, height) : Draws a filled rectangle.

* strokeRect(x, y, width, height) : Draws a rectangular outline.

* clearRect(x, y, width, height): Clears the specified rectangular area, making it fully transparent.

Rectangular shape example:

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




