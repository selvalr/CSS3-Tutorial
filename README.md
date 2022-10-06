# what is css?

- CSS stands for Cascading Style Sheets
- Not Programming Language
- Used for Styling
- Design purpose
- External stylesheets are stored in CSS files
- Continuation of HTML

# why use CSS?

- styling
- layout & Design
- Animation
- Font changes
- organization
- flex-box
- grid system

# Types Of Styles

1. Inline-Adding style in each line
2. Internal-style tags
3. External-Linking external CSS file



## CSS Syntex:

selecter {property:value}


# CSS RoadMap


## CSS Basic

1.Box model --->content,padding,border,margin

2.Selecter and,Combinators

3.border,margin,padding,and outline

4.border-radius

5.background

6.colors -->simple,gradient,alpha transpency

6.Text -->

7.fonts

7.Icons

8.display -->block,inline,inline-block,etc..

9.position -->static,relative,absoulate,fixed,sticky

10.dimenation -->top,left,height,width,max-width,aspect-ratio etc..

12.overflow --> visible,hidden,scroll,auto

13.z-index -->-1,1,2,3

---

**1.Box model**

Content - The content of the box, where text and images appear.  


Padding - Clears an area around the content. The padding is transparent.


Border - A border that goes around the padding and content.


Margin - Clears an area outside the border. The margin is transparent.

---

**2.Selecter & combinater**

simple selecter ==>p{} , .class{} , #id{} , *{} , h1,p,h2{},

***combinators***

1.Descendant Selector(space):

div p{all div tag inside elements p} 

2.Child Selecter(>):

 div>p{The child selector selects all elements}
 
3.Adjacent Sibiling Selecter(+):

 div + p{div block outside first element working}

4.General Sibiling Selecter(~):

 div ~ p{div block outside all p element working}

 ***Attribute selecter***
  
  *CSS [attribute] Selector*:

  [title] {
  color: blue;
  }

  abbr[title] {
  color: red;
  }

  input[type="submit"] {
  border: 1px solid green;
  }

  [class~="warning"] {
  color: #fff;
  background: red;
  }

  [lang|=en] {
  color: #fff;
  background: blue;
  }

  a[href^="http://"] {
  background: url("external.png") 100% 50% no-repeat;
  padding-right: 15px;
  }

  a[href$=".pdf"] {
  background: url("pdf.png") 0 50% no-repeat;
  padding-left: 20px;
  }

  [class*="warning"] {
  color: #fff;
  background: red;
  } #\*= operator to make an attribute selector matches all elements

---

**3.border,margin,padding,and outline**

border-style:;<br>
border-width:;<br>
border-color:;<br>
border-left:;<br>
<br>
margin-top:;<br>
margin-right:;<br>
margin-bottom:<br>
margin-left:;<br>
<br>
padding-top:;<br>
padding-right:<br>
padding-bottom;<br>
padding-left:;<br>
<br>
outline-style:<br>
outline-color:<br>
outline-width:<br>
outline-offset;<br>
outline:;<br>

---

**4.border-radius**

border-radius:;

---

**5.bacground**

background-color:;

background-image:;

background-repeat:;

background-attachment:;

background-position:;

background (shorthand property):;

---

**6.colors**

color:;,RGB(0,0,0);,Hex,hsl

---

**6.Text**

***text alignment***

text-align:;

text-align-last:;

direction:;

unicode-bidi:;

vertical-align:;

***text Decoration***

text-decoration-line:;

text-decoration-color:;

text-decoration-style:;

text-decoration-thickness:;

text-decoration:;

***text transform***

text-transform:;

***text spacing***

text-indent:;

letter-spacing:;

line-height:;

word-spacing:;

white-space:;

***text shadow***

text-shadow:;

---

**7.fonts**
 
 font-family:;

 font-style:;

 font-size;

 font-weight:;

 font-variant:;

---

**7.Icons**
```
<script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>

<i class="fas fa-cloud"></i>

<i class="fas fa-heart"></i>
```

---


**8.display**

display:;#inline,block,none,inline-block

visibility:;#hidden

---

**9.position**

position:;#static,relative,fixed,absolute,sticky

