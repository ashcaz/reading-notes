# Matplotlib

**LINKS**

- [Matplotlib Tutorial](https://www.labri.fr/perso/nrougier/teaching/matplotlib/)
- [Video: Seaborn Tutoiral](https://seaborn.pydata.org/tutorial.html)
- [Video: Bokeh Tutorial](https://mybinder.org/v2/gh/bokeh/bokeh-notebooks/master?filepath=tutorial%2F00%20-%20Introduction%20and%20Setup.ipynb)
- [Seaborn Cheat Sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Python_Seaborn_Cheat_Sheet.pdf)

## Matplotlib tutorial

### Introduction

matplotlib is probably the single most used Python package for 2D-graphics. It
provides both a very quick way to visualize data from Python and
publication-quality figures in many formats. We are going to explore
matplotlib in interactive mode covering most common cases.

### IPython and the pylab mode

`IPython <http://ipython.org/>`\_ is an enhanced interactive Python shell that
has lots of interesting features including named inputs and outputs, access to
shell commands, improved debugging and much more. When we start it with the
command line argument -pylab (--pylab since IPython version 0.12), it allows
interactive matplotlib sessions that have Matlab/Mathematica-like functionality.

### pyplot

pyplot provides a convenient interface to the matplotlib object-oriented
plotting library. It is modeled closely after Matlab(TM). Therefore, the
majority of plotting commands in pyplot have Matlab(TM) analogs with similar
arguments. Important commands are explained with interactive examples.

### Simple plot

In this section, we want to draw the cosine and sine functions on the same
plot. Starting from the default settings, we'll enrich the figure step by step
to make it nicer.

The first step is to get the data for the sine and cosine functions:

```Python

   import numpy as np

   X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
   C, S = np.cos(X), np.sin(X)
```

X is now a NumPy array with 256 values ranging from -π to +π (included). C is
the cosine (256 values) and S is the sine (256 values).

To run the example, you can download each of the examples and run it using::

    $ python exercice_1.py

You can get source for each step by clicking on the corresponding figure.

### Using defaults

.. admonition:: Documentation

[plot tutorial](http://matplotlib.sourceforge.net/users/pyplot_tutorial.html)
[plot() command] (http://matplotlib.sourceforge.net/api/pyplot_api.html#matplotlib.pyplot.plot)

Matplotlib comes with a set of default settings that allow customizing all
kinds of properties. You can control the defaults of almost every property in
matplotlib: figure size and dpi, line width, color and style, axes, axis and
grid properties, text and font properties and so on. While matplotlib defaults
are rather good in most cases, you may want to modify some properties for
specific cases.

[Back to Homepage](https://ashcaz.github.io/reading-notes)
