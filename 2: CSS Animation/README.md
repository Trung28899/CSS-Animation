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
