# Earthdate 25022020

## HTML&CSS Chapter 3

### Lists
*	**Ordered lists** are lists where each item in the list is numbered  
        
        <ol>  
            <li>Chop cabbage</li>  
            <li>Slice cucumber</li>  
            <li>Peel tomato</li>  
        </ol>  
        
*	**Unordered lists** are lists that begin with a bullet point  

        <ul>  
            <li>Peanuts</li>  
            <li>Grapes</li>  
            <li>Bread</li>  
        </ul>  

*	**Definition lists** are made of a set of terms along with the definitions for each of those terms  

        <dl>
            <dt>Sashimi</dt>
            <dd>Slice raw fish that is served with condiments such as shredded daikon raddish or ginger root.</dd>
            <dt>Scale</dt>
            <dd>A device used to accurately measure the weight of ingrdients</dd>
        </dl>
            
* lists can be nested


## HTML&CSS Chapter 13

### Boxes

* By default a box is sized just big enough to hold its contents, but you can use the **width** and **height** properties.
* The **min-width(height)** and **max-width(height)** properties can be used to limit the size of boxes
* the **overflow** property tells the browser what to do if the content contained within a box is larger than the box itself.
    - **hidden** hides any extra content that does not fit in the box
    - **scroll** adds a scrollbar to the box
* **padding** is the space between a box's border and its content
* every box has a **border** even if it is not visible or specified at 0 pixels
    - the **border-width** property controls the width of a border
    - the **border-style** property styles a border
        * solid
        * dotted
        * dashed
        * double
        * groove
        * ridge
        * inset
        * outset
        * hidden/none
    - the **border-color** property will color the border
    - shorthand: border property (width, style, color)
* **margin** is the space outside the edge o the border
* to center a box on the page you must set the box with a width, then set *left-margin* and *right-margin* to *auto*. In order to make this work in older browsers, you must also use the *text-align: center* property and value
* the **display** property allows you to turn an inline element into a block-level element or vice versa
    - **inline** causes a block-level element to act like an inline element
    - **block** causes an inline element to work like a block-level element
    - **inline-block** causes a block-level element to flow like a inline element, while retaining other features of a block-level element
    - **none** hides an element from the page
* ther **visibility** property allows you to hide boxes from users but it leaves a space where the element would have been
    - **hidden** hides the element
    - **visible** shows the element
* the **border-image** property applies an image to the border of any box
    1. the URL of the image
    2. Where to slice the image
    3. What to do with the straight edges; values are:
        * **stretch** to stretch the image
        * **repeat** to repeat the image
        * **round** which repeats the image, but scales the tiles of the image to fit exactly
    - the box must also have a *border-width*
* the **box-shadow** property allows you to add a drop shadow around a box
    - **horizontal offset**
    - **vertical offset**
    - **blur distance**
    - **spread of shadow**
    - **inset**
* the **border-radius** property rounds the corners of any box
    - horizontal and vertical values can be specified independently *{border-radius: 1em 2em 1em 2em / 2em 4em 2em 4em;}*

###