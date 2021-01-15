# Lists

- Ordered L ists
- Unordered Lists
- Definition Lists

```html
<!--This is how an Ordered list is made in HTML
Items arranged this way will created a numbered list
-->
<ol>
  <li>1. Cut chicken breasts into chunks.</li>
  <li>2. Apply salt and pepper to chicken thoroughly.</li>
  <li>3. Cook on high heat until browned.</li>
  <li>4. Pour masala sauce over chicken.</li>
  <li>5. Let chicken and sauce simmer for 10 minutes on low hear.</li>
</ol>

<!-- Unordered List:
Items arranged in this way will appear as a bulleted list
-->
<ul>
  <li>1 pound of chickbreasts</li>
  <li>16 jar of Tikka Masala simmer saucer</li>
  <li>cooking spray or 1 tabespoon of butter</li>
  <li>salt and pepper</li>
</ul>

<!-- Definition Lists;
Type of list that will portray a list of words, with their defintions written below them
-->
<dl>
  <dt>Chicken</dt>
  <dd>
    A type of flightless, domestic bird that is commonly bred as a source of
    food.
  </dd>
  <dt>Cooking</dt>
  <dd>
    The act of preparing and combining ingredents in order to create a meal.
  </dd>
</dl>
```

- **Definitons Lists will render as...**
<dl>
  <dt>Chicken</dt>
  <dd>
    A type of flightless, domestic bird that is commonly bred as a source of
    food.
  </dd>
  <dt>Cooking</dt>
  <dd>
    The act of preparing and combining ingredents in order to create a meal.
  </dd>
</dl>

- It is important to note that lists CAN BE NESTED.

# Boxes:

- the demensions of certain block elements can be manipulated in the following was.

```css
/* can by calling the FULL tag directly as a selector*/
div {
  height: 300 px;
  width: 400 px;
}
/*notice that we can alter size based on exact pixels, and on percentage of screen space*/
p {
  height: 75%;
  width: 75%;
}

/*note that we can also set limits on HOW big or small our dimensions can be*/
div.classname {
  min-width: 450px;
  max-width: 450px;
  max-height: 450px;
  min-height: 450px;
  padding: 5px;
  margin: 0px;
}
```

- the **overflow** property can be used control to handle text cannot fit in a box element.
  - overflow has two values that can be applied to it
    - _hidden_: hides extra content that doesnt fit
    - _scroll_: adds scroll feature to the box to fit all contents

## Borders:

- can be applied in css as like so

```css
p.one {
  border-width: 2px; /*set pixel width for each side of the border*/
}

p.two {
  border-width: thick; /*thin, medium, OR thick*/
}
p.three {
  border-width: 1px 4px 12px 4px; /* specfies the width of the border oneach side of the box*/
}

/* Can also apply border styes*/
p.four {
  border-style: solid; /*dashed,dotted,double,ridge,inset,outset,etc*/
}
```

## Padding and Margin Properties

- Padding: allows you to specify how much space should appear between content and its border.
- Margin: controls the gap between boxes.

```css
/* can be set like THIS in css*/
p {
  width: 257px;
  border: 2px;
}
p.example {
  padding: 10px;
  margin: 20px;
}
```

## Other Properties

- **display**: Allows you to turn inline elements into block-level elements, and vice versa.
  - values: inline, block, inline-block, none
- **visibility**: Allows you to hide boxes from users, but leaves a space where the element would normally be.
  - values: hidden, visible.

## Using Switch Statements:

- can be good to use instead of ELSE/IF
- especially if there are multiple conditions.

ELSE/IF example:

```javascript
//Keep in mind that even when a match is found, If statements will still continue to go through every option.
// keyowrd *break;* can ensure that the loops end when a match is found
if ((level = 1)) {
  title = "Level 1";
  break;
} else if ((level = 2)) {
  title = "Level 2";
  break;
} else if ((level = 3)) {
  title = "Level 3";
  break;
} else {
  break;
}
```

SWITCH example:

```javascript
//Far fewer {} and () to worry about
switch (level) {
  case 1:
    title = `Level 1`;
    break;

  case 2:
    title = `Level 2`;
    break;

  case 2:
    title = `Level 2`;
    break;

  // default will run if there are no options that match
  default:
    title = "Test";
    break;
}
```

## Types and Values

- Javascript is _type coercion_, whcih means that it can convert data types behind the scnes to complete an operation.
- Javascript also has _weak typeing_, which means the data type of a value can be changed.

## Loops

- below are some examples of loops!

```js
//FOR LOOP
for (var number = 0; number < 10; number++) {
  msg += msg + "I say 'Bird! Bird! B-birds the word!' ";
}

//WHILE LOOP
var x = 0;
while (x < 100) {
  x++;
}

//DO WHILE LOOP
var x = 100;
do {
  x--;
} while (x > 0);
```

for(var num = 0; num < array.length; num++){
console.log(array[])
}
