# CSS Transforms, Transitions, and Animations

## CSS Transitions


**- What is CSS Transition?**
* CSS transitions allows you to change property values smoothly, over a given duration.


* Transitions has the following properties:
1. `transition` 
2. `transition-delay` 
3. `transition-duration` 
4. ` transition-property` 
5. `transition-timing-function` 


**- How to Use CSS Transitions?**
* To create a transition effect, you must specify two things:

1. the CSS property you want to add an effect to
2. the duration of the effect

* If the duration part is not specified, the transition will have no effect, because the default value is 0.

* Example: The following example shows a 100px * 100px red `<div>` element. The `<div>` element has also specified a transition effect for the width property, with a duration of 2 seconds:


```
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
}
```

* The transition effect will start when the specified CSS property (width) changes value.


## CSS Transforms

**- What is CSS Transforms?**
* The transform property applies a 2D or 3D transformation to an element. This property allows you to rotate, scale, move, skew, etc., elements.

* Syntax:


```
transform: none|transform-functions|initial|inherit;
```


* Example: Translating and rotating an element:



```
div {
  border: solid red;
  transform: translate(30px, 20px) rotate(20deg);
  width: 140px;
  height: 60px;
}
```



![](https://i.ibb.co/k3d2xp6/aaaa.png)



## CSS Animations

**- What are CSS Animations?**
* An animation lets an element gradually change from one style to another.

* You can change as many CSS properties you want, as many times as you want.

* To use CSS animation, you must first specify some keyframes for the animation.

* Keyframes hold what styles the element will have at certain times.


**-Using The @keyframes Rule:** 

* When you specify CSS styles inside the @keyframes rule, the animation will gradually change from the current style to the new style at certain times.

* To get an animation to work, you must bind the animation to an element.

* Example: 


```
/* The animation code */
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

/* The element to apply the animation to */
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
```

* The animation-duration property defines how long an animation should take to complete. If the animation-duration property is not specified, no animation will occur, because the default value is 0s (0 seconds).

* In the example above we have specified when the style will change by using the keywords "from" and "to" (which represents 0% (start) and 100% (complete)).
