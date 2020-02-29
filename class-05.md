# Earthdate 28022020

## HTML&CSS Chapter 5

### Images

* If you are creating a site from scratch it is good practice to create a directory for all of the site's images  
* To add an image to a page use the **<img>** element, which is an **empty element**  
    * the *<img>* element requires a **src** attribute to link to the image URL  
    * an **alt** attribute is required to provide a text description of the image when it can't be seen  
    * you can also include a **title** attribute to provide additional information  
    * the **height** and **width** of an image can also be specified in HTML, though it is best practice to use CSS to style images

#### Placing an Image

* Examples of image placement:
    * Before the paragraph - the paragraph starts on a new line after the image  
    * Inside the paragraph - the first row of text aligns with the bottom of the image  
    * In the middle of the paragraph - the image is placed between the words of the paragraph that it appears in  

*Old code: the **align** attribute used to indicate how the other parts of a page should flow around an image. The attribute takes horizontal values of **left** or **right**, and vertical values of **top**, **middle**, or **bottom**.*  

#### Creating Images

1. Save images in the right format - typically *.jpg*, *.png*, or *.gif*  
2. Save images at the right size - save the image at the same size it will appear on the site  
3. Measure images in pixels - this is the sizing that will translate most directly to a computer screen

#### Tools

* Software:  
    * Adobe Photoshop  
    * Adobe Fireworks  
    * Pixelmator  
    * PaintShop Pro  
    * Paint.net  

* Online Editors:  
    * www.photoshop.com  
    * www.pixlr.com
    * www.splashup.com
    * www.ipiccy.com  

* **JPEG** - use whenever you have many different colors in a picture  
* **GIF** and **PNG** - use when saving images with few colors or large areas of the same color  
* **Vector Images** differ from bitmap images and are resolution-independent; they are commonly created in programs such as Adobe Illustrator  
* Animated GIFs show several frames of an image in sequence to create simple animations  
* Images often come with captions. A **<figure>** element can contain and image and its caption - the **<figcaption>** element.  


## HTML&CSS Chapter 11

### Color

* The **color** property allows you to specify the color of text inside an element  
* **RGB Values** - these express colors in terms of how much red, green, and blue  
* **Hex Codes** - these are six digit codes that represent the amount of red, green, and blue in a color, preceded by a pound sign  
* **Color Names** - there are 147 predefined color names that are recognized by browsers  
* **background-color** sets the color behind the element  


## HTML&CSS Chapter 12

### Text

#### Typeface

* **Serif** - have extra details on the ends of the main strokes of the letters  
* **Sans-Serif** - have straight ends to letters  
* **Monospace** - every letter in font is the same width  
* **weight** - the font weight not only adds emphasis, but can also affectthe amount of whitespace and contrast on a page  
* **style** - *italic* fonts have a cursive aspect to some of the lettering and *oblique* font styles take the normal style and put it on an angle  
* **stretched** - in condensed versions of the font, letters are thinner and closer together - expanded versions are thicker and further apart  
* **font-family** - the user's computer needs the typeface installed. CSS is used to specify the typeface  
* **font-face** - CSS specifies where a font can be downloaded from if it is not installed on teh computer  
* service-based font-face - commercial services give users access to a wider range of fonts using @font-face  
* images - you can create a graphic that contains the text as you want it to appear in a different typeface  
* SIFR - the font is embedded into a Flash movie, and JavaScript replaces specified HTML text with a flash version of it  
* Cufon - The font is embedded into a Flash movie, and JavaScript replaces specified HTML text with a flash version of it  
* **font-size**  
    * **pixels** - are commonly used because they allow web designers very precise control over how much space their text takes up  
    * **percentages** - the default size of text in a browser is 16px or 100%  
    * **ems** - an em is equivalent to the width of a letter m  
* **@font-face** - allows you to use a font, even if it is not installed on the computer of the person browsing  
    * *font-family* specifies the name of the font  
    * *src* specifies the path to the font  
    * *format* specifies the format that the font is supplied in  
* the **text-transform** property is used to change the case of text giving it one of the following values:  
    * **uppercase** - causes the text to appear uppercase  
    * **lowercase** - causes the text to appear lowercase  
    * **capitalize** - causes the first letter of each word to appear capitalized  
* the **Text-decoration** property allows you to specify the following values:  
    * **none** - removes any decoration already applied to the text  
    * **underline** - adds a line underneath the text  
    * **overline** - adds a line over the top of text  
    * **line-through** - adds a line through words  
    * **blink** - animates the text to make it flash on and off  
* **line-height** or **leading** - the vertical space between lines of text  
* **letter-spacing** or **kerning** - the term for the space between each letter  
* **word-spacing** - the gaps between words  
* the **text-align** property allows you to control the alignment of text - can take one of four values: left, right, center, justify  
 * the **vertical-align** property is not intended to allow you to vertically align text in the middle of a block level element such as *<p>* or *<div>*. It is more commonly used with inline elements such as *<img>*, *<em>*, or *<strong>*  
 * the **text-indent** property allows you to indent the first line of text within an element
 * the **text-shadow** property is ise to create a drop shadow, which is a dark version of the word just behind it and slightly offset

 ```css
 p {
 text-shadow: 1px 1px 0px #000000;
 }
 ```

    * the first length indicates how far left or right the shadow should fall
    * the second value indicates the distance to the top or bottom that the shadow should fall
    * the third value is optional and specifies the amount of blur that should be applied to the drop shadow
* you can specifiy different values for the first letter or the first line of text inside an element using **:first-letter** and **:first-line**. These are not properties, but **pseudo-elements**
* in CSS, there are two **pseudo-classes** that allow you to set differnt styles for links that have and have not yet been visited:
    * **:link** - sets styles for links not yet visited
    * **:visited** - sets styles for links that have been visited
* **:hover** is applied when a user hovers over an element with a pointing device
* **:active** is applied when an element is being activated by a user, like a clicked button
* **:focus** is applied to an element having focus - any element you can click on or any form you can control