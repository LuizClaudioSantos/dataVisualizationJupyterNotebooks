# Data Visualization in Python


## Data Visualization Best Practices (Darkhorse Analytics)

1. Less is more effective

2. Less is more attractive

3. Less is more impactive


## Matplotlib 

It is a library used to build data visualizations in Python, for more matplotlib official documentation click [here](https://matplotlib.org/).


### Matplotlib Architecture

The Matplotlib has three main parts: Scripting Layer (pyplot), Artist Layer (Artist) and Backend Layer (FigureCanvas, Renderer, Event).

#### Backend Layer

The backend layer has three main abstract interface classes:

1. FigureCanvas: **matplotlib.backend_bases.FigureCanvas**
* Encompasses the are onto which the figure is drawn.

2. Renderer: **matplotlib.backend_bases.Renderer**
* Knows how to draw on the FigureCanvas

3. Event: **matplotlib.backend_bases.Event**
* Handles user inputs such as keyboard strokes and mouse clicks

### Artist Layer

* Comprised of one object - **Artist**. It knows how to use the Renderer to draw on the canvas.

* Title, lines, tick labels, and images, all correspond to individual Artist instances.

* Two types of **Artist** objects:

1. **Primitive**: Line2D, Rectangle, Circle and Text.
2. **Composite**: Axis, Tick, Axes and Figure.

* Each composite arist may contain other composite artists as well as primitive artists.

* Here you can check out a basic usage of matplotlib with Artist Layer.

A simple example of an histogram can be found [here](first_matplotlib.ipynb)

