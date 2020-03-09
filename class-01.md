#### Earthdate 25022020
# HTML Chapter 1
## Structural Markup
The elements that you can use to describe both headings and paragraphs
-	**headings** (h1, h2, h3, h4, h5, h6) – main headings down to 5 levels of subheadings  
-	**paragraphs** (<p></p>) – to create a paragraph, surround with open and closing tags  
-	**bold** (<b></b>)  
-	**Italic** (<i></i>)  
-	**Superscript** (<sup></sup>)  
-	**Subscript** (<sub></sub>)  
-	**White space collapsing** - when a browser comes across two or more spaces next to each other of a line break it treats it as only one space  
-	**Line breaks** (<br />) – to add a line break within a paragraph without creating a new division  
-	**Horizontal Rules** (<hr />) – to create a break between themes such as a change of topic in a book or a new scene in a play  

## Semantic Markup
Provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, etc.
-	**<strong></strong>** - indicates that its content has strong importance  
-	**<em></em>** - indicates emphasis that subtly changes the meaning of a sentence  
-	**<blockquote></blockquote>** - used for longer quotes that take up an entire paragraph  
-	**<q></q>** - used for shorter quotes that sit within a paragraph  
-	**<abbr></abbr>** - if you use an abbreviation or an acronym this tag will pop-up a small window on hover  
-	**<cite></cite>** - When you’re referencing a piece of work such as a book, film, or research paper  
-	**<dfn></dfn>** - used to indicate the defining instance of a new term
-	**<address></address>** - contains contact details for the author of a page
-	**<ins></ins>** - used to show content that has been inserted into a document
-	**<del></del>** - can show text that has been deleted from a document
-	**<s></s>** - indicates something that is no long accurate or relevant (but that should not be deleted)

# HTML Chapter 8
## CSS
# p {
# font-family: Arial;}
*p* is the **selector**  
*font-family: Arial* is the **declaration**  
*font-family* is the **property**  
*Arial* is the **value**  

## CSS Selectors
**Universal Selector** - * {}  
**Type Selector** - h1, h2, h3 {}  
**Class Selector** - .note {}  
**ID Selector** - #introduction {}  
**Child Selector** - li > a {}  
**Descendant Selector** - p a {}  
**Adjacent Sibling Selector** - h1+p {}  
**General Sibling Selector** - h1~p {}  

# HTML Chapter 17
## Semantic HTML
**<header>** and **<footer>** - the main header and footer that appears at the top or bottom of every page or a header or footer for an individual *<article>* or *<section>* within the page  
**<nav>** - used to contain the major navigational blocks on the site such as the primary site navigation  
**<article>** - acts as a container for any section of a page that could stand alone and potentially be syndicated  
**<aside>** - when used inside an *<article>* element, it should contain information that is related to the article but not essential to its meaning. When used outside of an *<article>* element, it acts as a container for content that is related to the entire page  
**<section>** - groups related content together, and typically each has its own heading  
**<hgroup>** - the purpose of heading groups is to group together a set of one or more *<h1>* through *<h6>* elements so that they are treated as one single heading  
**<figure>** and **<figcaption>** - can be used to contain content that is referenced from the main flow of an article (not just images). The *<figure>* element should always contain a *<figcaption>* element which provides a text description for the content of the *<figure>* element  
**<div>** - use where there is no suitable element to group a set of elements  

# HTML Chapter 18
-	Each website should be design for the target audience
-	Even if the site has wide appeal, you can still think about the demographics of a sample of the target audience
-	Invent some fictional visitors from your typical target audience
-	They can influence design decisions from color palettes to level of detail in descriptions
-	Now that you know who your visitors are, you need to consider **why** they are coming
o	Are they looking for general entertainment or do they need to achieve a specific goal?
o	If there is a specific goal, is it a personal or professional one?
o	Do they see spending time on this activity as essential or a luxury?
-	First, you want to create a list of reasons why people would be coming to your site
-	Now you need to work out what information they need in order to achieve their goals quickly and effectively
-	You can prioritize levels of information from key points down to non-essential or background information
-	Working out how often people are likely to revisit your site gives you an indication for how often you should update it
-	It can often be helpful to set up a schedule for when to update your site
-	The aim is to create a diagram of the pages that will be used to structure the site, known as a **site map**
-	**card sorting** - involves placing each piece of information that a visitor might need to know on a separate piece of paper and then organizing the related information groups
-	A site map will usually begin with the homepage
-	**wireframe** - a simple sketch of the key information that needs to go on each page of a site
-	**visual hierarchy** - helps users focus on the key messages that will draw people’s attention, and then guide them to subsequent messages
### Designing Navigation
-	Concise – navigation should be quick and easy to read. No more than 8 links in a menu is a good idea
-	Clear – users should be able to predict the kind of information that they will find on the page before clicking the link
-	Selective – the primary navigation should only reflect the selections or content of the site
-	Context – lets the user know where they are in the website at that moment
-	Interactive – each link should be big enough to click on and the appearance of the link should change when the user hovers over each item or clicks on it
-	Consistent – it is best to keep primary navigation exactly the same, particularly as sites become larger

# JavaScript Chapter 1
A **script** is a series of instructions that a computer can follow to achieve a goal, like a recipe, a handbook, or a manual. To write a script, you first need to state your goal and then list the tasks that need to be completed in order to achieve it.  
Start with the big picture of what you want to achieve, and break them down into smaller steps.
1. **Define the goal** – first, define the task you want to achieve
2. **Design the script** – split the goal out into a series of tasks. One may try representing them with a flow chart.
3. **Code each step** – each step must be written in JavaScript

### Objects & Properties
**Objects (Things)** - in computer programming, each physical thing in the world can be represented as an **object**.  Each object can have its own **properties**, **events**, and **methods**.  
**Properties (Characteristics)** - each property has a **name** and a **value**, and each of these name/value pairs tells you something about each individual instance of the object

## Events
Programs are designed to do different things when users interact with the computer in different ways. An **event** is the computers wat of sticking up its hand to say, “Hey, this just happened!” When an event happens, it can be used to trigger specific sections of the code.

## Methods
**Methods** typically represent how people or other things interact with an object in the real world. The code for a method can contain lots of instructions that together represent one task.  

**Web browsers are programs built using objects** The **Window Object** is representing by the browser. The **Document Object** models the current webpage loaded into each window.

## HTML, CSS, JavaScript
Web pages are most commonly broken down into three primary languages – HTML, CSS, and JavaScript. HTML is where the content of a page lives. It gives the page structure and adds semantics. CSS is the presentation layer, enhancing and styling the HTML elements. JavaScript is the behavior layer, adding interactivity and other dynamic features.

## Objects & Methods
# Document.write(‘Good afternoon!’);
*Document* is known as the **object**. The document object represents the entire webpage. The *write()* **method** of the document object allows new content to be written into the page where the *script* element sits. The dot between *document* and *write* is known as a **member operand**. **Objects** have several **methods** which can be accessed by placing this dot between the object and the method. Each piece of information inside the parentheses of the method is called a **parameter**.
