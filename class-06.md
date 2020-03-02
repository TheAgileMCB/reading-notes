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