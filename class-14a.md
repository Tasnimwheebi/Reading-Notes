# Transforms
With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

*The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.*

## Transform Syntax
    div {
    -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
             transform: scale(1.5);
    }

## 2D Transforms
* 2D Rotate : The rotate value provides the ability to rotate an element from 0 to 360 degrees.
* 2D Scale : The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger. 

(Using the scale value within the transform property allows you to change the appeared size of an element).

* 2D Translate : Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
* 2D Skew : is used to distort elements on the horizontal axis, vertical axis, or both.

*  Combining Transforms :
It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

* Transform Origin :
The default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used.

* Perspective :
The perspective of an element can be set in two different ways:
    * One way includes using the perspective value within the transform property on individual elements.
    * The other includes using the perspective property on the parent element residing over child elements being transformed.
  ##   3D Transforms 
 * 3D Rotate : With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.

 * 3D Scale :By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale.
 * 3D Translate : Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.
 * 3D Skew :  Elements may be skewed on the x and y axis, then transformed three-dimensionally as wished, but they cannot be skewed on the z axis.
 * Shorthand 3D Transforms : As with combining two-dimensional transforms, there are also properties to write out shorthand three-dimensional transforms. These properties include rotate3d, scale3d, transition3d, and matrix3d.


# Transitions & Animations
## Transitions 
A transition to take place, an element must have a change in state, and different styles must be identified for each state.
* Transitional Property : The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. 
* Transition Duration : The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms).
* Transition Timing :The transition-timing-function property is used to set the speed in which a transition will move.
* Transition Delay : The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. 
* Shorthand Transitions : Declaring every transition property individually can become quite intensive, especially with vendor prefixes. Fortunately there is a shorthand property, transition, capable of supporting all of these different properties and values.

## Animations 
* Animations Keyframes : The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
* Animation Name : The animation-name declaration is applied to the element in which the animation is to be applied to.
### Customizing Animations 
* Animation Iteration : By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the animation-iteration-count property may be used.
* Animation Direction :  to set the number of times an animation repeats, you may also declare the direction an animation completes using the animation-direction property.
* Animation Play State : The animation-play-state property allows an animation to be played or paused using the running and paused keyword values respectively.
* Animation Fill Mode : The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run.
### Shorthand Animations 
Fortunately animations, just like transitions, can be written out in a shorthand format. This is accomplished with one animation property, rather than multiple declarations.