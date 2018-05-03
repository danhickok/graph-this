# graph-this
### _A stand-alone, single-file web application for graphing algebraic functions_

Some time ago I wanted to find a nice combination of sine waves that, when applied to the red, green, and blue components of a series of elements, would provide a nice gradient of colors.  So I thought, "Is there a simple application out there that could draw the sine functions I wanted to use?"

Well, there are *lots* of applications out there, but nothing really simple -- and most required multiple files (as all good applications do).  Some depended heavily on external libraries to do the drawing.  What I really wanted was just a simple, one-page application.

So I made one.

"Graph This!" is a single HTML file - no dependent libraries, no compiler, nothing else required but this one file.  Open it in any HTML5-compliant browser that supports the canvas element and JavaScript -- er, I mean ECMAScript 2016 (ES6), and you'll get a page that lets you enter up to four formulas.  Then click any of the zoom or movement buttons, and you'll see your functions graphed out in their corresponding colors.

The formulas should be in "computerese".  You can enter an asterisk (`*`) for multiplication or an up-arrow (`^`) for raising to a power.  Additionally, all the ES6 math functions are available.  (You don't need to put "`Math.`" in front of the functions.)  Spaces are optional, but I like them for readability.

Here are some interesting formulas to try:

* `sin(pi * x) / x`
* `e^x`
* `sign(sin(pi * x))`

It's easy to use, and easy to modify.  I've included lots of comments to guide you.  To add more formulas, all you need to do is add additional colors to the `colorOf.formula` array.

#### Planned Features

Right now, only Cartesian functions are supported.  I plan to add two more "modes":  one for polar functions, and one for parametric functions (that is, where X and Y are functions of time).

I also want to add an option to make a legend at the bottom showing the formulas used for each graph.

Not all browsers let you right-click and save the drawn image, so I am thinking of adding a button to let you do that.

I want to add a "save" and "restore" button to let you set up formulas ahead of time.
