# Notes -

## Creating react project using vite -

`npm create vite@latest my-react-app -- --template react`
Here in place of react you can also use - react-ts, react-swc, react-swc-ts

**To Run dev server in vite -**
`npm run dev`

## CSS selector basics -

CSS selectors are patterns used to select the HTML elements that you want to style. There are different types of CSS selectors, such as:

### Element selectors:

select HTML elements based on their tag name, such as `p` for paragraphs or `h1` for headings.

### Class selectors:

select HTML elements that have a specific class attribute, such as `.intro` for elements with `class="intro"`.

### ID selectors:

select a unique HTML element that has a specific id attribute, such as `#firstname` for the element with `id="firstname"`.

### Attribute selectors:

select HTML elements that have a specific attribute or attribute value, such as `[target="_blank"]` for elements with `target="\_blank"`.

### Pseudo-class selectors:

select HTML elements based on their state, such as `:hover` for elements that are hovered over by the mouse or `:checked` for checked checkboxes.

#### list of some common pseudo-class selectors:

**:active:** selects an element when it is activated by the user, such as clicking on a link or button.

**:checked:** selects an element that is checked, such as a checkbox or radio button.

**:disabled:** selects an element that is disabled and cannot be interacted with by the user, such as a form input or button.

**:empty:** selects an element that has no children, including text nodes.

**:enabled:** selects an element that is enabled and can be interacted with by the user, such as a form input or button.

**:first-child:** selects an element that is the first child of its parent element.

**:first-of-type:** selects an element that is the first of its type among its siblings.

**:focus:** selects an element that has focus, such as a form input or a link.

**:hover:** selects an element when the user hovers over it with the mouse cursor, such as a link or a button.

**:invalid:** selects an element that has an invalid value, such as a form input that does not match the required pattern or format.

**:lang:** selects an element that has a specific language attribute, such as `lang="en"` for English or `lang="fr"` for French.

**:last-child:** selects an element that is the last child of its parent element.

**:last-of-type:** selects an element that is the last of its type among its siblings.

**\:link:** selects an element that is an unvisited link, such as an anchor element with an href attribute.

**:not:** selects an element that does not match a given selector, such as `:not(p)` for elements that are not paragraphs.

**:nth-child:** selects an element that is the nth child of its parent element, where `n` can be a number, a keyword, or a formula, such as `:nth-child(2)` for the second child, `:nth-child(odd)` for odd-numbered children, or `:nth-child(3n+1)` for every third child starting from the first.

**:nth-last-child:** selects an element that is the nth child of its parent element, counting from the last child, where n can be a number, a keyword, or a formula, such as `:nth-last-child(2)` for the second to last child, `:nth-last-child`(even) for even-numbered children, or `:nth-last-child(3n+1)` for every third child starting from the last.

**:nth-of-type:** selects an element that is the nth of its type among its siblings, where n can be a number, a keyword, or a formula, such as `:nth-of-type(2)` for the second element of its type, :nth-of-type(odd) for odd-numbered elements of its type, or :nth-of-type(3n+1) for every third element of its type starting from the first.

**:nth-last-of-type:** selects an element that is the nth of its type among its siblings, counting from the last element of its type, where n can be a number, a keyword, or a formula, such as `:nth-last-of-type(2)` for the second to last element of its type, `:nth-last-of-type(even)` for even-numbered elements of its type, or `:nth-last-of-type(3n+1)` for every third element of its type starting from the last.

**:only-child:** selects an element that is the only child of its parent element.

**:only-of-type:** selects an element that is the only element of its type among its siblings.

**:optional:** selects an element that is optional, such as a form input that does not have the required attribute.

**:read-only:** selects an element that is read-only and cannot be modified by the user, such as a form input with the readonly attribute.

**:read-write:** selects an element that is read-write and can be modified by the user, such as a form input without the readonly attribute.

**:required:** selects an element that is required, such as a form input with the required attribute.

