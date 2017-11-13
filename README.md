# CSS Notes

Notes on CSS

## Flexbox

### Using Flexbox

Flexbox is great at aligning the content inside elements. It is used to position the smaller details of page. Flexbox works better in one direction only.
Flexbox can be applied to elements using `display: flex;`

### Justify Content

`justify-content` aligns items horizontally, and accepts the following values:

1. `flex-start`: Items align to the left side of the container.
1. `flex-end`: Items align to the right side of the container.
1. `center`: Items align at the center of the container.
1. `space-between`: Items display with equal spacing between them (Space is ***not*** added to the left of the first element, and right side of last element)
1. `space-around`: Items display with equal spacing around them (Space ***is*** added to the left of the first element, and right side of last element)

### Align Items

`align-items` aligns items vertically, and accepts the following values:

1. `flex-start`: Items align to the top of the container.
1. `flex-end`: Items align to the bottom of the container.
1. `center`: Items align at the vertical center of the container.
1. `baseline`: Items display at the baseline of the container.
1. `stretch`: Items are stretched to fit the container.

### Flex Direction

`flex-direction` defines the direction items are placed in the contained, and accepts the following values:

1. `row`: Items are placed the same as text direction.
1. `row-reverse`: Items are placed opposite to the text direction.
1. `column`: Items are placed top to bottom.
1. `column-reverse`: Items are placed from bottom to top.

### Order (Flex)

`order` is applied to individual items inside a container. By default, items have a value of 0, but the property can be set to a positive of negative integer value. Setting the value to 1 means moving forward the order of items inside the container by 1. For the element 1, before, (1,2,3,4,5) After, (5,1,2,3,4)

### Align Self

`align-self` does the exact same thing as `align-items`, but it is applied to individual items inside a container instead.

### Flex Wrap

`flex-wrap` changes the wrap of items inside it, and accepts the following values:

1. `nowrap`: Everything is fit to a single line.
1. `wrap`: Items wrap around to additional lines.
1. `wrap-reverse`: Items wrap around to additional lines in reverse.

### Flex Flow

`flex-flow` is a combination of `flex-direction` and `flex-wrap`. This property accepts one of the two properties separated by a space.

### Align Content

`align-content` is used to set how multiple lines are spaced apart from each other. This property takes the following values:

1. `flex-start`: Line are packed at the top of the container.
1. `flex-end`: Lines are packed at the bottom of the container.
1. `center`: Line are packed at the vertical center of the container.
1. `space-between`: Lines display with equal spacing between them.
1. `space-around`: Lines display with equal spacing around them.
1. `stretch`: Lines are stretch to fit the container.

`align-content` determines the spacing between lines, whereas `align-items` determine how items as a whole are aligned within the container.

## Grid

CSS grids are used to build the bigger picture. They make it easier to manage the layout of the page, and can even handle more unorthodox and asymmetrical designs. CSS grids are used for 2D layouts.

### Grid Column Start

`grid-column-start` is used to specify a grid item's start position within the grid column, by contributing a line, span, or nothing (automatic) to its grid placement. This start position defines the block-start edge of the grid area. `grid-column-start` also accepts negative values.

### Grid Column End

`grid-column-end` is used to specify a grid item's end position within the grid column. This end position defines the block-end edge of the grid area. `grid-column-end` also accepts negative values.

### Span

Instead of defining a grid item based on the start and end positions of the grid lines, you can define it based on your desired column using the `span` keyword. ***span*** only works with positive values.

### Grid Column

`grid-column` is a shorthand property that can accept values for both `grid-column-start` and `grid-column-end` at once, separated by a slash.

### Grid Row

`grid-row-start` works much like `grid-column-start`, except along the vertical axis. The same applies for other properties, such as `grid-row-end`

### Grid Area

`grid-area` is a shorthand for `grid-row-start`, `grid-column-start`, `grid-row-end`, followed by `grid-column-end`.

### Order (Grid)

By default, all grid items have an `order` of 0, but this can be set to any positive or negative integer, similar to `z-index`.

### Grid Template Columns, Rows

`grid-template-columns` and `grid-template-rows` define the line names and track sizing functions of the grid columns and rows. They accept values of percentages, pixels, and em.

### Repeat

`repeat` can be used inside `grid-template-columns` and `grid-template-rows` to eliminate the need to type out the repeated values. e.g. `grid-template-columns: repeat(8, 12.5%);`

### FR Unit

The unit `fr` is a fractional unit that allocates one share of the available space. For example, if two elements are set to `1fr` and `3fr` respectively, the space is divided into 4 equal shares; the first element occupies 1/4 and the second element occupies 3/4 of any leftover space.

### Grid Template

`grid-template` is a shorthand property that combines `grid-template-rows` and `grid-template-columns`. e.g. `grid-template: 50% 50% / 200px;` will create a grid with two rows that are 50% each, and each one column that is 200 pixels wide.
