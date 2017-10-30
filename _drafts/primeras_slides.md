---
layout: slides
title: Machine Learning y Neural Networks
excerpt: Curso en español
date: 2017-09-20
tags: [Slides]

d3jsv3: true
threejs: false
functionPlot: true
---

<section>
    <h1>Machine Learning</h1>
    <h1>&</h1>
    <h1>Neural Networks</h1>
    <h3>Curso en Español</h3>
    <p>
        <small>
            Creado por <a href="http://twitter.com/guiferviz">@guiferviz</a>
        </small>
    </p>
</section>

<section data-markdown>
### Linear models
$$\hat{y} = \mathbf{w}^T \cdot \mathbf{x} + b$$
</section>

<section data-markdown>
### Linear models
Python example

```python
import numpy as np

d = 10
w = np.random.rand(d)
b = np.random.rand(1)

def f(x):
    """ Last slide math expression. """
    return np.dot(w.T, x) + b

f(np.random.rand(d))
```
</section>

<section data-state="plot-slide">
<div id="plot-container" style="min-height: 400px;"></div>
<style>
    .function-plot > .x.axis > .tick > line {
        fill: green;
    }
    
    .function-plot .y.axis {
        .tick {
          line {
            fill: red;
          }
          text {
            fill: blue;
          }
        }
        path.domain {
          fill: yellow;
        }
      }
    }
</style>
</section>

<section data-background="https://i0.wp.com/www.extremetech.com/wp-content/uploads/2013/09/340.jpg">
    <h1 style="color: #fff;">¡Neural Networks!</h1>
</section>


<script>
    Reveal.addEventListener("plot-slide", function () {
        functionPlot({
            target: '#plot-container',
            grid: true,
            yAxis: {domain: [0, 10]},
            xAxis: {domain: [0, 10]},
            width: 500,
            height: 500,
            disableZoom: true,
            data: [{
                points: [
                    [1, 1],
                    [2, 1],
                    [2, 2],
                    [1, 2],
                    [1, 1]
                ],
                fnType: 'points',
                graphType: 'scatter',
                attr: {"fill": "green", "r": 5, "stroke": "none"}
            },
            {
                fn: 'x^2',
                skipTip: false
            },
            {
                vector: [2, 1],
                offset: [1, 0],
                graphType: 'polyline',
                fnType: 'vector'
            }]
        })
    });
</script>
