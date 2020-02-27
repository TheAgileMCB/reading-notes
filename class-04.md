# Earthdate 26022020

## HTML&CSS Chapter 4

### Links

#<a href="http://www.imdb.com">IMDB</a>

The content with in the first pair of angle brackets is the **opening link tag**. The *</a>* element is the closing link tag. and the content between the two tags is the clickable link.  
Users will be taken to the page specified in the href attribute. When you link to a differet website, the value of the href attribute will be the full web address for the site, known as an **absolute** URL. When you link to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a **relative** URL.

* **mailto:** - creates a link that starts up the users email program when target by the href attribute.  
* the **target** attribute can be used one the opening link tag with a value of *_blank* to open a link in a new page.  
* You can link internally to a spot on the same page by targeting an *id* attribute (href="#contact-me")  
* You can link to id attributes on external pages, as well, by following the same syntax with another page's URL (href="http://www.htmlandcssbook.com/#bottom")  


## HTML&CSS Chapter 15

### Layout

CSS treats each HTML element as if it is in its own box. Boxes will either be **block-level** or **inline**. Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text.  
If one block-level element sits inside another block-level element then the outer box is known as the **containing** or **parent** element.

#### Element Position

CSS has the following **positioning schemes**:
    - Normal Flow  
        - every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-by-side, they will not appear next to each other.  
    - Relative positioning  
        - this moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements.
    - Absolute positioning  
        - this positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements.  

You specify the positioning scheme using the *position* property in CSS. You can also float elements using the *float* property. To indicate where a box should be positioned, you may also need to use **box offset* properties to tell the browser how far from the top or bottom and left or right it should be placed.  
    - **Fixed positioning** is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.  
    - **Floating elements** allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.  
    - the **z-index** property allows you to control which box appears on top when elements are floated


## JavaScript&Jquery Chapter 3

### Functions  

**Functions** let one group a series of statements together to perform a specific task. Functions are *reusable*. Functions will also help one *store* the steps needed to achieve a task. In order to **call**, or ask it to operate, later a function must be given a name. Some functions must be provided with information to perform their task. This information is called **parameters**. When you write a function and expect it to produce an answer, the answer is known as a **return value**.  

# function sayHello() {
# document.write(‘Hello!’);
# }

*function* is referred to as the **function keyword**. *sayHello* is the **function name** and the content with the curly braces is considered the **code block**.  

# function getArea(width, height) {
# Return width * height;
# }

The content within the parentheses are **parameters**. The parameters are used like variables within the function.  

When one calls a function the needs information, one must insert appropriate information within the parentheses to fulfill the parameters. This information are called **arguments**.  

#### Anonymous Functions & Function Expressions

A **function declaration** creates a function that you can call later in your code. In order to call a function later, you must give it a name. It is, then, a **named function**.  

If you put a function where the interpreter would expect to see an expression, then it is treated as an expression, and it is known as a **function expression**. In function expressions, the name is usually omitted. A function with no name is called an **anonymous function**. **Immediate Invoked Function Expressions(IIFE)** are a type of anonymous function.  
* When to use anonymous functions and IIFE:  
    - as an argument when a function is called (to calculate the value for that function)  
    - To assign the value of a property to an object
    - In event handlers and listeners to perform a task when an event occurs
    - To prevent conflicts between two scripts that might use the same variable names  

#### Variable Scope

The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variables **scope**. Specifically, this variable has **local scope**. If you create a variable *outside* of a function, then it can be used anywhere within the script. This is known as **global scope**.  

If you forget to declare a variable using the *var* keyword, it will be automatically treated as a *global* variable. Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that the function is being executed.  


## 6 Reasons for Pair Programming

1. Greater efficiency

2. Engaged collaboration

3. Learning from fellow students

4. Social skills

5. Job interview readiness

6. work environment readiness
