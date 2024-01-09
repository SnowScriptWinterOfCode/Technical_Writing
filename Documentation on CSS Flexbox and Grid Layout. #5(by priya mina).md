 <b><h1>documentation on CSS Flexbox and Grid Layout </h1></b>
<b><h2>Overview:</h2> </b>
 ![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/6b9d1d19-f619-45c0-880c-749cd5021aed)
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/3afda02e-1fb4-497b-b6bb-d3eeaf549831)



## CSS Flexbox:
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/6806769c-c530-4b2d-bb76-cce807384b03)


### Introduction to Flexbox
- **Definition:** Explain how Flexbox is a layout model that allows the creation of flexible and responsive layouts.
- **Main Concepts:** Discuss main concepts like flex containers and flex items.

### Properties of Flex Container
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/f8218a4b-4548-4176-a888-c65818300306)

1. **display:** Explain how to define an element as a flex container using `display: flex;`.
2. **flex-direction:** Detail the direction of flex items within the flex container (`row`, `row-reverse`, `column`, `column-reverse`).
3. **flex-wrap:** Describe how items wrap within the flex container (`nowrap`, `wrap`, `wrap-reverse`).
4. **justify-content:** Explain alignment along the main axis (`flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`).
5. **align-items:** Detail alignment along the cross axis (`flex-start`, `flex-end`, `center`, `baseline`, `stretch`).
6. **align-content:** Discuss alignment for multiple lines within the flex container (`flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `stretch`).

### Properties of Flex Items
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/1fdd3683-1b84-4898-9f31-1b281e73ce82)

1. **order:** Explain the order of individual flex items.
2. **flex-grow:** Detail how items grow relative to other items within the container.
3. **flex-shrink:** Describe how items shrink relative to other items within the container.
4. **flex-basis:** Specify the initial size of a flex item.
5. **flex:** Combine `flex-grow`, `flex-shrink`, and `flex-basis` into a shorthand property.
6. **align-self:** Explain how to override `align-items` on individual flex items.

## CSS Grid Layout
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/dc94b5f7-ca22-4754-910d-738020ff906b)


### Introduction to Grid Layout
- **Definition:** Explain how Grid Layout is a two-dimensional system for laying out elements in columns and rows.
- **Main Concepts:** Discuss grid containers, grid items, rows, columns, and tracks.

### Properties of Grid Container
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/b69d56b3-f963-479e-bd7b-a894aa846cfb)

1. **display:** Define an element as a grid container using `display: grid;`.
2. **grid-template-columns/grid-template-rows:** Specify the size of grid tracks (columns/rows).
3. **grid-gap:** Set the gap between grid tracks.
4. **justify-items:** Align grid items along the inline (row) axis.
5. **align-items:** Align grid items along the block (column) axis.
6. **justify-content:** Align grid tracks along the inline (row) axis.
7. **align-content:** Align grid tracks along the block (column) axis.

### Properties of Grid Items

1. **grid-column-start/grid-column-end/grid-row-start/grid-row-end:** Specify the location of grid items within the grid.
2. **grid-column/grid-row:** Shorthand for grid-column-start and grid-column-end/grid-row-start and grid-row-end.
3. **grid-area:** Assign a name to a grid item for easy placement within the grid.