---

**10.dimenation**

height:;#px not response,% is res in height,width

width:;

min-height:;

max-height:;

---

**11.float**

float:;#left,right,none,inherit

clear:;

---

**12.overflow**

overflow:;#visible,hidden,scroll,auto

---

**13.z-index**

b78- The z-index property specifies the stack order of an element.

z-index:;#-1,1,2,..

---

**14.Counters**

- counter-reset - Creates or resets a counter

- counter-increment - Increments a counter value

- content - Inserts generated content

- counter() or counters() function - Adds the value of a counter to an element

---

**CSS Medium**

1.Specificity

2.pseudo classes,elements

3.opacity

4.filter

5.clip-path

6.mask

7.transform

8.media

9.flexbox

10.grid

11.animation

---

**1.Specificity**

  - Inline styles - Example: `<h1 style="color: pink;"></h1>`
  
  - Header style - Example: <style>*{color:"red"};</style>
  
  - external style - Example:`<link rel="stylesheet" href=style.css>`
  
  - ID  - Example: #idName
  
  - Classes, pseudo-classes, attribute selectors - Example: .test, :hover, [href]
  
  - Elements and pseudo-elements - Example: h1, :before

***first runnuning is inline css next id and next class and next tag:***
  .test {color: green;}

  p {color: red;}

  <p id="demo" class="test" style="color: pink;">Hello World!</p>

 .test {color: green;}

  p {color: red;}

  <p class="test">Hello World!</p>//output is:green color

 #demo {color: blue;}

    .test {color: green;}

    p {color: red;}

    <p id="demo" class="test">Hello World!</p>//output:blue color is running first


---

**2.pseudo classes, elements**

*Pseudo Class:*

`
syntex:
        selector:pseudo-class {
                         property: value;
                            }
                            `
  - Anchor Pseudo-classes --->  a:link{},a:visited{},a:hover{},a:active{}

  - Pseudo-classes and HTML Classes  --->  a.classname:hover {}

  - Hover on <div> ---> div:hover{}

  - CSS - The :first-child Pseudo-class ---> p:first-child{}


*Pesudo-Elemet:*

`
syntex:
      selector::pseudo-element {
                                property: value;
                              }
`
  - The ::first-line Pseudo-element ---> p::first-line {}
  
  - The ::first-letter Pseudo-element ---> p::first-letter {}
  
  - Pseudo-elements and HTML Classes ---> p.intro::first-letter {}
  
  - CSS - The ::before Pseudo-element ---> h1::before {}
  
  - CSS - The ::after Pseudo-element ---> h1::after {}
  
  - CSS - The ::marker Pseudo-element ---> ::marker {}
  
  - CSS - The ::selection Pseudo-element ---> ::selection {}

---

**3.opacity**

img {
  opacity: 0.5;
}

---

**4.filter**

filter: none | blur() | brightness() | contrast() | drop-shadow() | grayscale() | hue-rotate() | invert() | opacity() | saturate() | sepia() | url();


filter:;#drop-shadow(8px 8px 10px gray);,none;,blur(5px),brightness(200%);, grayscale(100%);,etc...

---

**5.Clip path**

clip: clip-source|basic-shape|margin-box|border-box|padding-box|content-box|fill-box|stroke-box|view-box|none|initial|inherit;

clip:;

---

**6.Mask**

mask-image:; = Specifies an image to be used as a mask layer for an element

mask-mode:;	Specifies whether the mask layer image is treated as a luminance mask or as an alpha mask

mask-origin:;	Specifies the origin position (the mask position area) of a mask layer image

mask-position:;	Sets the starting position of a mask layer image (relative to the mask position area)

mask-repeat:;	Specifies how the mask layer image is repeated

mask-size:;	Specifies the size of a mask layer image

---

**7.transform**

***2D Transform***

syntex:

transform: none|transform-functions|initial|inherit;

properties:

transform:;none,rotate(10deg);, rotateX(45deg);, rotateY(45deg);, skew(20deg,20deg);, skewX(30deg);,translate(20px,10px);,scale(2,2);matrix(0.866,0.7,-0.8,0.866,0,0);,

***3D Transform***

