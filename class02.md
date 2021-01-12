# Class 2 Notes

## Text In HTML

### Types of Tags/Markup

- **Structured**: elements used to describe headings and paragraphs
- **Semantic**: extra information; such as emphasis in text, quations, acroynms, etc

### Strctured Markup:

- **Headings:**

  - `<h1>, <h2> ,<h3>, <h4>, <h5>, <h6>`
  - six levels of size, `<h1>` being biggest, and `<h6>` being smallest

- **Paragraphs:**

  - `<p>`
  - surrounding text with <p> to create paragraph blocks

    ```html
    <p>
      hello, my name is nick, and this is a how I would create a paragraph in
      HTML.
    </p>
    ```

    - **Bold & Italic:**

    - enclosing text with `<b>...</b>` or `<i>...</i>` will make make text bold or italicized respectivly.
    -

    ```html
    <p><i>Good morning</i>, and <b> hello world </b></p>
    ```

      <p> <i>good morning</i> and <b> hello world</b> </p>

    **Subscript/Superscript:**

    - subscript = `<sub>...</sub>`
    - superscript = `<sup>...</sup>`

    ```html
    <p>Papers are due one the 4<sup>th</sup> of January</p>

    <p>E = MC<sup>2</sup></p>
    ```

       <p> Papers are due one the 4<sup>th</sup> of January</p>
       <p> E = MC<sup>2</sup></p>

    **LineBreaks/Horizontal Rules:**

    - line breaks: `<br />`

    ```html
    <p>
      The Earth<br />gets one hundred tons heaveir every day <br />
      due to falling debris
    </p>
    ```

      <p>
      The Earth<br />gets one hundred tons heaveir every day <br />
      due to falling debris
    </p>

    - horizontal divide: `<hr />`

    ```html
    <p>Venus is the only planet that rotates clockwise.</p>
    <hr />
    <p>Jupitor is bigger than all the planets combined.</p>
    ```

    <p>Venus is the only planet that rotates clockwise.</p>
    <hr />
    <p>Jupitor is bigger than all the planets combined.</p>

### Semantic Markup:

**Strong & Emphasis**

- `<strong>...</strong>` is used to mark something as important
- `<em>...</em>` is used to mark emphasis which subtley changes the meaing of the sentence.
- Both are used in much the same way as `<i>` and `<b>` cosmetically.

**Quotations**

- `<blockquote>...</blockquote>` for long quotations
- `<q>...</q>` for shoter quotations.

```html
<blockquote>
  <p>Did you ever stop the think, and forget to start again?</p>
</blockquote>
<p>
  As A.A Milne once said.
  <q>
    Some people talk to animals. Not many listen though. That's the problem</q
  >
</p>
```

  <blockquote>
    <p>Did you ever stop the think, and forget to start again?</p>
  </blockquote>
  <p>
    As A.A Milne once said.
    <q>
      Some people talk to animals. Not many listen though. That's the
      problem</q>
  </p>

**Abbriviations/Acroynms:**

- abbreviation = `<abbr>`
- acronym = `<acronym>`

```html
<p>
  <abbr title="Doctor"
    >Dr.</abbr>
      Anthony Morris is a leader in both brain and bone cancer research</abbr
    ></abbr
  >
</p>

<p><acronym title = "National Aeronautics and Space Admin">NASA
</acronym></p>

```

**Changes To Content:**

- `<ins>..</ins>` adds underline to text.
- `<del>..</del>` item has been deleted out text.
- `<s>..</s>` item is no longer relevant.
- Both `<del>` and `<s>` cross out text.

## Introducing CSS

- allows us to maniuplate color, size, fonts, etc on an html page.
- CSS rules are applied through a _selector_, and a _declaration_.

```css
selector - p {
  font-family: Arial ---- declaration;
}
```

- _Declaration_ is made up of a property - such as funt size - , and
  a value - such as Arial.

- A `<link>` element can be used within an HTML file to tell the broswer to use a style page.
  - ```html
    <head>
      <link href="css/styles.css" type="text/css" rel="stylesheet" />
    </head>
    ```
- A `<style>` element can be used to at styling within HTML
  - ```html
    <style type="text/css">
      body {
        font-family: arial;
      }
      h1 {
        color: red;
      }
    </style>
    ```
- **\*types of selectors include**:
  - class selector - `h1, h2, h3 { }`
  - type selector - `.note { }`
  - id selector - `#idname { }`

## Basic Javascipt Instructions:

- **Statements:** Insctructions that make up the script of JS.

- **Code-Block:** A set of one or more statements wrapped within `{}`.

- **Variables:** a container that temporarily holds a piece of data.
  - they are declared in code as `var today = new Date()`. where `var` is the keyword used to name `today` as a variable.

### Data types:

- numerical: a number
- string: text characters
- boolean: true/false

- **Arrays:** lists of related values.

  - Declared as `colors = ['red', 'white', 'blue']`. or
    `var colors = new Array('red', 'white', 'blue')`
  - Can get the length of an array using `length = colors.length`

- **operators:**

  - Addition +
  - Subtration -
  - Division /
  - Multiplication \*
  - Increment ++
  - Decrement --
  - Modules %

  - order of operations follows same as it does in normal arithmatic

## Decisions and Loops:

- sometimes the code must be written in a way for one line of code will followed instead of another line of code. conditions are set that decided which path of code is taken.

- Example
  ```js
  if (score > 50) {
    document.write("You passed!");
  } else {
    document.write("Try again...");
  }
  ```
- Comparison Operators:

  - `==` - is equal to
  - `!=` - is not equal
  - `===` - stict equal
  - `!==` - strict not equal to
  - `>` - gretaer than
  - `<` - lesser than
  - `>=` - greater than or equal to
  - `<=` - less than equal to

- Logical Operators:
  - `&&`
  - `||`
  - `!`
