# what is css?

- CSS stands for Cascading Style Sheets
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media
- CSS saves a lot of work. It can control the layout of multiple web pages all at once
- External stylesheets are stored in CSS files

# why use CSS?

- styling
- layout & Design
- Animation
- Font changes
- organization
- grid system

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

  #CSS [attribute] Selector

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

# command

```bash
***CSS comments***

/**/#is a multi line command
//#is a single line command


***CSS Background Color***
#RGB,HEX,HSL is a color format

background-color:Tomato;#bg-color is tomato

***CSS Text Color***

color:red;#font-color is red


***CSS Border****

border:2px;#border is a line

***RGB Value RED,GREEN,BLUE***

color:rgb(255, 0, 0);#redcolor is rgb value

***RGBA Value RED,GREEN,BLUE,ALBHA***

color:rgba(255, 99, 71, 0.8);

***HEX Vale***

background-color:#ff0000;

***HSL***

background-color:hsl(0, 100%, 50%);

***CSS Background***

background-color:red;#rgb,rgba,hsl colors
opacity:0.5;#light color
background-image:url();#image bg
background-repeat:repeat; no-repeat,repeat-x,space,initialinherit
background-attachment:fixed; scroll
background-position:; left top,left center,left bottom,right top,right center,right bottom,center top,center center,center bottom

background (shorthand property): background: #ffffff url("img_tree.png") no-repeat right top;


***CSS Border***

border-style:;
dotted - Defines a dotted border
dashed - Defines a dashed border
solid - Defines a solid border
double - Defines a double border
groove - Defines a 3D grooved border. The effect depends on the border-color value
ridge - Defines a 3D ridged border. The effect depends on the border-color value
inset - Defines a 3D inset border. The effect depends on the border-color value
outset - Defines a 3D outset border. The effect depends on the border-color value
none - Defines no border
hidden - Defines a hidden border

border-width:;#n px, pt, cm, em, etc
border-color:;#border color
border: 5px solid red;#width,syle,color
border-radius:;#px,cm,em


***CSS Margin***

margin-top:;
margin-right:;
margin-bottom:;
margin-left:;
margin:;

***CSS Padding***

padding-top:;
padding-right:;
padding-bottom:;
padding-left:;
padding:;

***CSS Height Width***

height:;,auto,length,%,initial,inherit
width:;
max-height:;
min-height:;
max-width:;
min-width:;


***OUTline***

outline-style:;dotted,etc...
outline-color:;#outline color
outline-width:;thin,medium,thick,px,em
outline-offset: 15px;
outline:;
outline: 5px solid yellow;

***Text color***

color:;
text-align:;
text-align-last:;
direction:rtl;
unicode-bidi:bidi-override;
vertical-align:;baseline,text-top,text-bottom,sub,super
text-decoration-line:;
text-decoration-color:;
text-decoration-style:;
text-decoration-thickness:;
text-decoration:;
text-transform:;
text-indent:;
letter-spacing:;
line-height:;
word-spacing:;
white-space:;
text-shadow:;


***Font***

font-family:;
font-style :;
font-weight:;
font-variant:;
font-size:;
 font: 20px Arial, sans-serif;


border: 2px solid;#border
outline: 2px solid;#borderoutline
background-size:;#auto, contain, and cover
background-color:;#background-color
background-image: url("images/tile.png");#bg-img
background-repeat:;#repeat,repeat-x,repeat-y,no-repeat
background-attachment:;#fixed,
background-clip:;#border-box, padding-box, content-box
background-position:;#left top,top,right,left,center,righttop
background-origin:;# border-box, padding-box, content-box.
text-align: center;#text alignment
font-size: 18px;#fontsize

font-family:;#serif, sans-serif,
font-style:;#normal, italic or oblique
font-weight:;#normal, bold, bolder, lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900 and inherit.
font-size:56px;#sizefont
font-variant:;# capital letters, in which lowercase letters
text-transform: uppercase;#textchaned
*#all element
#->#id element
. #class select
text-decoration: none;#text underline none
text-overflow :;# clip and ellipsis and string.
text-align:;# left, right, centre or justified
text-decoration:;# underline, overline, line-through, and none
text-transform:;#uppercase or lowercase letters, or capitalize
text-indent:;#percentage (%), length values in pixels, ems, etc.
line-height:;#percentage (%), length values in pixels, ems, etc.
letter-spacing:;#percentage (%), length values in pixels, ems, etc.
word-spacing:;#percentage (%), length values in pixels, ems, etc.
box-shadow: offset-x offset-y blur-radius color;
a:link #define styles for normal or unvisited links.
a:visited #define styles for links that the user has already visited.
a:hover # define styles for a link when the user place the mouse pointer over it.
a:active #define styles for links when they are being clicked.

list-style-type:;#letters, circle, square,
list-style-position:;# inside.outside
list-style-image:;#list img

border-style:;#none, hidden, solid, dashed, dotted, double, inset, outset, groove, and ridge
 border-width:;
 border-color:;
 border-radius:;
 border-img:;
 outline-style:;#border-outside line ,ex: none, solid, dashed, dotted, double, inset, outset, groove, and ridge
 outline-width:;
 outline-color:;
border-collapse:;#collapse
border-spacing: 10px;
height:;
width:;

Flexbox Container Properties

display:flex;
flex-direction: row | row-reverse | column | column-reverse;

flex-wrap:nowrao|wrap|wrap-reverse;
justify-contents:flex-star|center|flex-end|sapce-between|sapce-around;

align-items:flex-star|center|flex-end|sapce-between|sapce-around;

align-contents:flex-star|center|flex-end|sapce-between|sapce-around;

flex-grow: 1;
flex-wrap: wrap;
 flex-shrink: 1;

margin-top:;
margin-right:;
margin-bottom:;
margin-left:;
 vertical-align:;#

 tbody tr:nth-child(odd) {
    background-color: #f2f2f2;
}#odd no color change

overflow-x: auto;#table response

padding:;#padding-top,padding-right

width: 300px;
height: 200px;
padding: 15px; /* set padding for all four sides */
border: 10px solid black; /* set border for all four sides */
margin: 20px auto; /* set top and bottom margin to 20 pixels, and left and right margin to auto */

min-width: 300px;
max-width: 500px;
  opacity: 0.7;#image bg light

cursor:;#mouse to assign to chnge the cursor
cursor: 	[url(address of cursor file),]0 or more times | auto | default | none | context-menu | help | pointer | progress | wait | cell | crosshair | text | vertical-text | alias | copy | move | no-drop | not-allowed | grab | grabbing | e-resize | n-resize | ne-resize | nw-resize | s-resize | se-resize | sw-resize | w-resize | ew-resize | ns-resize | nesw-resize | nwse-resize | col-resize | row-resize | all-scroll | zoom-in | zoom-out | initial | inherit


overflow-x and overflow-y :;#visible (default), hidden, scroll


display:;#block,inline,inline-block,none
position:;#top or bottom and/or left or right.absoluate,fixed,relative
z-index :;
float:;#left,right,none




 visibility :;#visible,hidden,collapse,inherit

linear-gradient(direction, color-stop1, color-stop2, ...)#Double colcor
linear-gradient(angle, color-stop1, color-stop2, ...)
radial-gradient(shape size at position, color-stop1, color-stop2, ...);
radial-gradient()#closest-side, farthest-side, closest-corner, farthest-corner.
```
