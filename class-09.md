#### Earthdate 04032020

# Forms, Lists, Tables, and Events

## Forms

###Form
* the form controls live inside this element  
  * **action** - a required element, it's value is the URL for the page on the server that will recieve the information in the form  
  * **method** - forms can be sent using one of two:  
    * **get**  
    * **post**  
* the **input** element is used to create several different form controls  
  * **type="text"** creates a single text line input  
    * **name** allows the server to identify and type the contents of the text box  
    * **maxlength** limits the number of characters a user may enter  
  * **type="radio"** allow users to pick just one of a number of options  
    * **name** is sent to the server with the value of the option the user selects  
    * **value** indicates the value that is sent to the server from the selected option  
    * **checked** can be used to indicate which value (if any) should be selected when the page loads  
  * **type="checkbox"** allow users to select one or more options  
    * **name** is sent to the server with the value of the checkbox(es) the user selects  
    * **value** indicates the value sent to the server  
    * **checked** indicates that this box should be checked when the page loads  
  * **type="file"** creates a box that looks like text input followed by a *browse* button which allows users to upload a file  
  * **type="submit"** sends a form to the server  
    * it can use a **name** attribute but does not need one  
    * the **value** attribute is used to control the text that appears on a button   
  * **type="image"** allows you to use an image for a submit button 
  * **type="hidden"** allows web page authors to add values to forms that users cannot see   
  * **type="date"** creates a date input  
  * **type="email"** asks a user for an email address  
  * **type="url"** can be used when you are asking a user for a web page address  
  * **type="search"** creates a single line text box for search queries  
    * **placeholder** works on any text input and allows you to place placeholder text within the text field  
* **select** is used to create a drop down list box  
    * the **name** attribute indicates the name of the form control being sent to the server  
  * the **option** element is used to specify the options that the user can select from  
    * the **value** attribute indicates the value that is sent to the server  
    * **selected** can be used to indicate the option that should be selected when the page loads  
    * **size** turns a drop down box into a box that shows more than one option  
    * **multiple** allows users to select multiple options from the list  
* the **button** element was introduced to allow users more control over how their buttons appear and to allow other elements to appear inside the button  
* **label** makes a form accessible to vision-impaired users  
  * **for** states which form control the label belongs to  
* **fieldset** groups related form controls together  
  * **legend** contains a caption which helps identify the purpose of that group of form controls  


## Lists

* the **list-style-type** property allows you to control the shape or style of a bullet point  
* the **list-style-image** property specifies an image to act as a bullet point, starting with a UTL  
* the **list-style-position** property decides the indent of a list  
  * **outside** - the marker sits to the left of the block text  
  * **inside** - the marker sits inside the block text  
* the **list-style** property is a shorthand for list styles  


## Table Properties

* width - sets the width of the table  
* padding - adds space around cell content  
* text-transform - converts text to uppercase  
* letter-spacing, font-size - adds size or space to letters  
* border-top, border-bottom - adds space around top and bottom of cells  
* text-align - aligns cell content left, right, center, or justified  
* background-color - change background color of specific cells  
* :hover - create hover effect over specified content  
* **border-spacing** controls the distance between adjacent cells  
  * **ollapse** collapses borders to a single border where possible  
  * **separate** detaches borders from each other  

#### Cursor

The cursor property allows you to control the type of mouse cursor that should be displayed  

- auto
- crosshair
- default
- pointer
- move
- text
- wait
- help
- url("cursor.gif");


## Events Definition Match

##### Definitions

1. Web page has finished loading
2. Web page is unloading
3. Browser encounters a JavaScript error or an asset doesn't exist
4. Browser window has been resized
5. User has scrolled up or down the page
6. User first presses a key
7. User releases a key
8. Character is being inserted (repeats while key is depressed)
9. User presses and releases a button over the same element
10. User presses and releases the button twice over the same element
11. User presses a mouse button while over an element
12. User releases a mouse button while over an element
13. User moves the mouse (not on a touchscreen)
14. User moves the mouse over an element (not on a touchscreen)
15. User moves the mouse off an element (not on a touchscreen)
16. Element gains focus
17. Element loses focus
18. Value in any input or textarea element has changed
19. Value in select box, checkbox, or radio button changes
20. User submits a form (using a button or key)
21. User clicks on a form's reset button
22. User cuts content from a form field
23. User copies content from a form field
24. User pastes content into a form field
25. User selects some text in a form field
26. Change has been made to document
27. Node has been inserted as a direct child of another node
28. Node has been removed from another node
29. Node has been inserted as a descendant of another node
30. Node has been removed as a descendant of another node


##### Terms

- focus / focusin
- select
- click
- dblclick
- DOMNodeInserted
- submit
- reset
- cut
- DOMNodeRemovedFromDocument
- input
- change
- mousedown
- mouseup
- DOMNodeInsertedIntoDocument
- mouseout
- keydown
- unload
- copy
- mouseover
- paste
- DOMNodeRemoved
- error
- resize
- mousemove
- blur / focusout
- DOMSubtreeModified
- keyup
- keypress
- load
- scroll