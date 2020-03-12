#### Earthdate 03122020.0

# 8 Simple CSS Transitions to Blow Your Mind

Let's talk CSS! Dynamic features, once relegated to JavaScript programming, are now more accessible than ever straight from the styling language you know and love: **CSS!** Here, I’ll reproduce a number of exciting and easy-to-execute CSS properties.


## The Fade
```css
.fade {
Opacity: 0.5;
}
.fade:hover {
Opacity:1;
}
```
This property allows your element to shift opacity, increasing or decreasing its visibility to the user. It’s great for drawing attention to a call to action!


## The Color Change
```css
.color:hover {
Background-color: #ff67ee;
}
```
Apparently, animating a color change used to be very complex and involved math for calculating the change in RGB values and then recombining them. Now, it’s easier than ever—the JavaScript behind a user’s web browser handling the brunt of the workload.  


## The Grow / Shrink
```css
.grow:hover {
-webkit-transform: scale(1.3);
-ms-transform: scale(1.3);
Transform: scale(1.3);
}
```
Once upon a time, you had to transform an element’s length, width, or padding to achieve this effect, but now you can simply scale the element. A scale higher than one will grow an element, whereas a scale below 1 will shrink it.
```css
.shrink:hover {
-webkit-transform: scale(0.8);
-ms-transform: scale(0.8);
Transform: scale(0.8);
}
```


## The Rotation
```css
.rotate:hover {
-webkit-transform: rotate(-30deg);
-ms-transform: rotate(-30deg);
Transform: rotate(-30deg);
}
```
This property rotates an element to the degree specified in the parentheses!


## TheSquare to Circle Transformation
```css
.circle:hover {
Border-radius:50%
}
```
Easy. Change the border-radius of an element to watch it morph shapes before your eyes!


## The 3-Dimensional Shadow
```css
.threed:hover {
Box-shadow:
1px 1px #ffffff,
2px 2px #ffffff,
3px 3px #ffffff;
-webkit-transform: translateX(-3px);
Transform: translateX(-3px);
}
```
Once shunned, the 3D shadow is now and easy and (when used tastefully) an effective tool at highlighting depth and dynamics on a web page. Translate gives the element the effect of moving along the Z-axis.


## The Swing
```css
@-webkit-keyframes swing
{
15%
{
-webkit-transform: translateX(5px);
Transform: translateX(5px);
}
30%
{
-webkit-transform: translateX(-5px);
Transform: translateX(-5px);
}
50%
{
-webkit-transform: translateX(3px);
Transform: translateX(3px);
}
65%
{
-webkit-transform: translateX(-3px);
Transform: translateX(-3px);
}
80%
{
-webkit-transform: translateX(2px);
Transform: translateX(2px);
}
100%
{
-webkit-transform: translateX(0);
Transform: translateX(0);
}
}
@keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
        transform: translateX(-5px);
    }
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
```
Not all of these flashy effects use the *transition* property. *@keyframes* is another styling property that adds great effects to a page. (**note:** You’ll notice the continued use of *webkit* identifiers. This is to handle compatibility issues between browsers. Technology moving as fast as it does, browsers can be slow to implement certain changes.) This property must be defined within your CSS styles first.
```css
.swing:hover {
-webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}
```


## The Inset Border
```css
.border:hover {
Box-shadow: inset 0 0 0 25px #45ee9e;
}
```
A useful reimagining of a popular web page feature—the ghost button. It’s a button with no background and a heavy border. There are, of course, many ways to accomplish the effect, but, thanks to CSS’s new dynamic features, this is as simple a solution as they come!

That’s it! Use these simple and accessible dynamic properties to excite your web pages and aw your users!
