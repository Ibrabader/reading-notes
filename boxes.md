# HTML Lists, Control Flow with JS, and the CSS Box Model

### LSITS : 
####  There are lots of occasions when we 
need to use lists. HTML provides us with 
three different types:
- Ordered lists are lists where each item in the list is 
numbered. For example, the list might be a set of steps for 
a recipe that must be performed in order, or a legal contract 
where each point needs to be identified by a section 
number.
- Unordered lists  are lists that begin with a bullet point 
(rather than characters that indicate order).
- Definition lists  are made up of a set of terms along with the 
definitions for each of those ter

1- `<ol>`

The ordered list is created with 
the `<ol>` element.
`<li>`
Each item in the list is placed 
between an opening `<li>` tag 
and a closing `</li>` tag. (The li 
stands for list item.)
Browsers indent lists by default.
Sometimes you may see a type 
attribute used with the `<ol>` 
element to specify the type of 
numbering (numbers, letters, 
roman numerals and so on). It 
is better to use the CSS list-
style-type property

2- `<ul>`

The unordered list is created 
with the `<ul>` element.
`<li>`
Each item in the list is placed 
between an opening `<li>` tag 
and a closing `</li>` tag. (The li 
stands for list item.)
Browsers indent lists by default.
Sometimes you may see a type 
attribute used with the `<ul>` 
element to specify the type of 
bullet point (circles, squares, 
diamonds and so on). It is better 
to use the CSS list-style

3- `<dl>`

The definition list is created with 
the `<dl>` element and usually 
consists of a series of terms and 
their definitions.
Inside the `<dl>` element you will 
usually see pairs of `<dt>` and 
`<dd>` elements.
`<dt>`This is used to contain the term 
being defined (the definition 
term).
`<dd>`This is used to contain the 
definition.
Sometimes you might see a list 
where there are two terms used 
for the same definition or two 
different definitions for the same 
term


### BOXES : 
- You can set several properties that affect the appearance of 
these boxes. In this chapter you will see how to:
Control the dimensions of your boxes ●
Create borders around boxes ●
Set margins and padding for boxes ●
Show and hide boxes ●
Once you have learned how to control the appearance of each 
box, you will see how to position these boxes on your pages in 
Chapter 15 when we look at page layout

#### Box Dimensions (width, height)
- The most popular ways to 
specify the size of a box are 
to use pixels, percentages, or 
ems. Traditionally, pixels have 
been the most popular method 
because they allow designers to 
accurately control their size.

**When you use percentages, 
the size of the box is relative to 
the size of the browser window**

**When you use ems, the size 
of the box is based on the size 
of text within it**

#### limiting WiDth min-width, max-width
- Some page designs expand and 
shrink to fit the size of the user's 
screen. In such designs, the 
min-width property specifies 
the smallest size a box can be 
displayed at when the browser 
window is narrow, and the 
max-width property indicates 
the maximum width a box can 
stretch to when the browser 
window is wide.
- These are very helpful properties 
to ensure that the content of 
pages are legible (especially on 
the smaller screens of handheld 
devices). For example, you can 
use the max-width property to 
ensure that lines of text do not 
appear too wide within a big 
browser window and you can 
use the min-width property 
to make sure that they do not 
appear too narrow.
- You may find it helpful to try this 
example out in your browser so 
that you can see what happens 
when you increase or decrease 
the size of the browser window.

#### limiting height min-height, max-height
- in the same way that you might 
want to limit the width of a box 
on a page, you may also want 
to limit the height of it. This is 
achieved using the min-height 
and max-height properties.

### Border, margin & padding

- Every box has three available properties that 
can be adjusted to control its appearance:
<ol>
<li>BORDER </LI>
Every box has a border (even if 
it is not visible or is specified to 
be 0 pixels wide). The border 
separates the edge of one box 
from another.
<LI>MARGIN</LI>
Margins sit outside the edge 
of the border. You can set the 
width of a margin to create a 
gap between the borders of two 
adjacent boxes.
<LI>PADDING</LI>
Padding is the space between 
the border of a box and any 
content contained within it. 
Adding padding can increase the 
readability of its contents.

#### Border Width 
- The border-width property 
is used to control the width 
of a border. The value of this 
property can either be given 
in pixels or using one of the 
following values:
<ul>
<li> thin</li>
<li> medium</li>
<li>thic</li>

**You cannot use percentages 
with this property**

syntax : 
border-top-width
border-right-width
border-bottom-width
border-left-widt

#### border-style

- You can control the style of a 
border using the border-style 
property. This property can take 
the following values:

- `solid` : a single solid line
- `dotted` :  a series of square dots
(if your border is 2px wide, then 
the dots are 2px squared with a 
2px gap between each dot)

- `dashed` : a series of short lines
- `double` two solid lines (the 
value of the border-width 
property creates the sum of the 
two lines)

- `groove`: appears to be carved 
into the page

- `ridge`: appears to stick out from 
the page

- `inset`: appears embedded into 
the page

- `outset`: looks like it is coming 
out of the screen
hidden / none no border is 
shown

#### padding 
- ou can specify different values 
for each side of a box using:

`padding-top`<br>
`padding-right`<br>
`padding-bottom`<br>
`padding-lef`<br>

- the value of this property is 
most often specified in pixels 
(although it is also possible to 
use percentages or ems). If a 
percentage is used, the padding 
is a percentage of the browser 
window (or of the containing box 
if it is inside another box).

**The value of the padding property is not inherited by child elements in 
the same way that the color value of the font-family property is; so 
you need to specify the padding for every element that needs to use it.**

#### Margin 

- ou can specify values for each 
side of a box using:<br>
`margin-top`<br>
`margin-right`<br>
`margin-bottom`<br>
`margin-lef`<br>

- he margin property controls 
the gap between boxes. Its value 
is commonly given in pixels, 
although you may also use 
percentages or ems.

