# Reading Notes 05

## IMAGES

- images can include logos, photos, button assets, etc
- When picking images to add to your site, the images should...

  - Be relevant
  - Convey information
  - Convey the right mood
  - Be instantly recognizable
  - Fit the color palette

- Consider storing your images in their own folder in your project.

- Adding An Image

  ```html
  <!--alt = text description of the image
      src = source path from where the imaage came from
      title = provide addition info. otherwise, just title
       height/widht = speaks for itself-->
  <img
    src="images/quokka.jpg"
    alt="A family of quokka"
    title="The quokka is an Australian marsupial that is similar in size to the domestic cat"
    height="500"
    width="450"
  />
  ```

  - where an image is placed will affect how it is display.
  - NOTE: the _align_ attribute has been removed from HTML5

  - keep in mind an images file format.
  - Images have a predetermined size, which should be taken into account when trying to fit them into a size you want in CSS
  - Photoshop and other image editing tools can be useful as well

## Color:

- ## colors can be set in css using...

  - RGB Values `rgb(225,225,200)`
  - Hex Codes `#ee3e80`
  - Color names `black`

  - the `background - color` property sets tgat cikir if the background in a box element.
  - opacity of colors can also be controled in css
  - measured in percentage/decimal format.

  ```css
  p {
    background-color: rgb(255, 0, 0);
    opacity: 0.5;
  }
  ```

  - CSS3 introduces 3 other ways of measuring color
    - Hue
    - Saturation
    - Lightness
    - alpha/opacity

```css
/*represent ins css3 as hsla*/
p {
  background-color: hsla(0, 100%, 100%, 0.5);
}
```

## Text

- properties that control text can be split into two groups.

  - those that directly affect the font and its appearance
  - those taht would have the same effect on text no matter what font you are using.

- Text has a HUGE impact on the readabiliy of your page, so dont slack on it.

- 3 properties of text include...
  - Weight
  - Style
  - Stretch
- different fonts are organized together into families called type faces. these are also called `font-family` in html.
