# Class 04 Notes

## Links

- link uses:

  - link from one website to another.
  - link from one page to page on the same website.
  - link from one part of a webpage to another part
  - links can open in a new browser
  - start up your email program and address a new email to someone

- links make use of the `<a>` element

```html
<!-- link to a new website -->
<a href="http://www.imdb.com"> IMDB</a>

<!--link to another page of a site-->
<a href="index.html">Home</a>
<a href="contact.html">Contacts</a>

<!--link to email-->
<a href="mailto:jonas@gmail.com">Email Jonas</a>

<!--Opening a link in a new window-->
<a href="http://www.imdb.com" target="_blank"></a>
```

## Layout

- Position Properties

  - **Absolute:** positions the elements in relation to its containg elements. it does not affect the position of its
    surrounding elements
  - **Fixed:** Removes element from the normal flow, and instead positon something relative to the view port?
  - **Relative:** keeps the element within the normal flow, but can be moved left and right, and can still use as an anchor point
  - **Static:** flow is preserved. cannot be used as anchor point.
  - **Sticky:** combination of fixed and absolute.
