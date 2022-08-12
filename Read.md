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

- Descendant Selector
  ul li{}

- Child Selector
  div>p{}

- Attribute Selector
  input[type="text"]{}

- Grouping Selector
  h1,h2,h3{}

- Adjacent Sibling Selectors
  h1+p{}

- General Sibling Selectors
  h1~p{}

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

  - CSS [attribute] Selector
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

### CSS3 Examples

# CSS Text

```bash
Setting the text color ==> color: blue;#text color,HEX,RGB,
Alignment of text ==> text-align: center;#justify
Indentation of text ==> text-indent: 100px;
Decoration of text ==> text-decoration:overline;#line-through,underline
Sets the spacing between characters ==> letter-spacing: -3px;
Sets the spacing between words ==> word-spacing: 20px;
Sets the spacing between lines of text ==> line-height: 1.2;
Preserving white-space and line breaks ==>			white-space: pre;# nowrap
Text wrapping inside an element ==> word-wrap: break-word;
Vertical alignment of an image inside text==>  vertical-align: top;#middle,baseline

# CSS Fonts

Sets the font of a text==> font-family: Arial, Helvetica, sans-serif;
Sets the size of the font==>font-size: 14px;
Sets the style of the font==>font-style: normal;#italic,oblique
Sets the variant of the font==>font-variant: small-caps;
Sets the boldness of the font==>font-weight: normal;#bold
Setting the all font properties in a single declaration - The font shorthand property ==>font: bold 2.5em "Times New Roman", Times, serif;

# CSS Links

Style different states of a link==>  a:link,    a:visited , a:hover ,a:active
Remove the default underline from hyperlinks==>text-decoration: none;#underline
Customize a link to look like a button==>
Create image rollover effect==>

# CSS Lists

Specify bullets and numbering in the lists==>  list-style-type: square;#upper-roman
Sets the position of list-item markers==>  ol.in li {
                                                    list-style-position: inside;
                                                     }
    ol.out li {
        list-style-position: outside;
    }
Sets an image as list-item markers==>list-style-image: url("/examples/images/bullet.png");
Setting all list properties in a single declaration - The list-style shorthand property==>list-style: circle inside;
Crating a simple navigation menus with lists==>
Crating a simple dropdown menu using lists==>

# CSS Tables

Setting the borders of a table==>	border-collapse: collapse;,border: 1px solid #000000;
Specify the dimension of a table==>
Creating better tables by collapsing the table borders==>
Setting the horizontal alignment of text inside table cell==>text-align: left;
Setting the vertical alignment of content==> vertical-align: bottom;
Specify how empty cells should be displayed==>empty-cells: show;
Specify padding of table cell==> padding: 10px;
Specify table layout algorithm - Automatic or Fixed==>table-layout: auto;#fixed
Setting the position of table caption==>caption-side: bottom;

# CSS Background

Setting the background color of an elementc==> background-color: #f0e68c;
Setting the image as elements background==> background-image: url("/examples/images/tile.png");
Repeating background image horizontally or vertically==>        background-repeat: repeat-x;
Specify the positioning of background image==> background-position: center;

A fixed background image that will not scroll with its containing element==>background-attachment: fixed;
Setting the all background properties at once - The background shorthand property==>background: #f0e68c url("/examples/images/smiley.png") no-repeat fixed 250px 25px;
Setting the size of the background image==>
Setting the background clipping==>background-clip: border-box;
Setting the background origin==> background-origin: content-box;
Adding multiple backgrounds to an element==>

# CSS Units

Working with absolute units (e.g. px, pt, cm etc.)==>
Working with relative units (e.g. em, ex, % etc.)==>

# CSS Dimension

Setting width and height of an element==>width: 300px;,height: 00px;
Setting maximum width and height of an element==>max-width: 400px;
			max-height: 50px;
Setting minimum width and height of an element==>	min-width: 300px;
			min-height: 100px;
Controlling overflow of content==>overflow: scroll;#fidden

# CSS Alignment

Alignment of text and inline element inside the block-level element==>
Center alignment of block element using margin property==>
Aligning element horizontally using the float property==>float: left;
Aligning element horizontally and vertically using the position property==>top:0;,bottom:0;
Prevent parent collapsing with the clear property==>clear: both;
        visibility: hidden;
Creating a Simple horizontal menu==>

# CSS Positioning

Position an element relative to the browser window==>position: reative;
Position an element relative to its parent element==> position: absolute;,position:relative;
Position an element relative to its normal position==>
Overlapping of elements using the z-index property==> z-index: 1;

# CSS Display

Hide an element using the visibility property==>  visibility:hidden;
Remove an element from DOM using the display property==> display:none;

Display an element as an inline element==> display: inline;
Display an element as a block element==> display: block;
Collapsing table elements==>

# CSS Border and Outlines

Draw border around element==>border-style: solid;
        border-width: 5px;
        border-color: #000000;
Draw border on the individual sides of an element==>border-top:;
Setting different styles for the borders==> border-style: none;
Setting the all border properties at once - The border shorthand property==>border: 5px solid #ff0000;
Creating the rounded corners around an element==>
Using images for creating borders==>border-image: url("/examples/images/border.png") 30 30 round;
Draw outline around element==>	outline: 5px solid #ff0000;
Draw border around element without effecting the surrounding elements==>

# CSS Margin and Padding

Sets the margins for individual sides of an element==> margin-top: 50px;
        margin-bottom: 100px;
        background: yellow;
Setting all margin properties in a single declaration - The margin shorthand property==>        margin: 25px;
Sets the paddings for individual sides of an element==>padding-top: 50px;
        padding-bottom: 100px;
        background: lime;
Setting all padding properties at once - The padding shorthand property==>pdding:;

# CSS Opacity

Setting transparency of an element==>opacity: 0.7;
Image rollover effect and transparency==> opacity: 0.5;
        display: block;
        filter: alpha(opacity=50); /* to work in IE */
Text in a transparent box==>



# CSS Pseudo-classes

Setting styles for different states of hyperlinks==>
Setting styles for form element in focus using the :focus pseudo-class==>a:focus {
        color: yellow;
    }
Setting the styles for first child of an element using the :first-child pseudo-class==>
Setting styles for last child of an element using the :first-child pseudo-class==>
Setting styles for nth-child of an element using the :nth-child pseudo-class==>
Setting styles for specific language using the :lang() pseudo-class==>
Using pseudo-classes with selectors==>

# CSS Pseudo-elements

Creating the drop cap effect using the ::first-letter pseudo-element==>
Styling the first line of a text differently using the ::first-line pseudo-element==>
Insert some content before and/or after an element using the ::before and/or ::after pseudo-element==>
Using pseudo-elements with classes==>

# CSS3 Gradients

Creating linear gradients from top to bottom direction==>
Creating linear gradients from left to right direction==>
Creating linear gradients along the diagonal==>
Setting the direction of linear gradients using angles==>
Creating linear gradients using multiple color stops==>
Setting the location of color stops while creating the gradients==>
Repeating the linear gradients==>
Creating radial gradients==>
Setting the shape of radial gradients==>
Setting the size of radial gradients==>
Repeating the radial gradients==>
Using transparency with gradients==>

# CSS3 Drop Shadows

Creating box shadow effect==>
Adding multiple box shadows to an elements box==>
Creating text shadow effect==>

# CSS3 2D Transforms

Moving the elements using the translate() method==>
Rotating the elements using the rotate() method==>
Increasing or decreasing the size of an element using the scale() method==>
Applying 2D transformation using the matrix() method==>
Applying multiple transformation to an element==>

# CSS3 3D Transforms

Moving an element in three dimensional space using the translate3d() method==>
Rotating an element in three dimensional space using the rotate3d() method==>
Scaling an element in three dimensional space using the scale3d() method==>
Applying 3D transformation using the matrix3d() method==>
Applying multiple 3D transformation to an element==>

# CSS3 Transitions

Applying transition effect to background-color==>
Applying transition effect to multiple property==>
Setting all transition properties at once - The transition shorthand property==>

# CSS3 Animations

Animating elements on a web page==>
Defining keyframe while creating animations==>
Setting all animation properties at once - The animation shorthand property==>

# CSS3 Multi-column Layouts

Creating multi-column layouts==>
Setting column count or width==>
Setting gap between the columns==>
Adding rule or vertical lines between the columns==>

```

```

```