syntex:
With the CSS transform property you can use the following 3D transformation methods:

rotateX()
rotateY()
rotateZ()

---

**8.media**

CSS Syntax:
`
@media not|only mediatype and (mediafeature and|or|not mediafeature) {
  CSS-Code;
}`

---

**9.Flex Box Layout**

- flex stands for flexible,adaptive
- single diamension layout design.  example: row OR Cloumn only
display:flex;
- flexbox use to no the alternative for: display:block,display:inline,display:inline-block; not used flexbox


***flex-direction***
  - box direction in flexiable
  
flex-direction:; #column,row,column-reverse,row-reverse

***flex-wrap***
- the content wrap the box next line
  
flex-wrap:;#wrap,nowrap,wrap-reverse,

***flex-flow***
- shorthand in flex-direction & flex-wrap:


flex-flow:;flex-direction && flex-wrap two same the element

***justify-content***
- this content main x axis working alignment

justify-content:;#center,flex-start,flex-end,space-aroud,space-between

***align-content***
- this is a cross-axis alignment

align-content:;#space-between,space-around,stretch,center,flext-start,flex-end,

***align-items***
- The align-items property is used to align the flex items.


align-items:;#center,lex-start,flex-end,stretch,baseline


**The flex item properties are:**

***order***
- The order property specifies the order of the flex items.


order:;-->order change the box

***flex-grow***
- The flex-grow property specifies how much a flex item will grow relative to the rest of the flex items.



flex-grow:;1box in 2 box

***flex-Shrink***
- The flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items.


flex-shrink:;2box in 1box

***flexx-basis***
- The flex-basis property specifies the initial length of a flex item.
  

flex-basis:;

***flex***
- The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.


flex:; 

***align-self***
- The align-self property specifies the alignment for the selected item inside the flexible container.

- The align-self property overrides the default alignment set by the container's align-items property.

align-self:;#strech,flex-start,flex-end,center

---

**10.Grid Layout**

- Grid is a two diamensinal layout
- making it easier to design web pages without having to use floats and positioning.

***Grid-display***

display: grid;

display: inline-grid;

***gap***

column-gap:50px; --> The column-gap property sets the gap between the columns:

row-gap:50px; --> The row-gap property sets the gap between the rows:

gap:50px; --> The spaces between each column/row are called gaps.




**Property	Description**

***grid-shorthand***

grid:150px / auto auto auto; --->The grid property is a shorthand property for: 
                                                
                                                grid-template-rows
                                                grid-template-columns
                                                grid-template-areas
                                                grid-auto-rows
                                                grid-auto-columns
                                                grid-auto-flow



grid-auto-rows, grid-auto-columns, and the grid-auto-flow properties

***grid-area-shorthand***

grid-area: 2 / 1 / span 2 / span 3; 

--> Make "item1" start on row 2 column 1, and span 2 rows and 3 columns:
-->The grid-area property specifies a grid item's size and location in a grid layout, and is a shorthand property for the following properties:
                  grid-row-start
                  grid-column-start
                  grid-row-end
                  grid-column-end

***grid-auto-column***
- The grid-auto-columns property sets a size for the columns in a grid container.

- syntex:
  
  ` grid-auto-columns: auto|max-content|min-content|length;`

grid-auto-columns:;

***grid-auto-flow***
- The grid-auto-flow property controls how auto-placed items get inserted in the grid.

- syntex :
 
  `grid-auto-flow: row|column|dense|row dense|column dense;`

grid-auto-flow	:;

***grid-auto-rows***
- The grid-auto-rows property sets a size for the rows in a grid container.

- This property affects only rows with the size not set

- syntex :
  
  `grid-auto-rows: auto|max-content|min-content|length;`
  

grid-auto-rows:;

***grid-column***
- The grid-column property specifies a grid item's size and location in a grid layout, and is a shorthand property for the following properties:
- syntex :
  
  `grid-column: grid-column-start / grid-column-end;`
  

grid-column	:1/5; --> 1st line to 5 th line

***grid-column-start***
- The grid-column-start property defines on which column-line the item will start.

- syntex:
  
  `grid-column-start: auto|span n|column-line;`
  
