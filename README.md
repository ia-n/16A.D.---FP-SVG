# FP7-SkraM
##Authors

Ian Roberts

Dmitri Kheifets

##Overview

Much similar to your typical paint program. With this software you are able to construct customize objects and place them on the screen. 
##Screenshot


<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br>



##Concepts Demonstrated

* **Object Passing** is used for the majority of the GUI 
* The objects for the shapes stored the type of shape as well as attributes 
* **Message passing** is how our different files communicate.

##External Technology and Libraries

* **racket/gui/base** provided us with the canvas, panes, gui objects and  mouse events 
* **racket/draw** provided us with color, brush and bitmap objects
* **xml** provided us with the functionality to save our picture









##Favorite Scheme Expressions
####Ian Roberts
```scheme


         ((λ () ( if (> x1  x2) (- x1 (max w h)) sx)))
         ((λ () ( if (> y1  y2)  (- y1 (max w h)) sy)))
         ((λ (max-run) (begin (set! max-run (max w h)) max-run))0)
         ((λ (max-run) (begin (set! max-run (max w h)) max-run))0)
```

The code above was used to allow a shape object to change its starting and end points
without that ability you could not draw a shape upwards or left.
The reason I like this code so much is because it stumped me for a long time.
What made it so difficult was trying to debug, with no clear indications other
than a crazy shape movement pattern it required me to deeply think about the
math events happening on the grid

#How to Download and Run

The code can be downloaded here:
https://github.com/ia-n/16A.D.---FP-SVG.git

To start things off, you need to only run main.rkt

From here we have a few menus, 

**Main Window**

The left side you will find your shapes.

At the bottom Save and undo.

The rest is your drawing area

**Side window**


The radio buttons 'stroke 'fill

These will allow you to change the color of the outline/filling.

Whats nice about these is that they remember their respective color settings


The above shape

The oval above allows you to preview the colors you have selected.


Apply fill check box

This gives the user the choice to to draw the shapes with or without filling.
