# Text In HTML

## Types of Tags/Markup

- **Structured**: elements used to describe headings and paragraphs
- **Semantic**: extra information; such as emphasis in text, quations, acroynms, etc

## Strctured Markup:

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

## Semantic Markup:

**Strong & Emphasis**

- `<strong>...</strong>` is used to mark something as important
- `<em>...</em>` is used to mark emphasis which subtley changes the meaing of the sentence.
- Both are used in much the same way as `<i>` and `<b>`.

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
