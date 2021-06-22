#  Basics of HTML, CSS & JS
- From duct html/css text book,Chapter 2. 
- **The main aspects :**
* Headings and paragraphs X
* Bold, italic, emphasis X
* Structural and semantic markup

### Headings and paragraphes: 

- When creating a web page, you add tags 
(known as markup) to the contents of the 
page. These tags provide extra meaning 
and allow browsers to show users the 
appropriate structure for the page.
In this chapter we focus on how to add markup to the text that 
appears on your pages. You will learn about:

- **Structural markup**: the elements that you can use to 
describe both headings and paragraphs
- **Semantic markup:**   which provides extra information; such 
as where emphasis is placed in a sentence, that something 
you have written is a quotation (and who said it), the 
meaning of acronyms, and so on

#### Headings : 
-  <q>`<h1>`</q> element is the largest, and the contents of 
an `</h6>` element is the smallest
#### Paragraphs :
- To create a paragraph, surround 
the words that make up the 
paragraph with an opening `<p>` 
tag and closing `</p>` tag
#### Bold & iTalic : 
- by enclosing words in the tags 
`<b>` and `</b>` we can make 
characters appear bold.
The `<b>` element also represents 
a section of text that would be 
presented in a visually different 
way (for example key words in a 
paragraph) although the use of 
the `<b>` element does not imply 
any additional meanin

#### line Breaks and horizental loops : 
- As you have already seen, the 
browser will automatically show 
each new paragraph or heading 
on a new line. But if you wanted 
to add a line break inside the 
middle of a paragraph you can 
use the line break tag `<br />`
- To create a break between 
themes — such as a change of 
topic in a book or a new scene 
in a play — you can add a 
horizontal rule between sections 
using the `<hr />` tag.
#### strong & emphasis 
- `<strong>` :  The use of the `<strong>` 
element indicates that its 
content has strong importance. 
For example, the words 
contained in this element might 
be said with strong emphasis.
By default, browsers will show 
the contents of a `<strong> `
element in bold

- `<em>` : The `<em>` element indicates 
emphasis that subtly changes 
the meaning of a sentence.
By default browsers will show 
the contents of an `<em>` element 
in italic.
- ##  semantic markup:
> There are some text elements that are not intended to affect the 
structure of your web pages, but they do add extra information to the 
pages — they are known as semantic markup.


# INTRODUCING CSS : 

- CSS treats each HTML element as if it appears inside  
its own box and uses rules to indicate how that 
element should look.
- Rules are made up of selectors (that specify the  
elements the rule applies to) and declarations (that 
indicate what these elements should look like).

- Different types of selectors allow you to target your  
rules at different elements.
- Declarations are made up of two parts: the properties 
of the element that you want to change, and the values 
of those properties. For example, the font-family 
property sets the choice of font, and the value arial 
specifies Arial as the preferred typeface.
- CSS rules usually appear in a separate document,  
although they may appear within an HTML page.

### Using external CSS : 
- `<link>` : The `<link>` element can be used 
in an HTML document to tell the 
browser where to find the CSS 
file used to style the page. It is an 
empty element (meaning it does 
not need a closing tag), and it 
lives inside the `<head>` element. 
It should use three attributes:
hrefThis specifies the path to the 
CSS file (which is often placed in 
a folder called css or styles).
typeThis attribute specifies the type 
of document being linked to. The 
value should be text/css.
relThis specifies the relationship 
between the HTML page and 
the file it is linked to. The value 
should be stylesheet when 
linking to a CSS file.
An HTML page can use more 
than one CSS style sheet. To 
do this it could have a `<link>` 
element for every CSS file it 
uses. For example, some authors 
use one CSS file to control the 
presentation (such as fonts and 
colors) and a second to control the layout .

### Usinng Internal CSS : 
`<style>`

You can also include CSS rules 
within an HTML page by placing 
them inside a `<style>` element, 
which usually sits inside the 
`<head>` element of the page. 
The `<style>` element should use 
the type attribute to indicate 
that the styles are specified in 
CSS. The value should be text/
css.
When building a site with more 
than one page, you should use 
an external CSS style sheet. This:
- Allows all pages to use the  
same style rules (rather than 
repeating them in each page).
- Keeps the content separate  
from how the page looks.
- Means you can change the styles used across all pages 
by altering just one file 
(rather than each individual 
page)


### WHY USE EXTERNAL STYLE SHEEET ?

- All of your web pages can share 
the same style sheet. This is 
achieved by using the `<link>` 
element on each HTML page of 
your site to link to the same CSS 
document. This means that the 
same code does not need to be 
repeated in every page (which 
results in less code and smaller 
HTML pages). 

Therefore, once the user has 
downloaded the CSS stylesheet, 
the rest of the site will load 
faster. If you want to make a 
change to how your site appears, 
you only need to edit the one 
CSS file and all of your pages 
will be updated. For example, 
you can change the style of 
every `<h1>` element by altering

- the one CSS style sheet, rather 
than changing the CSS rules on 
every page. The HTML code 
will be easier to read and edit 
because it does not have lots of 
CSS rules in the same document. 
It is generally considered good 
practice to have the content of 
the site separated from the rules 
that determine how it appears.