grid-column-start:;

***grid-column-end***
- The grid-column-end property defines how many columns an item will span, or on which column-line the item will end (see example at the end of this page).

- syntex:
 
  `grid-column-end: auto|span n|column-line;`
  


grid-column-end:;--->column end line


***grid-column-gap***
- The grid-column-gap property defines the size of the gap between the columns in a grid layout.

- Note: This property was renamed to column-gap in CSS3. 

- syntex:
  
  `grid-column-gap: length;`
  
grid-column-gap:;


***grid-gap***
- The grid-gap property defines the size of the gap between the rows and columns in a grid layout, and is a shorthand property for the following properties:

- grid-row-gap
- grid-column-gap
- Note: This property was renamed to gap in CSS3.  


- syntex :
  
  `grid-gap: grid-row-gap grid-column-gap;`

grid-gap:;-->gap the content

***grid-row***
- The grid-row property specifies a grid item's size and location in a grid layout, and is a shorthand property for the following properties::

- grid-row-start
- grid-row-end

- syntex:
- grid-row: grid-row-start / grid-row-end;


grid-row:;

***grid-row-end***
- The grid-row-end property defines how many rows an item will span, or on which row-line the item will end (see example at the end of this page).


- syntex:
  
  `grid-row-end: auto|row-line|span n;`
  
grid-row-end:; -->row end of width line

***grid-row-gap***
- The grid-row-gap property defines the size of the gap between the rows in a grid layout.

- Note: This property was renamed to row-gap in CSS3

- syntex:
  
  `grid-row-gap: length;`


grid-row-gap:;--->row gap grid

***grid-row-start***
- The grid-row-start property defines on which row-line the item will start.

- syntex:
  
  `grid-row-start: auto|row-line;`


grid-row-start:;

***grid-template***
- The grid-template property is a shorthand property for the following properties:

grid-template-rows
grid-template-columns
grid-template-areas

- syntex:
  
  `grid-template: none|grid-template-rows / grid-template-columns|grid-template-areas|initial|inherit;`


grid-template:;

***grid-template-areas***
- The grid-template-areas property specifies areas within the grid layout.

- You can name grid items by using the grid-area property, and then reference to the name in the grid-template-areas property.

- Each area is defined by apostrophes. Use a period sign to refer to a grid item with no name.

- syntex:
  
  `grid-template-areas: none|itemnames;`


grid-template-areas:;

***grid-template-columns***
- The grid-template-columns property specifies the number (and the widths) of columns in a grid layout.

- The values are a space separated list, where each value specifies the size of the respective column

- syntex:
  
  `grid-template-columns: none|auto|max-content|min-content|length|initial|inherit;`


grid-template-columns:;


***grid-template-rows***
- The grid-template-rows property specifies the number (and the heights) of the rows in a grid layout.

- The values are a space-separated list, where each value specifies the height of the respective row
row-gap:;--->row gap

- syntex:
  
  `grid-template-rows: none|auto|max-content|min-content|length|initial|inherit;`

grid-template-rows:;


***justify-content***

justify-content:;--> The justify-content property is used to align the whole grid inside the container.

***align-content***

align-content:;--> The align-content property is used to vertically align the whole grid inside the container.

---

**10.CSS Animations**

@keyframes

animation-name

animation-duration

animation-delay

animation-iteration-count

animation-direction

animation-timing-function

animation-fill-mode

animation

---

**CSS Advanced**

1.Rounded Corner #border radius round corner

2.Border-Image # border image set

3.CSS Multiple Background #multiple bg-image set

4.CSS Gradients #gradient is a multiple color background

5.CSS Shadow #text and box shadows

6.Transitions



**1.Rounded-corner**

border-radius:;

border-top-left-radius:;

border-top-right-radius:;

border-bottom-right-radius:;

border-bottom-left-radius:;

---

**2.Border-image**

border-image:;

border-image-source:;
 
order-image-slice:;
  
border-image-width:;
   
border-image-outset:;
    
border-image-repeat:;

---

**3.CSS Multiple Background**
`
#example1 {
  background-image: url(img_flwr.gif), url(paper.gif);
  background-position: right bottom, left top;
  background-repeat: no-repeat, repeat;
}`

