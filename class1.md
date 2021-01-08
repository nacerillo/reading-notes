#HTML#
##Structure##

HTML uses elements to describe the structure of pages

these elements are enlosed by **tags**

- **Tag**: serves as a container for an HTML element, and give us information about the nature of those elements.
  - all elements are enclosed by an opening (<tag>) and closing (</tag>) tag

Example:

<html>
    <body>

    <h1>This is a Heading</h1>

    <p>
    Hello World. this is a paragraph
    </p>

    <h2> This is a sub-heading </h2>

    </body>

</html>

Tags can also contain **attributes**, which provide addional information
about an element's contents.

-attributes consist of two parts: a _name_ and a _value_

Example: **style** is the name, and **red** is the value.

<p style = "red"> This paragraph is now red<p>

##Extra Markup##

throughout the years, there have been many different versions of HTML.
Because there are so many versions, web pages created using HTML
should begin with a declaration of _<DOCTYPE>_

- DOCTYPE lets the browser know which version of HTML the page is using

Every HTML Element can also carry an attribute call _id_.

- id is used to identify an element from other elements on a page, even
  among similar elements.
- giving elements an id allow us to style elements from similar instances differently using HTML.
-Example:
   <p id = "para1"> This paragraph is red </p>
   <p id = "para2"> This paragraph is green</p>

HTML Elements can also carry a _class_ attribute.
