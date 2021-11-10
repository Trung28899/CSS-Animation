## Resources:

- https://easing.net
- https://cubic-bezier.com
- https://jakearchibald.github.io/svgomg/

  > optimize svg before animating them. See section 4 videos

- https://greensock.com/
  > javascript svg animation library

Pre-written CSS animation libraries:

- https://animxyz.com/
- https://animate.style/

Custom Tool:

- https://animista.net/

---

## PART I: Transitions and Transform

## 1: Basic of Transform

- Transform:
  Transform will change how our elements and images appear but won't create animation

- The order of the functions called in transform does affect how the element will
  appear because the transform refer to itself

- 3d Transform

Example Code:
transform: translate(100px, 200px) scale(2) rotate(90deg);

## 2: Transition

- transition took place whenever the element change
  we can have different properties of the css changed differently
  like the code down below

  transition: background 0.3s ease-in, transform 0.2s ease-in-out,
  border-radius 0.5s;

See Code Folder for more info

## NOTABLE PROPERTIES / SYNTAX:

- transform
- transition

---

## PART II: CSS Animation Fundamental

## Keyframe Fundamental:

1. animation-fill-mode:
   +, animation-fill-mode: backwards; set the element style in delay time (before animation) to keyframe styling at 0%
   +, animation-fill-mode: forwards; set the element style After an animation to keyframe styling at 100%
   +, animation-fill-mode: both; do both of the above values

=> See video: "A closer look at animation-fill-mode" to understand how it works

2. Timing Function and easing:

   - Easing is what describes the speed changes of your animation
   - can be used in animation (with animation-timing-function:) or transition (transition-timing-function)
   - there are 3 options for this:
     +, Easing keywords: ease, ease-in-out, ease-in, ease-out, linear.

     +, Custom cubic-bezier curves:
     a more custom function of easing. Visit this website to choose your custom
     cubic-bezier: https://cubic-bezier.com/

     +, steps(): Plays an animation back in a defined number of steps. Pausing briefly at each, instead of smoothly interpolating
     between keyframes states. Good for work typing animation

=> See video "2: Timing functions and easing" for this
=> See code in "2: animation-direction" Folder
=> See code for steps() in "2: steps()" Folder

## Notable Properties:

- animation-name
- animation-duration

- animation-delay: specifies the amount of time to wait before beginning
  to perform the animation
- animation-fill-mode: let you control what happens during delays before an animation
  starts actively playing, and/or what happens after an animation's duration has ended

=> See the properties above in "2: KeyFrame Fundamental" Folder

- animation-direction: lets you control what order your keyframes are executed in. It values:
  +, normal
  +, reverse
  +, alternate
  +, alternate-reverse

- animation-iteration-count: defines how many times does the animation repeat

- animation-timing-function: lets you control the type of animation speed

=> See the properties above in "2: animation-direction" Folder

## Notable Syntax:

- @keyframe keyFrameName {}

---

## PART III: CSS Animation Building Blocks

## Infinite Loop:

- See animation in "3: Infinite Looping" Folder

## animation-play-state

- controls whether an animation is playing or paused
  animation-play-state: paused; > stop animation
  animation-play-state: running; > Play animation

see code in "3: Play Or Pause" Folder

- Chaining KeyFrame:
  => See code in "3: Chaining Multiple KeyFrame"

## Notable Properties:

- perspective: 1000px; Always set this for 3d animation
- transform-style: preserve-3d;

- transform-origin: the point around which a transformation is applied

=> See these properties in "3: 3d Transform" Folder

---

## PART IV: Animating SVG

## Animating SVG:

- SVG Exporting and Optimization Settings

## Notable:

- Origin point of a svg is at the top left
- JS library for SVG animation: https://greensock.com/

---

## PART V: Advanced CSS Animation

## Notable Properties:

- offset-path: Specifies a path for an element to follow or be placed along
- offset-distance: specifies a position along an offset-path for an element
  to be placed

- font-variation-settings: provides low-level control over variable fonts
  based on the axis and characteristics available in a given font

## Motion path creation:

- Need to get path from a SVG editor
  create path in svg > copy the svg code > in the <path>
  > look for d=. The value there is what we need to put in offset-path

=> See code in "5: Motion Path" Folder

## Dynamic Animation With CSS Variables:

- CSS Variables:
  +, Can be changed at runtime
  +, Follow the CSS cascade
  +, Can be easily accessed by Javascript

=> See code in "5: Dynamic CSS Animation" Folder

## Animating Variable Font with CSS:

- Variable Font:
  +, A font file that is able to store a continuous range of design variants
  +, See last video in Part 5 for more understanding

Resources:
https://wakamaifondue.com
https://recursive.design

Custom Tool:
https://animista.net/

---