#CSS Background Size:

background-size:;#contain and cover,and height,width

background-origin:;#border-box,padding-box,content-box

background-clip:;#border-box,padding-box,content-box

---

**4.CSS Gradients**

- Linear Gradients (goes down/up/left/right/diagonally)
`example:
        #grad {
  background-image: linear-gradient(red, yellow);
}
`

- Radial Gradients (defined by their center)
`examle:
#grad {
  background-image: radial-gradient(red, yellow, green);
}`


- Conic Gradients (rotated around a center point)
`
example:
  #grad {
  background-image: conic-gradient(red, yellow, green);
}

`

---

**5.CSS Shadow**

*text shadow*
  
  ```
  h1 {
      text-shadow: 2px 2px 5px red;
      }
```
*box-shadow*

```
div.card {
  width: 250px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  text-align: center;
}
```

---

**6.Transitions**

- transition

- transition-delay:;#1s

- transition-duration:;#2s

- transition-property:;#width,height

- transition-timing-function:;#ease,linear,ease-in,ease-out,ease-in-out,cubic-bezier(n,n,n,n)

---



# css Selecter

- Element or Tag Selector
  h1{},p{},h2{}

- Id Selector
  #idname{}

- Class Selector
  .classname{}

- Universal Selector
  \*{

  }

- CSS Grouping Selector
  h1,h2,h3{}

- Attribute Selector
  input[type="text"]{}

#CSS Combinators selecter

- Descendant Selector
  ul li{}

- Adjacent Sibling Selectors
  h1+p{}

- Child Selector
  div>p{}

- General Sibling Selectors
  h1~p{}

  #Anchor Pseudo-classes

  - a:link{}
  - a:visited{}
  - a:hover{}
  - a:active{}

- firstchild pesudoclass
  ol li:first-child{}

- lastchild
  ul li:last-child {
  border-right: none;
  }

- The :nth-child Pseudo-class
  table tr:nth-child(2n) td {
  background: #eee;
  }

#Pseudo-Elements

- The ::first-line Pseudo-element
  p::first-line {
  color: #ff0000;
  font-variant: small-caps;
  }

- The ::first-letter Pseudo-element

p::first-letter {
color: #ff0000;
font-size: xx-large;
}

- The ::before and ::after Pseudo-element
  h1::before {
  content: url("images/marker-left.gif");
  }
  h1::after {
  content: url("images/marker-right.gif");
  }

 


# css cheetsheet

![css!](./roadmap-img/1.jpg "css cheetsheet")
![css!](./roadmap-img/2.jpg "css cheetsheet")
![css!](./roadmap-img/3.jpg "css cheetsheet")
![css!](./roadmap-img/4.jpg "css cheetsheet")
![css!](./roadmap-img/5.jpg "css cheetsheet")
![css!](./roadmap-img/6.jpg "css cheetsheet")
![css!](./roadmap-img/7.jpg "css cheetsheet")
![css!](./roadmap-img/8.jpg "css cheetsheet")
![css!](./roadmap-img/9.jpg "css cheetsheet")
![css!](./roadmap-img/10.jpg "css cheetsheet")
![css!](./roadmap-img/11.jpg "css cheetsheet")
![css!](./roadmap-img/12.jpg "css cheetsheet")
![css!](./roadmap-img/13.jpg "css cheetsheet")
![css!](./roadmap-img/14.jpg "css cheetsheet")
![css!](./roadmap-img/15.jpg "css cheetsheet")
![css!](./roadmap-img/16.jpg "css cheetsheet")
![css!](./roadmap-img/17.jpg "css cheetsheet")
![css!](./roadmap-img/18.jpg "css cheetsheet")
![css!](./roadmap-img/19.jpg "css cheetsheet")
![css!](./roadmap-img/20.jpg "css cheetsheet")

# css basic

![css!](./basic-css.jpg "css cheetsheet")
![css!](./css-center.jpg "css cheetsheet")
![css!](./flex-box-css.jpg "css cheetsheet")
![css!](./grid-css.jpg "css cheetsheet")

