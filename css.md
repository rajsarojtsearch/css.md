CSS Interview Questions and Answers💖💖

Navigation Menu
interview

Code
Issues
Pull requests
interview
/css.md
tecresearch
tecresearch
4 months ago
360 lines (261 loc) · 16.5 KB

*Preview Code Blame*
CSS Interview Questions and Answers
Basic Questions:
What is the difference between relative, absolute, and fixed positioning in CSS?

relative: Positions the element relative to its normal position.
absolute: Positions the element relative to its nearest positioned ancestor.
fixed: Positions the element relative to the viewport, staying in place when scrolling.
What is the difference between em, rem, %, and px in CSS?

px: Absolute unit of measurement.
em: Relative to the parent element's font-size.
rem: Relative to the root element (html) font-size.
%: Relative to the parent container's dimension.
What is the difference between flexbox and grid in CSS?

Flexbox is one-dimensional (row or column layout).
Grid is two-dimensional (both rows and columns).
What are pseudo-classes and pseudo-elements in CSS?

Pseudo-classes (e.g., :hover, :nth-child()) target elements based on state or position.
Pseudo-elements (e.g., ::before, ::after) style parts of elements.
What is the difference between visibility: hidden and display: none?

visibility: hidden hides the element but keeps its space.
display: none removes the element from the layout.
How does the z-index property work in CSS?

z-index controls the stacking order of elements. Higher values appear on top.
What is the difference between min-width, max-width, and width?

width: Fixed width.
min-width: Minimum width the element can shrink to.
max-width: Maximum width the element can grow to.
What are media queries in CSS?

Media queries allow CSS to be applied based on screen size, resolution, or device type.
Example: @media (max-width: 600px) { body { background-color: red; } }
What is the difference between inline, block, and inline-block elements?

inline: Does not allow width/height changes, flows with text.
block: Takes full width, starts on a new line.
inline-block: Allows width/height changes but stays inline.
What is the difference between absolute, relative, and sticky positioning?

absolute: Positioned relative to the nearest positioned ancestor.
relative: Positioned relative to itself.
sticky: Sticks to a position while scrolling until its parent container scrolls out of view.
Advanced Questions:
How does CSS specificity work?

Inline styles (1000), ID selectors (100), class/pseudo-classes (10), element selectors (1).
What are CSS transitions and animations?

Transitions allow smooth property changes (transition: all 0.3s ease-in-out;).
Animations allow keyframe-based animations (@keyframes move { 0% { left: 0; } 100% { left: 100px; } }).
What is a CSS preprocessor?

A tool like Sass or LESS that extends CSS with variables, mixins, and nested syntax.
How do CSS variables work?

--main-color: red; defined in :root and used as color: var(--main-color);.
What is the difference between vh, vw, and % in CSS?

vh and vw are relative to the viewport. % is relative to the parent element.
How do you make a website responsive without using a framework?

Use flexbox/grid, media queries, percentage-based widths, and responsive images.
What are the benefits of using CSS sprites?

Reduces HTTP requests, improves performance.
What is the difference between object-fit and object-position in CSS?

object-fit: Defines how an image fits in a container.
object-position: Defines the position of the image within the container.
What are the different types of CSS units?

Absolute (px, pt, cm), Relative (%, em, rem, vw, vh).
How does the clip-path property work?

Defines a clipping area for an element, allowing for non-rectangular shapes.
Complex & Logical Questions:
How would you create a pure CSS tooltip that appears on hover?

.tooltip { position: relative; display: inline-block; }
.tooltip .tooltip-text {
    visibility: hidden; background-color: black; color: white; 
    position: absolute; bottom: 100%; left: 50%; transform: translateX(-50%);
}
.tooltip:hover .tooltip-text { visibility: visible; }
How do you create a full-page background image without distortion?

body { background: url('image.jpg') no-repeat center center/cover; }
How do you make a div perfectly centered using flexbox?

.container { display: flex; justify-content: center; align-items: center; height: 100vh; }
How would you create a responsive navbar using CSS only?

Use flexbox with media queries for toggling visibility.
How can you make text overflow with ellipsis (...) in CSS?

