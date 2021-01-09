# HTML

## Structure

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

## Extra Markup

throughout the years, there have been many different versions of HTML.
Because there are so many versions, web pages created using HTML
should begin with a declaration of _<DOCTYPE>_

- DOCTYPE lets the browser know which version of HTML the page is using

Every HTML Element can also carry an attribute call _id_.

- **id** is used to identify an element from other elements on a page, even
  among similar elements.
- giving elements an id allow us to style elements from similar instances differently using HTML.
-Example:
<html>
<body>
   <p id = "para1"> This is paragraph 1 </p>
   <p id = "para2"> This is paragraph 2</p>
   </body>
   </html>

HTML Elements can also carry a **class** attribute.

# Javascript

## The ABCs of Programming

- A. What is a script?

  - a script is a set of instructions that a computer reads in order to achieve a certain outcome or goal

  - just as we would follow every step outline in a recipe or repair manual to complete a task, a computer follows every action and task written within a script one at a time to reach a desired outcome.

  - to create a script, you should do the following

    1. Define The Goal:

       - define what you want the purpose of the script is. What task do you wish
         for your computer to complete using your script?

    2. Design The Script:

       - as mentioned before, a script is made up of a series of tasks and actions. split your goal into a list or flow chart of differnt tasks
         that most be done in order to reach your goal.

    3. Code Each Step:
       - each step must then be translated into code, in our case _Javascript_

  - a script must be written as _CODE_: a special language that we use to communicate computers in order to get them to do something.
    - like all languages, code has **Vocabulary** (key words that a computer will be able to recognize), and **Syntax** (the way in which the instrutions are arranged in script).
  - computers read these instructions **programmatically**; which means they read the script one task at a time.

- B. Computers and the World Around Them:

  - In programming, a physical thing may be represent in an **object**
  - Objects can be defined by their...

    1. Properties
       - the descriptors of an object. what charascteristics does the object possess?
       - Example:
         Object Person:
         Properties:
         Name: Bob
         Gender: Male
         Hieght: 5'11
         Married: False
    2. Events

       - Actions that a computer performs in response to certain inputs
         and interactions that it reads from a user.
       - Example:
         Object Person:
         Event | Trigger:
         Walk | when given command to walk
         Jump | when given command to jump

    3. Methods
       - represent what actions are taken in relation to the object. They can
         retrieve or update an objects property, and can be triggered by events
       - methods can contain a large amount of code and instructions that
         make up a single task.
       - Example:
         exercise();
         startEngine();

  - Web Browsers

    - A web page is made up of many objects
    - Two important objects include the **Window** and the **Document** objects

      - Window: Represents each tab/page. contains a _location_ property that tells
        the url of the current page.
      - Document: models the current webpage that is loaded into each window. contains
        the _title_ property (everything that is enclosed within the <title></title> tags)
        and the _lastModified_ property(date of when that page was last altered)

    - Web browsers use HTML markup to create a model of a web page.

- C. Writing Script for a Webpage: - All web pages are build using HTML, CSS and JAvascript - HTML displays content of a page, and defines the structure of the content - CSS enhances HTML content (background,sizes, borders, color) - Javascript defines the behaviour and actions of the webpage.

       - build the webpage layer be layer: HTML -> CSS -> Javascript

  - When you want to link a javascript or css file to an HTML file, use the lines
      <html> 
      <link rel = "stylesheet1" href = "css/stylesheet1.css"/>
      <script src = "js/javaconent.js"></script>
      </html>

  - can also add Javascript in line with HTML.
      <html>
          <script> 
              document.write('<h3> Welcome! </h3>');
          </script>
      </html>
