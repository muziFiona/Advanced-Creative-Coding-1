# Session 4: Pixel Manipulation and Image Processing

## Recap
 - Last session we looked at basic 2D graphics concepts
 - We learned about cartesian and polar conversions
 - We also looked at how to convert between polar and cartesian coordinates (super important)
 - We learned how to draw circles from scratch using trigonometry
 - We learned about how the radius of a circle can describe the magnitude of something and also the distance between some things
 - We also thought a little about how this is the same as the hypoteneuse of a right-angled triangle
 - We learned about how the position around a circle is an angle in radians, which we can call Theta, or Phase, depending on what we're thinking about
 - We then looked at how we can use this knowledge to visualise periodic signals in polar space
 - I then set a task for you to all convert a simple processing sketch that draws interesting polar patterns so that it runs in pure JavaScript

## First
 - Let's have a look at the work you have done in the last week. 
 - Do you have any questions about the task? What problems did you have?

## Creating Images From Scratch
 - The algorithms we used for creating the polar line drawings are basic geometric 'expressions' 
 - We're now going to learn about how we can draw filled shapes using similar expressions
 - For example, take a look at this:
 - https://mimicproject.com/code/f3a32c49-7c24-556f-af1b-91315be36ad9
 - The above example uses the 'createImageData' method to draw some concentric rings.
 - We iterate through every pixels on the canvas
 - We then decide what colour each pixel should be by using a simple expression
 
## Writing output pixels
 - set red, green, blue, and alpha:
```JavaScript
position=(x+y*imageData.width)*4;
imageData.data[position] = c%255;
imageData.data[position+1] = c%255;
imageData.data[position+2] = c%255
imageData.data[position+3] = 255;```
 - 
 
