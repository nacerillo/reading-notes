# Class Notes 14-a:

## What Google Learned From Its Quest to Build the Perfect Team:

- understanding and influencing group norms were the keys to improving Google’s teams.

- Good teams all had high ‘‘average social sensitivity’’ — a fancy way of saying they were skilled at intuiting how others felt based on their tone of voice, their expressions and other nonverbal cues.
- teams like minded peiople with high "average socical sensitivity" and asymetrical heirachry seem to be the optimal team structure.

- Make sure that you can trust the people that you are with
- Make sure that you feel value in your team.
- Everyone is able to communicate and contribute. 
- team-meates that hav good emotional awareness of one another. 

## CSS Transformations:

- Transform: moving/manipulating an object over a 2d or 3d plane.
- `transform` property examples below.
  Example:
  All of these properties can be used to transform shapes on a screen.

```css
/*2D Transforms */
div {
  transform: scale(1.5, 1.5);
  transform: scaleX(1.5);
  transform: scaleY(1.5);
  transform: rotate(25deg);

  transform: translateX(10px);
  transform: translateY(10px);
  transform: translateX(10px, 10px);

  transform: skew(5deg);
  transform: skewX(20deg);
  transform: skewY(20deg);
  /* this changes the angle of the 'camera' that the screen shows*/
  transform: perspective(200px) rotateX(45deg);

  /*
  
  3D transform are much the same, excpet they include the Z-axis.
  */
}
```

## Transitions and Animations:

- transtions must have a change of state. and different stles must be identified for each state.

- the four transition properties are...

  - `transtion-property` determines what properteis will be altered
  - `transtion-duration` determines how long the transition takes place
  - `transtion-timing-function` sets the speed/acceleration of the transition
  - `transition-delay` control when the transition takes place.

  ```css
  .box {
    background: #2db34a;
    transition-property: background;
    transition-duration: 1s;
    transition-timing-function: linear;
  }
  ```

  Full animations are used when more control or complexity is required.

  - The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

    - below are the porperties that can be set for an animation, along with how keyframes are set in css

  ```css
  @keyframes slide {
    0% {
      left: 0;
      top: 0;
    }
    50% {
      left: 244px;
      top: 100px;
    }
    100% {
      left: 488px;
      top: 0;
    }
  }

  .stage:hover .ball {
    animation-name: slide;
    animation-duration: 2s;
    animation-timing-function: ease-in-out;
    animation-delay: 0.5s;
  }
  ```

  ## Examples of On-Hover Effects

  Fade in

  ```css
  .fade {
    opacity: 0.5;
  }
  .fade:hover {
    opacity: 1;
  }
  ```

  Color Change

  ```css
  .color:hover {
    background: #53a7ea;
  }
  ```

  Grow n Shrink

  ```css
  .grow:hover {
    -webkit-transform: scale(1.3);
    -ms-transform: scale(1.3);
    transform: scale(1.3);
  }
  ```

  Rotation

  ```css
  .rotate:hover {
    -webkit-transform: rotateZ(-30deg);
    -ms-transform: rotateZ(-30deg);
    transform: rotateZ(-30deg);
  }
  ```

  Square to Circle

  ```css
  .circle:hover {
    border-radius: 50%;
  }
  ```

  3D Shadow Effect

  ```css
  .threed:hover {
    box-shadow: 1px 1px #53a7ea, 2px 2px #53a7ea, 3px 3px #53a7ea;
    -webkit-transform: translateX(-3px);
    transform: translateX(-3px);
  }
  ```
