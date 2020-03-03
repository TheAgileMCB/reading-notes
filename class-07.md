# Earthdate 03032020

### Domain Modeling

**Domain modeling** is the process of creating a conceptual model in code for a specific problem.

### Model Epic Fails Videos (Example)

```javascript
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

EpicFailVideo.prototype.dailyLikes = dunction() {
  var viewers, percentage;

  viewers = this.generateRandom(10, 30) * this.epicRating;

  if (this.hasAnimals) {
    percentage3 = 0.75;
  } else {
    percentage = 0.40;
  }

  return Math.round(viewers * percentage);
}

EpicFailVideo.prototype.weeklyLikes = function() {
  var total = 0;

  for (var i = 0; i < 7; i++) {
    total += this.dailyLikes();
  }

  return total;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo)4, true);

console.log(parkourFail.weeklyLikes());
console.log(corgiFail.weeklyLikes());
```

### Fill in the Blank

1. An entity that stores data in properties and encapsulates behaviors in methods is referred to as an ________________.

2. To ________________ is to create an instance by defining one particular variation of object within a class.

3. to _________________ a property means memory is allocated for the variable, such as when it is declared.

4. A *string object* is known as a  __________________ and its properties and methods can be used on any value that is a string.

5. Each character in a string is automaically given an ________________, starting from 0.

6. JavaScripts 5 simple or primitive data types are:  
_____________  
_____________  
_____________  
_____________  
_____________  

7. An _____________ is a whole number (not a fraction).

8. A ______________ is a number that uses decimals to represent a fraction.

9. A function created at the top level of a script is considered in the ______________.


**Terms**

object-oriented model  
initialize  
instantiate  
wrapper object  
index number  
string  
boolean  
number  
undefined  
null  
interger  
floating point number  
global scope  