.text-overflow { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
What are the best practices for improving CSS performance?

Minify CSS, use shorthand properties, limit use of @import, optimize selectors.
How do you create a button with an animated ripple effect in CSS?

button:active::after {
    content: ''; width: 100px; height: 100px; background: rgba(0, 0, 0, 0.3);
    position: absolute; border-radius: 50%; transform: scale(0);
    animation: ripple 0.5s linear;
}
@keyframes ripple { 100% { transform: scale(4); opacity: 0; } }
What is the difference between contain and cover in background-size?

contain: Ensures the image fits completely inside the container.
cover: Ensures the image covers the entire container without distortion.
How do you create a sticky footer using CSS?

html, body { height: 100%; }
.content { min-height: calc(100vh - 50px); }
.footer { height: 50px; }
How do you implement a dark mode toggle using only CSS?

Use CSS variables and media queries for dark mode, toggled using JavaScript.
CSS Interview Questions and Answers

Q: What is CSS?
A:
CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of HTML documents.

Q: What are the different types of CSS?
A:
Inline CSS, Internal CSS, and External CSS.

Q: What is the difference between relative, absolute, and fixed positioning in CSS?
A:
Relative: Positioned relative to its normal position.
Absolute: Positioned relative to the nearest positioned ancestor.
Fixed: Positioned relative to the viewport, remains in place when scrolling.

Q: What is the difference between em, rem, %, and px in CSS?
A:
 em: Relative to the font size of the parent.
 rem: Relative to the root element’s font size.
 %: Relative to the parent element.
 px: Absolute unit, fixed size.

Q: How does the z-index property work?
A:
 The z-index property specifies the stack order of elements. Higher values bring elements forward.

Q: What is Flexbox in CSS?
A:
 Flexbox is a CSS layout module designed for distributing space and aligning items efficiently.

Q: What are media queries in CSS?
A:
 Media queries allow applying styles based on device characteristics like width, height, and resolution.

Q: Explain the difference between nth-child and nth-of-type. 
A:
  nth-child(n): Selects the nth child of its parent.
  nth-of-type(n): Selects the nth occurrence of a specific tag type within its parent.
  
Q: What is Grid Layout in CSS? 
A:
 CSS Grid Layout is a two-dimensional layout system for placing elements in rows and columns.

Q: How can you create a responsive design using CSS? 
A:
 Use flexible units (em, %), media queries, Flexbox, and Grid.

Q: What is the difference between max-width and min-width? 
A:
 max-width: Specifies the maximum width an element can have.
 min-width: Specifies the minimum width an element can have.
 
Q: What is the difference between visibility: hidden and display: none?
A:
 visibility: hidden: Hides the element but it still takes up space.
 display: none: Hides the element and removes it from the document flow.
 
Q: What is pseudo-class in CSS?
A:
 A pseudo-class defines a special state of an element (e.g., :hover, :focus).

Q: What is a pseudo-element in CSS?
A:
 A pseudo-element allows styling a specific part of an element (e.g., ::before, ::after).

Q: What is the difference between inline, block, and inline-block elements?
A:
 inline: Does not start on a new line, respects width of content.
 block: Starts on a new line, takes full width.
 inline-block: Behaves like inline but allows setting width and height.
 
Q: What is the difference between opacity and rgba? 
A:
 opacity: Affects the entire element’s transparency.
 rgba: Affects only the element’s background transparency.
 
Q: What is a sticky element in CSS?
A:
 A position: sticky element stays fixed when scrolling within a specified boundary.

Q: How can you center an element vertically and horizontally?
A:
 Use display: flex and justify-content: center; align-items: center;.

Q: What is the difference between hover and focus?
A:
 hover applies styles when the mouse is over an element; focus applies styles when an element is focused.

Q: What are keyframes in CSS animations?
A:
 Keyframes define animation states and transitions between them.

Q: How can you create a CSS animation?
A:
 Use @keyframes with animation-name and animation-duration properties.

Q: What is clip-path in CSS?
A:
 The clip-path property is used to define a clipping region for an element.

Q: What is the difference between relative and absolute units in CSS?
A:
Relative units (em, %, rem) depend on another element.
Absolute units (px, cm, in) have fixed values.

Q: What is the difference between inherit, initial, and unset?
A:
inherit: Inherits the value from the parent.
initial: Resets to the default CSS property value.
unset: Acts as inherit for inherited properties, and initial otherwise.

Q: How does the object-fit property work?
A:
Defines how an <img> or <video> fits inside its container (cover, contain, fill).

Q: What is the difference between absolute and fixed positioning?
A:
absolute: Positioned relative to the nearest ancestor with position: relative.
fixed: Positioned relative to the viewport.

Q: How does overflow work in CSS?
A:
Controls content that overflows an element (visible, hidden, scroll, auto).

Q: What is the difference between static, relative, absolute, and fixed positioning?
A:
static: Default, follows normal document flow.
relative: Relative to its normal position.
absolute: Relative to the nearest positioned ancestor.
fixed: Relative to the viewport.
Q: What is the difference between vw and vh?
A:
 vw: Viewport width percentage.
 vh: Viewport height percentage.
 
Q: What is the difference between linear-gradient and radial-gradient?
A:
 linear-gradient: Creates a gradient in a straight line.
 radial-gradient: Creates a circular or elliptical gradient.
 CSS INTERVIEW QUESTIONS AND ANSWERS

Q: What is CSS and why is it used?
A:
 CSS (Cascading Style Sheets) is used to style HTML elements, controlling layout, colors, and typography to enhance user experience.

Q: What are the different types of CSS?
A:
 Inline CSS, Internal CSS, and External CSS.

Q: Explain the difference between relative, absolute, and fixed positioning in CSS.
A:
 Relative is positioned relative to its normal position, absolute is positioned relative to the nearest positioned ancestor, and fixed is positioned relative to the viewport.

Q: What is the difference between ‘em’, ‘rem’, and ‘px’ units in CSS?
A:
 ‘em’ is relative to the font-size of the parent, ‘rem’ is relative to the root element’s font-size, and ‘px’ is an absolute unit.

Q: What is the difference between ‘visibility: hidden’ and ‘display: none’?
A:
 ‘visibility: hidden’ hides the element but it still takes up space, whereas ‘display: none’ removes the element from the document flow.

Q: What is Flexbox and why is it useful?
A:
Flexbox is a layout model that allows easy alignment and distribution of elements in a container, making responsive designs easier.

Q: How does Grid layout differ from Flexbox?
A:
 Grid is two-dimensional (rows and columns), whereas Flexbox is one-dimensional (either row or column).

Q: What is the difference between min-width, max-width, and width?
A:
 ‘min-width’ sets the minimum width, ‘max-width’ sets the maximum width, and ‘width’ sets a fixed width.

Q: Explain the difference between ‘nth-child()’ and ‘nth-of-type()’.
A:
 ‘nth-child()’ selects based on position among all siblings, while ‘nth-of-type()’ selects based on type.

Q: What are pseudo-classes in CSS?
A:
 Pseudo-classes define a special state of an element, such as :hover, :focus, and :nth-child().

Q: How can you make an element responsive using CSS?
A:
 Use relative units like %, em, rem, and flexbox/grid along with media queries.

Q: What is the difference between ‘relative’, ‘absolute’, and ‘fixed’ positioning?
A:
 Relative positions an element relative to itself, absolute relative to its parent, and fixed relative to the viewport.

Q: What are pseudo-elements in CSS?
A:
 Pseudo-elements allow styling specific parts of an element, like ::before and ::after.

Q: How does z-index work?
A:
 z-index controls the stack order of elements; higher values appear in front.

Q: What is the difference between ‘inline’, ‘block’, and ‘inline-block’ elements?
A:
 Inline does not allow setting width/height, block takes full width, and inline-block allows both inline and block properties.

Q: What is the difference between ‘opacity’ and ‘visibility’ in CSS?
A:
Opacity makes an element transparent but still interactive, while visibility hides it but keeps its space.

Q: Explain the use of media queries in CSS.
A:
 Media queries apply styles based on screen size, enabling responsive designs.

Q: What are CSS transitions?
A:
 CSS transitions allow smooth property changes over a defined duration.

Q: What is the difference between ‘transform’ and ‘transition’ in CSS?
A:
 ‘transform’ modifies elements (scale, rotate), while ‘transition’ animates changes smoothly.

Q: What is the difference between ‘position: sticky’ and ‘position: fixed’?
A:
 Sticky remains fixed within its parent until a threshold is reached, whereas fixed stays at a position relative to the viewport.

Q: What is the purpose of the ‘clip-path’ property? 
A:
 It clips an element into a specific shape (circle, polygon, etc.).

Q: Explain the difference between ‘grid-template-columns’ and ‘grid-auto-columns’. 
A:
 ‘grid-template-columns’ defines the structure, while ‘grid-auto-columns’ handles dynamically added items.

Q: How can you create a CSS animation? 
A:
 Use @keyframes and apply animation properties like duration and delay.

Q: What are the differences between ‘rem’ and ‘em’ in CSS?
A:
 ‘rem’ is relative to the root element, while ‘em’ is relative to its parent.

Q: How do you implement a sticky footer using CSS?
A:
 Use flexbox with ‘min-height: 100vh’ and ‘flex-grow: 1’ for the content section.

Q: What are the different values for the ‘overflow’ property?
A:
 visible, hidden, scroll, auto.

Q: What is a CSS variable and how is it defined?
A:
 CSS variables store reusable values and are defined using ‘--var-name’ syntax.

Q: How does ‘pointer-events’ work in CSS? 
A:
 It controls whether an element can receive mouse events.

Q: Explain the concept of layering in CSS with examples.
A:
 Layering is controlled by ‘z-index’ where higher values appear in front.

Q: What is the ‘object-fit’ property in CSS? 
A:
 It controls how an image or video fits within a container.
