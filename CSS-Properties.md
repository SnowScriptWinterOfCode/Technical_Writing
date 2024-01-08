<b><H1>Documentation on various CSS properties</H1></b>
<b><h1>(1)Introduction to CSS</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/648b6d9f-6305-4710-8e1b-773015945de6)

What is CSS?

CSS stands for Cascading Style Sheets. It's a style language used to describe the presentation of a document written in HTML. CSS allows developers to control the layout, formatting, and appearance of multiple web pages all at once.


<b><h1>(2)Role in Web Development</h1></b>
CSS plays a crucial role in web development by separating the content (HTML) from its presentation (CSS). It enhances the visual aspects of a web page, making it more appealing, readable, and user-friendly.
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/4038a3fd-1f3c-4776-a692-d552af68ea10)


<b><h1>(3)Basic Syntax</b></h1>
CSS consists of style rules that define how HTML elements are displayed. It follows a simple structure:
 code:
selector {
    property: value;
}
<b><h1>(4)Selector: Targets HTML elements to apply styles.</b></h1>
Property: Attribute being modified (e.g., color, font-size).
Value: Specific setting for the property (e.g., blue, 16px).
Different Types of Selectors
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/3c811df7-8ead-469b-9c6c-f75ae7a2a7dc)

Element Selector: Targets HTML elements directly (e.g., p { color: blue; }).
Class Selector: Uses classes (.class) for more specific styling (e.g., .highlight { background-color: yellow; }).
ID Selector: Selects elements with a specific ID (#id) (e.g., #header { font-size: 24px; }).
Attribute Selector: Selects elements based on their attributes (e.g., input[type="text"] { border: 1px solid black; }).
How to Include Styles
There are three main methods to include CSS styles:

Inline CSS: Apply styles directly to HTML elements using the style attribute.
html
code:
<!-- <p style="color:red;">This is a red paragraph.</p> -->

Internal CSS: Place CSS within the <style> tag in the HTML <head> section.
 code:
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>
External CSS: Link an external CSS file using the <link> tag.
 code:
<head>
    <link rel="stylesheet" href="styles.css">
</head>
Understanding these basics will set you on the right path to start styling your web pages with CSS

<b><h1>(5). Basic CSS Properties</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/6b853acb-5a67-4a54-84df-11ec6b9ee291)

Color Property
The color property sets the text color within an element.

css
code
p {
    color: blue;
}
Background Color
The background-color property defines the background color of an element.

css code
body {
    background-color: #f1f1f1;
}
Text Properties
Font Family: font-family defines the font used for text.
css code
body {
    font-family: Arial, sans-serif;
}
Font Size: font-size sets the size of the font.
css code
h1 {
    font-size: 24px;
}
Font Weight: font-weight specifies the thickness of the font.
css code
strong {
    font-weight: bold;
}
Text Alignment: text-align aligns text within an element.
css
code
.centered {
    text-align: center;
}
<b><h1>(6)Units in CSS</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/6dce1911-d9b3-4c47-934a-143b83b5bcdb)

Pixels (px): Absolute unit, commonly used for precise sizes.
Ems (em): Relative unit based on the font size of the element.
Rems (rem): Relative unit based on the font size of the root element.
Percentages (%): Relative to the parent element's size.
Viewport Units (vh, vw): Relative to the viewport's height or width.
css
code:
.container {
    width: 80%; /* Percentage */
    padding: 20px; /* Pixels */
    font-size: 1.2em; /* Relative to parent font size */
}
Understanding these basic properties and units will help you control the appearance of text and backgrounds on your web pages.

<b><h1>(7) Box Model and Layout Properties</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/8d00526c-4413-4cf3-8494-ea2a0b188b9c)

Box Model
The box model describes how elements are structured and spaced within the layout.

Height and Width: height and width set the height and width of an element.

css
code:
.box {
    height: 100px;
    width: 200px;
}
Border: border defines the border around an element.

css code:
.box {
    border: 1px solid black;
}
Padding: padding creates space inside the element's border.

css code:
.box {
    padding: 10px;
}
Margin: margin sets space outside the element's border.

css code:
.box {
    margin: 20px;
}
<b><h1>(8)Display Property</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/05d7b85a-7654-4196-a1b0-575130f30534)

display: Determines how an element is displayed.

block: Takes up the full width available, starts on a new line.

inline: Takes up only as much width as necessary, doesn't start a new line.

inline-block: Behaves like an inline element but allows for block-level styling.

Visibility and Positioning

visibility: Controls the visibility of an element.

css code
.hidden {
    visibility: hidden;
}
<b><h1>(9)position: Determines the type of positioning for an element.</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/ea9bf64c-7b83-4bc1-8e87-2bef47116faa)


static: Default position, follows the normal document flow.

relative: Positioned relative to its normal position.

absolute: Positioned relative to the nearest positioned ancestor.

fixed: Positioned relative to the viewport.

z-index: Sets the stack order of positioned elements.

css code:
.higher {
    z-index: 999;
}
Background Image and Size
background-image: Sets a background image for an element.

css
code:
.bg {
    background-image: url('image.jpg');
}
background-size: Adjusts the size of the background image.

css code:
.bg {
    background-size: cover; /* or contain, auto, etc. */
}
Understanding these box model properties, along with display, visibility, positioning, and background-related properties, allows you to structure and style elements effectively within your web layout.
<b><h1>(10). Flexbox Model:</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/94ef4d8c-89c3-4180-b240-65f15c95a828)

Definition
Flexbox is a layout model in CSS that allows creating flexible and responsive layouts. It provides a more efficient way to distribute space among items in a container, even when their size is unknown or dynamic.

