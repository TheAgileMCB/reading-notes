# Earthdate 02032020

## JavaScript&Jquery Chapter 3

### Objects

* **objects** group togehter a set of variables and functions to create a model of something you would recognizr from the real world  
* literal notation is the easiest and most popular way to create objects  

```javascript
var hotel = {
  name: 'Quay',
  rooms: 40,
  booked: 25,
  gym: true,
  roomTypes: ['twin', 'double', 'suite'],
  
  checkAvailability: function() {
    return this.room - this.booked;
  }
};
```

* a hotel **object**  
* name - roomTypes are the **properties**, *name: 'Quay'* represent a **key/value pair**  
* *checkAvailability* and the following function is a **method**  
* a **method** is an action that can be performed on an object
* separate each key from its value with a colon  
* separate each property and method with a comma  
* the **this** keyword indicates that the method is using the property of *this* object  
* **Dot notation** - to access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method  
* the period is known as the **member operator**  
* the property or method on the right is a member of the object on its left  
* you can also access the properties and methods of an object using square brackets - most commonly used when:  
  * the name of the property or method contains special characters  
  * the name of the property is a number  
  * a variable is being used in place of the property name  
  * an object is reusable - the values exchangable  

## JavaScript&Jquery Chapter 5

### Document Object Model

* the **DOM** is neither part of HTML, nor JavaScript; it is a separate set of rules  
* the DOM specifies the way in which the browser should structure this model using a **DOM tree**  
* the DOM tree is made of objects  
* each object represents a differet part of the page loaded in the browser  
the DOM is also called an **Application Programming Interface (API)**  
  * user interfaces let humans interact with programs; APIs let programs (and scripts) talk to each other  

#### The DOM Tree is the model of a wedpage

* it is stored in the browser and consists of 4 types of nodes:  
  * The **document node** represents the entire page and is at the top of the DOM tree
  * **Element nodes** *describe* the structure of an HTML page  
  * **Attribute nodes** are not *children* of the element that carries them; they are *part of* that element
  * **Text nodes** the text of an element

#### Accessing Elements

* **getElementById()** - uses the value of an element's id attribute
* **querySelector()** - uses a CSS selector, and returns the first matching element  
* **getElementsByClassName()** - selects elements that a specific value for their class name  
* **getElementsByTagName** - selects elements that have the specified tag name  
* **querySelectorAll** - uses a CSS selector to select all matching elements
* **parentNode** - selects the parent of the current element node
* **previousSibling / nextSibling** - selects the previous or next sibling from the DOM tree  
* **firstChild / lastChild** - select the first or last child of the current element  

#### Work with Those Elements

* **nodeValue** - lets you access or update contens of a text node
* **innerHTML** - allows you to access the text of child elements
* **textContent** - allows access of just the text
* **createElement(), createTextNode(), appendChild() / removeChild()** - methods that allow you to create new nodes, add nodes to a tree, and remove nodes from a tree  
* **hasAttribute(), getAttribute(), setAttribute(), removeAttribute()** - checks if an attribute exists, gets its value, updates its value, removes the attribute

#### Update HTML Contents

##### document.write()
Advantages  
* it is quick and easy for beginners 
Disadvantages  
* it only works when the page initially loads
* if you use it after the page loads it can:  
  * overwrite the whole page  
  * not add the content to the page  
  * create a new page
* tt can cause problems with XHTML pages that are strictly validated
* this method is very rarely used by programmers these days

##### element.innterHTML
Advantages  
* you can use it to add a lot of new markup using less code than the DOM manipulation method
* it can be faster than DOM manipulation when adding a lot of new elements
* it is a simply way to remove all of the content from one element
Disadvantages  
* it should not be used to add content that has come from a user
* it can be difficult to isolate single elements
* event handlers may no longer work as intended

##### DOM Manipulation
Advantages  
* it is suited to changing one element from a DOM fragment where there are many siblings
* it does not affect event handlers
* it easily allows a script to add elements incrementally
Disadvantages
* if you have to make a lot of changes to the content of a page, it is slower than innerHTML
* you need to write more code to achieve the same things compared with innerHTML