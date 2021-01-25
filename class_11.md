# Class 11:

## Images:

- like most elements, image size can be controlled using `width` and `height` properties in css.
- it is sometimes good practice to have all of your images be the same size.
- the `align` property can be used to position images, but it is usally better to use `float`
- by default, images are _INLINE ELEMENTS_.
- to center an image, recommend setting it to `display: block`

- `background-image` property allows you to place image behindn other HTML elements.
- `background-repeat` property allows you to copy an image along a defined path to create a pattern.

```css
p {
  background-image: url("iamges/pattern.gif");
  background-repeat: repeat-x;
}
```

- `background-position` can also be used to define where an image will appear. potential values include...

  - `top left`
  - `top right`
  - `bottom left`
  - `bottom right`
  - `center top`
  - `center bottom`
  - etc.

- can also use percentages to set position.
- **Rollover:** when a button changes to a different style when the users clicks or moves over a button.
- **Sprite:** a single image that is used for several different parts of an interface.

## Practical Info:

### Search Enging Optimization:

- the practice of trying to help a site appear nearer to the top of search engine results.
- the idea of working out which terms people are likely to enter into a search to find your site.
- search engines also look at how many sites link to you.
- **On-Page-Techniques:** include key words that people would search for within the text and HTML code.
- **Off-Page-Techniques:** getting other sites to link to yours. the more sites linked to yours, the more likely your site is to come up on a search.
- Key words in things like the page title, web url, headins, text, text links, page descriptions, etc.

### Analytics:

- it is important to learn about those that visit your site.
- Google.com/analytics gives your site a tracking code. every time some visits your page, the code sens data to Google servers.
- you can look up information such as the number of visits, average time people spend on the site. etc.

## Video and Audio:

- The `<video>` and `<audio>` elements allow us to embed video and audio into web pages.

```html
<video controls>
  <source src="rabbit320.mp4" type="video/mp4" />
  <source src="rabbit320.webm" type="video/webm" />
  <p>
    Your browser doesn't support HTML5 video. Here is a
    <a href="rabbit320.mp4">link to the video</a> instead.
  </p>
</video>

<!--The <source> element allows us to present a video in different formats -->
```

- Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example `HTMLMediaElement.play()`, `HTMLMediaElement.pause()`, etc. This interface is available to both `<audio>` and `<video>` elements, as the features you'll want to implement are nearly identical. Let's go through an example, adding features as we go.

- Event handler functions associated with video/audio
  - `playPauseMedia()`
  - `stopMedia()`
  - `mediaBackward()`
  - `mediaForward()`