Flexbox Direction:
flex-direction: Defines the direction of the flex container and how flex items are placed within it.
row: Items are placed in rows (default).
row-reverse: Items are placed in rows but reversed.
column: Items are placed in columns.
column-reverse: Items are placed in columns but reversed.
css code:
.container {
    display: flex;
    flex-direction: row; /* or column, row-reverse, column-reverse */
}
Flex Properties:
justify-content: Aligns flex items along the main axis.

flex-start: Items are packed toward the start of the flex container.

flex-end: Items are packed toward the end of the flex container.

center: Items are centered in the flex container.

space-between: Items are evenly distributed with the first item at the start and the last item at the end.

space-around: Items are evenly distributed with equal space around them.

align-items: Aligns flex items along the cross axis.

flex-start: Items are aligned at the start of the cross axis.
flex-end: Items are aligned at the end of the cross axis.
center: Items are centered along the cross axis.
baseline: Items are aligned based on their baseline.
stretch: Items are stretched to fill the container.
css
 code:
.container {
    display: flex;
    justify-content: space-between; /* or center, flex-start, flex-end, space-around */
    align-items: center; /* or flex-start, flex-end, center, baseline, stretch */
}
Flex Items Properties:
flex-grow: Specifies the ability of a flex item to grow.
flex-shrink: Specifies the ability of a flex item to shrink.
flex-basis: Specifies the initial size of a flex item before it's placed in a flex container.
css
 code:
.item {
    flex-grow: 1;
    flex-shrink: 0;
    flex-basis: auto;
}
Understanding these Flexbox properties helps in creating flexible and responsive layouts easily. Flexbox simplifies the alignment and distribution of space among items within a container, making it a powerful tool for web layout design. 

<b><h1>(11). Media Queries and Responsive Design</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/a01a4941-bbc8-48f0-ab65-df43bdc67970)

Media Queries:
Media queries allow the presentation of content to be tailored to a specific range of devices or conditions, such as screen width, height, device orientation, etc.

Syntax:
css
code:

/* Basic Media Query */
@media screen and (max-width: 600px) {
    /* CSS rules for screens with a maximum width of 600px */
    body {
        font-size: 14px;
    }
}

Types of Media Features:

Width and Height: max-width, min-width, max-height, min-height.

Device Orientation: orientation: portrait, orientation: landscape.

Device Aspect Ratio: aspect-ratio, min-aspect-ratio, max-aspect-ratio.

Device Resolution: resolution.


Responsive Frameworks (e.g., Tailwind CSS)
Frameworks like Tailwind CSS provide a set of pre-defined CSS classes and components to facilitate rapid development of responsive websites.

Example Usage (Tailwind CSS):
html
css code:
<div class="lg:flex lg:justify-between lg:items-center">
    <div class="lg:w-1/2">
        <!-- Content for large screens (width >= 1024px) -->
    </div>
    <div class="lg:w-1/2">
        <!-- Content for large screens (width >= 1024px) -->
    </div>
</div>
Responsive Grid Systems: Offer classes for defining grid layouts for different screen sizes.

Utility Classes: Provide classes for responsive text, padding, margin, visibility, etc., based on screen sizes.

Benefits of Responsive Design:

Improved User Experience: Content adapts to various devices.

Better SEO: Responsive sites often rank higher in search engines.

Easier Maintenance: Single codebase for multiple devices.

Utilizing media queries and frameworks like Tailwind CSS allows developers to create websites that seamlessly adapt to different devices and screen sizes. They simplify the process of building responsive designs by providing a structured approach and reusable components. Experimenting with these techniques will help in mastering responsive web design!


<b><h1>(12) Transformations and Animations in CSS:</h1></b>
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/9d8023d3-355b-4d7f-9654-6208f12aa4c1)


Transformations:
CSS transform property allows you to modify the appearance of an element by applying various transformations.

Common Transform Functions:
scale(): Changes the size of an element.
css
code:
.box {
    transform: scale(1.2); /* Increases size by 20% */
}
rotate(): Rotates an element by a specified angle.
css code:
.shape {
    transform: rotate(45deg); /* Rotates element by 45 degrees */
}
translate(): Moves an element along the x and y-axis.
css code:
.object {
    transform: translate(50px, 20px); /* Moves element 50px right and 20px down */
}
skew(): Skews an element along the x and y-axis.
css code:
.element {
    transform: skew(10deg, 20deg); /* Skews element by specified degrees */
}
Animation Property and Syntax
CSS animation property allows creating animations by gradually changing an element's style over time.

Syntax:
css
code:
/* Define animation keyframes */
@keyframes animationName {
    from {
        /* Initial styles */
    }
    to {
        /* Final styles */
    }
}

/* Apply animation to an element */
.element {
    animation-name: animationName;
    
    animation-duration: 2s; /* Duration of animation */

    animation-delay: 1s; /* Delay before animation starts */
    
    animation-direction: normal; /* Direction of animation */
    
    /* Other animation properties */
}
Animation Properties:

animation-name: Specifies the name of the animation.

animation-duration: Duration of the animation in seconds or milliseconds.

animation-delay: Delay before the animation starts.

animation-direction: Specifies whether the animation plays forward, backward, or alternates.

animation-timing-function: Defines the pace of the animation (e.g., ease, linear, ease-in-out).

animation-iteration-count: Number of times the animation should repeat (infinite for continuous).
Example:
css
 code:
@keyframes move {
    from {
        transform: translateX(0);
    }
    to {
        transform: translateX(100px);
    }
}

.element {
    animation-name: move;

    animation-duration: 2s;

    animation-delay: 1s;

    animation-direction: alternate;

    animation-timing-function: ease-in-out;

    animation-iteration-count: infinite;
}

Mastering CSS transformations and animations allows you to add interactive and visually appealing elements to your web pages. Experimenting with different transformation functions and animation properties can lead to captivating effects!
