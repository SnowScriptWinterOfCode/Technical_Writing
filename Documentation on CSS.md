# CSS Technical Documentation

## 1. Introduction

CSS (Cascading Style Sheets) is a stylesheet language used for describing the look and formatting of a document written in HTML or XML. It allows web developers to control the presentation of web pages, including the layout, colors, and fonts.

## 2. Basic Syntax

CSS consists of a set of rules that define the styling of HTML elements. A CSS rule is composed of a selector and a declaration block. Example:
```
   selector {
        property: value;
    } 
```


## 3. Selectors

CSS selectors are patterns that are used to select and style HTML elements on a web page. Selectors target specific elements based on their type, attributes, class, ID, or relationship with other elements in the HTML document.

### 3.1 Type Selector

```
p {
  /* Styles for all <p> elements */
}
```

### 3.2 Class Selector

Selects elements with a specific class attribute.

```
.highlight {
  /* Styles for elements with class="highlight" */
}
```

### 3.3 ID Selector

Selects a single element with a specific ID attribute.

```
#header {
  /* Styles for the element with id="header" */
}
```

### 3.4 Attribute Selector

Selects elements based on their attributes.

```
input[type="text"] {
  /* Styles for <input> elements with type="text" */
}
```

### 3.5 Pseudo-classes

Selects elements based on their state or position.

```
a:hover {
  /* Styles for links when hovered over */
}
```

Pseudo-elements
Selects a specific part of an element.

```
p::first-line {
  /* Styles for the first line of <p> elements */
}
```

## 4. Properties

CSS properties define the visual styles and layout of HTML elements on a web page. Each property has a specific purpose, and values are assigned to these properties to determine how the elements should appear.

### 4.1 Color Properties

color: Sets the text color.
background-color: Sets the background color.

```
p {
  color: blue;
  background-color: #f0f0f0;
}
```

### 4.2	Typography Properties:

font-family: Specifies the font for text.
font-size: Sets the size of the font.
font-weight: Defines the thickness of the font.
```
h1 {
  font-family: "Arial", sans-serif;
  font-size: 24px;
  font-weight: bold;
}
```

### 4.3	Spacing Properties:

margin: Sets the outer margin of an element.
padding: Sets the inner spacing of an element.
```
div {
  margin: 10px;
  padding: 5px;
}
```

### 4.4	Border Properties:

border: Combines the properties for setting the width, style, and color of the border.
```
img {
  border: 1px solid #ccc;
}
```

### 4.5	Layout Properties:

width: Sets the width of an element.
height: Sets the height of an element.
display: Defines how an element is displayed.
```
.container {
  width: 80%;
  height: 400px;
  display: flex;
}
```

### 4.6	Positioning Properties:

position: Specifies the positioning method for an element.
top, right, bottom, left: Adjusts the position of an element.
```
.absolute-position {
  position: absolute;
  top: 10px;
  left: 20px;
}
```

### 4.7	Flexbox Properties:

display: flex: Enables flex container properties.
justify-content: Aligns items along the main axis.
align-items: Aligns items along the cross axis.
```
.flex-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

### 4.8	Grid Properties:

display: grid: Enables grid container properties.
grid-template-columns, grid-template-rows: Defines the size of columns and rows.
```
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

### 4.9	Media Query Properties:

@media: Defines styles for specific screen sizes or devices.
```
@media screen and (max-width: 600px) {
  body {
    font-size: 14px;
  }
}
```

## 5.	Box Model

The box model describes how elements are displayed on the page, including content, padding, border, and margin.

```
.box {
  width: 200px;
  height: 100px;
  padding: 10px;
  border: 1px solid #000;
  margin: 20px;
}
```

## 6.	Grid

CSS Grid Layout is a two-dimensional layout system that provides a powerful and flexible way to create grid-based layouts.
```
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}
```

## 7.	Flexbox

Flexbox is a layout model that allows for the design of complex layouts more efficiently.

## 8.	Layout

CSS provides various layout techniques, such as positioning, floats, and the more modern flexbox and grid.
```
/* Floats */
.float-left {
  float: left;
}

/* Flexbox */
.container {
  display: flex;
  justify-content: space-between;
}

/* Grid */
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
```

## 9.	Responsive Web Page

A responsive webpage in CSS refers to a design approach that ensures a website's layout and content adapt to different devices and screen sizes. The goal of responsive web design is to provide an optimal viewing and interaction experience, regardless of whether the user is accessing the site on a desktop computer, laptop, tablet, or smartphone.

## 10.	Conclusion

Styling Web Pages:
The primary purpose of CSS is to style HTML documents. It enables web developers to control the visual presentation of web pages, specifying how elements like text, images, links, and other HTML components should appear.



