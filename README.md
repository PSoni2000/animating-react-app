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

## Animating with only CSS -