**:root:** selects the root element of the document, which is usually the `<html>` element.

**:target:** selects an element that is the target of the current URL fragment, such as an element with an id that matches the hash part of the URL.

**:valid:** selects an element that has a valid value, such as a form input that matches the required pattern or format.

**:visited:** selects an element that is a visited link, such as an anchor element with an href attribute that has been clicked by the user.

[CSS Pseudo-Classes Selectors (With Examples)](https://www.programiz.com/css/pseudo-class-selectors)

### Pseudo-element selectors:

select and style a part of an HTML element, such as `::before` for inserting content before an element or `::first-letter` for styling the first letter of an element.

#### list of all pseudo-element selectors:

**::after:** inserts content after the element
**::backdrop:** styles the backdrop of a fullscreen element
**::before:** inserts content before the element
**::cue:** styles the cue text of a media element
**::cue-region:** styles the cue region of a media element
**::first-letter:** styles the first letter of the element
**::first-line:** styles the first line of the element
**::file-selector-button:** styles the file selector button of an input element
**::grammar-error:** styles the text that has a grammar error
**::marker:** styles the marker of a list item
**::part():** styles a part of a shadow DOM subtree
**::placeholder:** styles the placeholder text of an input element
**::selection:** styles the user-selected part of the element
**::slotted():** styles a slot of a shadow DOM subtree
**::spelling-error:** styles the text that has a spelling error
**::target-text:** styles the text that matches the URL fragment

[CSS Pseudo-Element Selector (With Examples)](https://blog.logrocket.com/css-pseudo-elements-guide/)

### Combinator selectors:

select HTML elements based on their relationship with other elements, such as div p for selecting all `<p>` elements inside `<div>` elements or `div > p` for selecting only the direct children `<p>` elements of `<div>` elements.

**Descendant selector:**
selects elements that are descendants (children, grandchildren, etc.) of another element. It is represented by a `space` character. For example, `div p` selects all `<p>` elements inside `<div>` elements.

**Child selector:**
selects elements that are direct children of another element. It is represented by a greater-than sign `(>)`. For example, `div > p` selects all `<p>` elements that are immediate children of `<div>` elements.

**Adjacent sibling selector:**
selects elements that are next to each other and have the same parent element. It is represented by a plus sign `(+)`. For example, `p + img` selects all `<img>` elements that are immediately after a `<p>` element.

**General sibling selector:**
selects elements that are siblings of another element, regardless of their position. It is represented by a tilde `(~)`. For example, `p ~ img` selects all `<img>` elements that are after a `<p>` element.

## CSS position basics -

The CSS position property is used to define the position of an element on a webpage.

The location of the positioned element is set with the four properties: top, left, right, and bottom. These properties only work when the position property is set and have different positioning behaviors.

The position property has the following five values:

### static (default value)

The `static` value of the `position` property allows elements to be positioned accordingly to the normal flow of the document. The `static` position is not affected by the `top`, `right`, `bottom`, and `left` values.

```
p.main {
    position: static;
    top: 50px; /* doesn't work */
    right: 50px; /* doesn't work */
    bottom: 50px; /* doesn't work */
    left: 50%; /* doesn't work */
    background-color: greenyellow;
}
```

### relative

The `relative` value positions the element relative to the original position in the document. The element is positioned with the `top`, `right`, `bottom`, and `left` values.

```
p.main {
    position: relative;
    /* positions 90px from the top */
    top: 90px;

    /* positions 40px from the left */
    left: 40px;
    background-color: greenyellow;
}
```

### absolute

The `absolute` value removes the element completely from its normal flow in the document.

The element is positioned relative to their closest positioned parent element (an ancestor element with a position value other than `static`).

If there is no positioned ancestor, they are positioned relative to the document itself.

```
p.main {
    position: absolute;
    top: 70px;
    left: 60px;
    background-color: greenyellow;
}
```

_Note: An absolutely positioned element loses its size and original space in the document flow._

### fixed

The `fixed` value positions an element to remain fixed in the same position, even when the page is scrolled. It is similar to the `absolute` value, but it remains relative to the viewport at all times.

```
p.main {
    position: fixed;
    top: 10px;
    background-color: greenyellow;
}
```

### sticky

The `sticky` value positions the element as a combination of `relative` and `fixed` values.

The `sticky` position behaves like `relative` positioning until the element reaches a certain scroll point on the screen. After that, the element sticks to the top of the viewport like a `fixed` element.

```
p.main {
    position: fixed;
    top: 10px;
    background-color: greenyellow;
}
```

## Animating with only CSS -

### CSS 2D Transforms Methods

The CSS 2D transform property allows us to use the following transformation methods:

#### translate():

moves an element both horizontally and vertically
`transform: translate(x-value,y-value)`
_Note: The negative value moves the element in the opposite direction._
`transform: translate(60px, -20px)`

#### rotate():

rotates an element in either clockwise or anticlockwise direction
`transform: rotate(degree)`
_Note:The negative degree value rotates the element in the anti-clockwise direction._
`transform: rotate(-30deg)`

#### scale():

increases or decreases the size of an element
`transform: scale(x-value, y-value)`
`transform: scale(2, 0.5)`

#### skew():

distorts an element by tilting along x and/or y axes
`transform: skew(x-angle,y-angle)`
_Note: The skew angles can be positive or negative, depending on the direction we want to skew the element. Positive values tilt the element in one direction, while negative values tilt it in the opposite direction._
`transform: skew(10deg, 20deg)`

#### matrix():

combines multiple transform methods into a single method
`matrix(scaleX(), skewY(), skewX(), scaleY(), translateX(), translateY())`
_Note: The skew values in the matrix() function are specified in radians, not degrees._
`transform: matrix(1.5, 0.5, -0.5, 1, 50, 10)`

[CSS 2D Transform](https://www.programiz.com/css/2d-transform)

### CSS 3D Transforms Methods

To visualize the effect of 3D transform methods, we need to use a perspective property. This property allows us to define the virtual distance between the viewer and 3D transformed elements.

The syntax of the perspective property is: `perspective: length_value;`

The perspective property takes a length value, which indicates the distance from the viewer to the 3D plane containing the transformed element.

CSS 3D transform property allows us to use the following transformation methods:

#### translate3d()

The translate3d() method moves an element in a three dimensional space along the x, y, and z-axes.
`transform: translate3d(x-value,y-value,z-value)`

#### rotate3d()

The rotate3d() method rotates an element in the three-dimensional plane to the clockwise or anti-clockwise direction.
`transform: rotate3d(x, y, z, angle)`
`transform: rotate3d(1, 1, 1, 30deg)`

#### scale3d()

The scale3d() method scales the element i.e increases or decreases the size of an element in three-dimensional space along all the axes. It changes the width, height, and depth of the element.
`transform: scale3d(x, y, z)`

[CSS 3D Transforms](https://www.programiz.com/css/3d-transform)

### CSS Transition

CSS transitions enable smooth changes in the CSS property values over the specified duration.
For example,

```
div {
    background-color: orange;
    transition: background-color 1s linear;
}

div:hover {
    background-color: red;
}
```

CSS transition includes the following properties:

#### transition-property -

`transition-property: none | all | property-name`

#### transition-duration -

`transition-duration: time-value`

#### transition-timing-function -

`transition-timing-function: timing-function`

Here, `timing-function` represents any of the following values:

`ease`: transition starts slowly, accelerates at the middle, and slowly ends
`linear`: specifies the constant transition speed throughout the duration
`ease-in`: specifies the transition with a slow start and fast end
`ease-out`: specifies the transition with a fast start and slow end
`ease-in-out`: specifies the transition with a slow start and end
`step-start`: specifies the transition with an instant beginning that remains constant throughout the end
`step-end`: specifies the transition with a constant beginning that ends instantly
`steps(int, start | end)`: represents transition with stepped timing function and defined interval
`cubic-bezier`: defines a custom transition with specified values

#### transition-delay -

`transition-delay: time_value`

#### transition (shorthand property) -

`transition: [transition-property] [transition-duration] [transition-timing-function] [transition-delay]`

For Example -
`transition: width 2s linear 1s;` is equivalent to,

```
transition-property: width;
transition-duration: 2 seconds;
transition-timing-function: linear;
transition-delay : 1 second;
```

[CSS Transitions](https://www.programiz.com/css/transitions)

### CSS Animation Properties

CSS animation has the following properties:

#### @keyframe rule

```
@keyframes animate-background {
  0% {
    background-color: orange;
  }
  100% {
    background-color: red;
  }
}
```

#### animation-name

`animation-name: animate-background` specifies the animation name

#### animation-duration

`animation-duration: 5s` specifies the animation duration

#### animation-delay

`animation-delay: 2s;`

#### animation-iteration-count

The `animation-iteration-count` property specifies the number of times the animation should be played.
The value of the `animation-iteration-count` property can be specified in the `integers` or `once` and `infinite` keywords.

#### animation-direction

The `animation-direction` property specifies the direction for the animation.

The possible values for the animation-direction property are:
`normal`: animation plays forward, default value
`reverse`: animation plays backward
`alternate`: animation alternates between forward and backward
`alternate-reverse`: animation alternates between backward and forward

#### animation-timing-function

The `animation-timing-function` property specifies how the intermediate property values are calculated during the animation duration.

The `animation-timing-function` property has the following values:

`ease`, `ease-in`, `ease-out`, `ease-in-out`,`linear`, `cubic-bezier(n, n, n, n)`

#### animation-fill-mode

The `animation-fill-mode` property decides how the animation applies to an element before and after the animation.

By default, the animation only affects the targeted element during the animation duration.

The `animation-fill-mode` property has the following possible values:

`none`: no styles are applied before and after the animation (default value)
`forwards`: styles of the last keyframes are applied after the animation
`backwards`: styles of the first keyframe are applied after the animation
`both`: applies styles both before and after the animation

#### animation

The `animation` property is a shorthand property that combines multiple animation-related properties into a single declaration.

The syntax of the animation property is as follows:
`animation: animation-name duration timing-function delay iteration-count direction fill-mode;`

e.g. -

```
.container:hover .inner-div {
    /* shorthand animation property */
    animation: animate-div 2s ease-in-out 0.1s 3 alternate forwards;
}
@keyframes animate-div {
    0% {
        left: 0%;
    }
    100% {
        left: 80%;
    }
}
```

[CSS Animations](https://www.programiz.com/css/animations)

## Animating with Framer Motion -

import { motion } from 'framer-motion';

### Animating between conditional values

[Framer Motion Docs](https://www.framer.com/motion/introduction/)

```
  <motion.span
  animate={{ rotate: isExpanded ? 180 : 0 }}
  className="challenge-item-details-icon"
>
```

### Adding/Disappearing Entry Animations

[AnimatePresence Docs](https://www.framer.com/motion/animate-presence/)

```
<AnimatePresence>
  {isVisible && (
    <motion.div
      initial={{ opacity: 0 }}
      animate={{ opacity: 1 }}
      exit={{ opacity: 0 }}
    />
  )}
</AnimatePresence>
```

### Hover Animation

```
<motion.button
  whileHover={{ scale: 1.1 }}
  transition={{ type: 'spring', stiffness: 500 }}
  onClick={handleStartAddNewChallenge}
  className="button"
>
```

### Variants

[Variants Docs](https://www.framer.com/motion/animation/#variants)
Setting `animate` as an object is useful for simple, single-component animations. But sometimes we want to create animations that propagate throughout the DOM, and orchestrate those animations in a declarative way. We can do so with variants.

```
<motion.div
  initial="hidden"
  animate="visible"
  variants={{
    visible: { opacity: 1 },
    hidden: { opacity: 0 },
  }}
/>
```

#### Propagation

If a `motion` component has children, changes in variant will flow down through the component hierarchy until a child component defines its own `animate` property.

```
const list = {
  visible: { opacity: 1 },
  hidden: { opacity: 0 },
}

const item = {
  visible: { opacity: 1, x: 0 },
  hidden: { opacity: 0, x: -100 },
}

return (
  <motion.ul
    initial="hidden"
    animate="visible"
    variants={list}
  >
    <motion.li variants={item} />
    <motion.li variants={item} />
    <motion.li variants={item} />
  </motion.ul>
)
```

### staggerChildren: number

When using variants, animations of child components can be staggered by this duration (in seconds).

For instance, if `staggerChildren` is `0.01`, the first child will be delayed by `0` seconds, the second by `0.01`, the third by `0.02` and so on.

The calculated stagger delay will be added to `delayChildren`.

```
const container = {
  hidden: { opacity: 0 },
  show: {
    opacity: 1,
    transition: {
      staggerChildren: 0.5
    }
  }
}

const item = {
  hidden: { opacity: 0 },
  show: { opacity: 1 }
}

return (
  <motion.ol
    variants={container}
    initial="hidden"
    animate="show"
  >
    <motion.li variants={item} />
    <motion.li variants={item} />
  </motion.ol>
)
```

### Keyframes

[KeyFrames Docs](https://www.framer.com/motion/animation/##keyframes)

Values in `animate` can also be set as a series of keyframes. This will animate through each value in sequence.

```
<motion.div
  animate={{ x: [0, 100, 0] }}
/>
```

We can use the current value as the initial keyframe by passing a **wildcard keyframe**, `null`.

```
<motion.div
animate={{ x: [null, 100, 0] }}
/>
```

This way, if a keyframes animation starts while the value is currently animating, the transition will be more natural. It also reduces duplication in our code.

### useAnimate() hook

[useAnimate docs](https://www.framer.com/motion/use-animate/)

`useAnimate` provides a way of using the animate function that is scoped to the elements within your component.

It provides a `scope` ref, and an `animate` function where every DOM selector is scoped to this ref.

```import useAnimate hook
import { useAnimate, stagger } from 'framer-motion';
```

```
const [scope, animate] = useAnimate();
```

```calling animate function
...
      animate(
        'input, textarea',
        { x: [-10, 0, 10, 0] },
        { type: 'spring', duration: 0.2, delay: stagger(0.05) }
      );
...
```

```
<form id="new-challenge" onSubmit={handleSubmit} ref={scope}>
<p>
  <label htmlFor="title">Title</label>
  <input ref={title} type="text" name="title" id="title" />
</p>
...
</form>
```

#### stagger

A function for staggering animations across elements.

When animating elements with the `animate` function, it's possible to stagger animations across them using stagger().

When animating more than one element, pass `stagger` to the `delay` option.

```
animate("li", { opacity: 1 }, { delay: stagger(0.1) })
```

### Layout animations

Create layout and shared layout animations with React and Framer Motion.

Framer Motion can animate between any CSS layout by using performant transforms instead of the layout system.

For example, this component is animated by switching `justify-content` between `flex-start` and `flex-end`.

To enable Framer Motion's layout animations, we simply set the `layout` prop of a `motion` component.

```
<motion.div layout />
```

Any layout change that happens as the result of a re-render will be animated. That could be any combination of:

- Reordering of a list.
- A style set on the component itself, for example a change in `width` or `position`.
- A change in the parent's layout, e.g. `flexbox` or `grid`.
- Or any other change in the component's layout.

### AnimatePresence

[AnimatePresence Docs](https://www.framer.com/motion/animate-presence/)

`AnimatePresence` allows components to animate out when they're removed from the React tree.
It's required to enable exit animations because React lacks a lifecycle method that:

- Notifies components when they're going to be unmounted and
- Allows them to defer that unmounting until after an operation is complete (for instance an animation).

#### Multiple children

`AnimatePresence` works the same way with multiple children. Just ensure that each has a unique `key` and components will animate in and out as they're added or removed from the tree.

#### mode: "sync" | "wait" | "popLayout"

Decides how AnimatePresence handles entering and exiting children.

- `"sync"`: (Default) Children animate in/out as soon as they're added/removed.
- `"wait"`: The entering child will wait until the exiting child has animated out. Note: Currently only renders a single child at a time.
- `"popLayout"`: Exiting children will be "popped" out of the page layout. This allows surrounding elements to move to their new layout immediately.

### Shared layout animations

When a new component is added that has a `layoutId` prop that matches an existing component, it will automatically animate out from the old component.

```
isSelected && <motion.div layoutId="underline" />
```

### Re-Triggering Animation via Keys

setting the key and updating it to a different value will recreate the component and therefore be used to rerun entry animation.

### useScroll

Create scroll-linked animations with the useScroll hook.

`useScroll` is used to create scroll-linked animations, like progress indicators and parallax effects.

`useScroll` returns four [motion values](https://framer.com/motion/motionvalue/):

`scrollX`/`scrollY`: The absolute scroll position, in pixels.
`scrollXProgress`/`scrollYProgress`: The scroll position between the defined offsets, as a value between 0 and 1.

```
import { useScroll } from "framer-motion";

const { scrollY } = useScroll();
```

### useTransform

[useTramsform Docs](https://www.framer.com/motion/use-transform/)
`useTransform` creates a `MotionValue` that takes the output of one or more other `MotionValues` and changes it some way.

#### Mapping

`useTransform` can also map a motion value from one range of values to another.

To illustrate, look at this `x` motion value:

```
useTransform(value, input, output, options)
```

We can use `useTransform` to create a new motion value called `opacity`. By defining an input range and an output range we can say, "when `x` is `0`, `opacity` should be `1`. When `x` is `100`, `opacity` should be `0`."

```
const opacity = useTransform(
  x,
  [0, 100], // Map x from these values
  [1, 0]  // Into these values
)
```

Now, if `x` gets set to `50`, `opacity` will be `0.5`.

**`motion` components have enhanced `style` props, allowing you to set them individually there, too.**

#### Parallax effect

```
import { motion, useScroll, useTransform } from 'framer-motion';
```

```
  const { scrollY } = useScroll();

  const yCity = useTransform(scrollY, [0, 200], [0, -100]);
  const opacityCity = useTransform(
    scrollY,
    [0, 200, 300, 500],
    [1, 0.5, 0.5, 0]
  );
  const yHero = useTransform(scrollY, [0, 200], [0, -150]);
  const opacityHero = useTransform(scrollY, [0, 300, 500], [1, 1, 0]);
  const yText = useTransform(scrollY, [0, 200, 300, 500], [0, 50, 50, 300]);
  const scaleText = useTransform(scrollY, [0, 300], [1, 1.5]);
```

```
  <header id="welcome-header">
    <motion.div
      id="welcome-header-content"
      style={{ scale: scaleText, y: yText }}
    >
      <h1>Ready for a challenge?</h1>
      <Link id="cta-link" to="/challenges">
        Get Started
      </Link>
    </motion.div>
    <motion.img
      style={{ opacity: opacityCity, y: yCity }}
      src={cityImg}
      alt="A city skyline touched by sunlight"
      id="city-image"
    />
    <motion.img
      style={{ y: yHero, opacity: opacityHero }}
      src={heroImg}
      alt="A superhero wearing a cape"
      id="hero-image"
    />
  </header>
```
