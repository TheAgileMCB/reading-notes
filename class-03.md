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

## JavaScript & Jquery Chapter 4

### if...else statements

# if (score >= 50) {
#    congratulate();
# } else {
#    encourage();
# }

*if* and *else* are the **conditional statement**  
*(score >= 50)* is the **condition**  
*{congratulate();}* is the **if code block**  
*{encourage();}* is the **else code block**  

### switch statements

```javascript
alert('Welcome to Spaceship Repair Port.');

var spaceHandle = prompt('What is your rad space handle?')
var spaceshipPart = prompt ('What spaceship part do you need?')

//write the switch logic

switch(spaceshipPart) {
    case '1':
        console.log('This is a spaceship part one.');
    break;
    case '2':
        console.log('This is a spaceship part two.');
    break;
    case '3':
        console.log('This is a spaceship part three.');
    break;
    default:
        alert('I don\'t think we have your parts.');
    break;
}
```

### Type Coercion & Weak Typing

* if you try to use a data type JavaScript did not expect, it tries to make sense of the operation rather than report the error 
    - JavaScript is said to use **weak typing** because the data type for a value can change. Conversely, languages that use **strong typing** will require you to specifiy the data type of each variable
* due to type coercion, every value in JavaScript can be treated as if it were true or false
    - **Falsy** values are treated *as if* they are false or as the number 0
    - **Truthy** values are treated *as if* they are true or as the number 1
* the presence of an object or an array is usually considiered **truthy**
    - because the presence of an object or arry can be considered truthy, it is often used to check for the existence of an element within a page
    - a **unary operator** returns a result with just one operand
* Logical operators are prcoessed left to right. They **short-circuit (stop)** as soon as they have a result, but they return the value that stopped the processing

### Loops

#### For Loops
* runs a code a specific amount of times
* condition is usually a counter
* the most common type of loop

#### While Loops
* condition can be something other than a counter
* effective when one doesn’t know how many times a code should run

#### Do While Loops
* very similar to while loop
* will always run the code loop *at least* once, even if the condition evaluates to false

# for (var I = 0; I < 10; i++) {
# document.write(i);
# }

*for* is the **keyword**. The content within the parentheses is the **condition** and the **counter**. The code between the curly braces is what is executed during the loop.

### Loop Counters

* **Initializing**
    - create a variable and set it to a beginning value
    - this variable is commonly called *i*
    - *var i = 0;*
    - This variable is only created the first time the loop is run
    - One can use the variable *index* instead
    - The variable can also be declared before the condition

* **Condition**
    - The loop will continue to run until the counter reaches a specified number
    - *i < 10;*
    - The condition may also use a variable that holds a number

* **Update**
    - Every time the loop has run the statements within the curly braces it adds to the counter
    - *i++*
    - In this case, one is added each iteration
    - *++* - Increment Operator
    - *--* - Decrement Operator