# Flexbox Notes

Notes on how Flexbox works

## Using Flexbox

Flexbox can be applied to elements using `display: flex;`

## Justify Content

`justify-content` aligns items horizontally, and accepts the following values:

1. `flex-start`: Items align to the left side of the container.
1. `flex-end`: Items align to the right side of the container.
1. `center`: Items align at the center of the container.
1. `space-between`: Items display with equal spacing between them (Space is ***not*** added to the left of the first element, and right side of last element)
1. `space-around`: Items display with equal spacing around them (Space ***is*** added to the left of the first element, and right side of last element)

## Align Items

`align-items` aligns items vertically, and accepts the following values:

1. `flex-start`: Items align to the top of the container.
1. `flex-end`: Items align to the bottom of the container.
1. `center`: Items align at the vertical center of the container.
1. `baseline`: Items display at the baseline of the container.
1. `stretch`: Items are stretched to fit the container.

## Flex Direction

`flex-direction` defines the direction items are placed in the contained, and accepts the following values:

1. `row`: Items are placed the same as text direction.
1. `row-reverse`: Items are placed opposite to the text direction.
1. `column`: Items are placed top to bottom.
1. `column-reverse`: Items are placed from bottom to top.

## Order

`order` is applied to individual items inside a container. By default, items have a value of 0, but the property can be set to a positive of negative integer value. Setting the value to 1 means moving forward the order of items inside the container by 1. For the element 1, before, (1,2,3,4,5) After, (5,1,2,3,4)

## Align Self

`align-self` does the exact same thing as `align-items`, but it is applied to individual items inside a container instead.

## Flex Wrap

`flex-wrap` changes the wrap of items inside it, and accepts the following values:

1. `nowrap`: Everything is fit to a single line.
1. `wrap`: Items wrap around to additional lines.
1. `wrap-reverse`: Items wrap around to additional lines in reverse.

## Flex Flow

`flex-flow` is a combination of `flex-direction` and `flex-wrap`. This property accepts one of the two properties separated by a space.

## Align Content

`align-content` is used to set how multiple lines are spaced apart from each other. This property takes the following values:

1. `flex-start`: Line are packed at the top of the container.
1. `flex-end`: Lines are packed at the bottom of the container.
1. `center`: Line are packed at the vertical center of the container.
1. `space-between`: Lines display with equal spacing between them.
1. `space-around`: Lines display with equal spacing around them.
1. `stretch`: Lines are stretch to fit the container.

`align-content` determines the spacing between lines, whereas `align-items` determine how items as a whole are aligned within the container.
