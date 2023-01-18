# Learn: Flexbox And It's Properties

## What is flex?

> The flex allows aligning and distribution of the items in a row and a column direction. Here we can resize, stretch, and shrink the items in the container.

## Properties of flex

* Parent properties (container)
    
* children properties(items)
    

## **Parent Properties(container)**

### Display

Default the items are in block-wise when we apply the property the direction will change to inline. It applies to all children elements.

```xml
.container {
  display: flex; /* inline-flex */
}
```

### Flex-direction

Here we can set the direction of flex as vertical or horizontal. The flex-direction are four types.

* `row` - The default flex is row, the items are arranged horizontally(L to R).
    
* `row-reverse` - The items are arranged in row reverse(R to L).
    
* `column` - The items are arranged vertically from top to bottom.
    
* `column-reverse` - The items are arranged in the reverse of column from bottom to top.
    

```xml
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

### Flex-wrap

If we decrease the screen size the items by default fit into one line(the size of items will decrease). So with the help of this property, we can wrap into multiple lines without decreasing the original size of the items.

```xml
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

> Note: The wrap-reverse is the reverse of the wrap.

### Flex-Flow

This is the shorthand for `Flex-direction` and `flex-wrap` properties. Here we can declare both values in a single property. The default is "row nowrap".

```xml
.container {
  flex-flow: column wrap;
}
```

### Justify-content

This defines the alignment along the row. It helps distribute extra **free space** **left over** when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. There are different types of values they are,

* `flex-start` (default): items are packed toward the start of the flex direction.
    
* `flex-end`: items are packed toward the end of the flex direction.
    
* `start`: items are packed toward the start of the `writing-mode` direction.
    
* `end`: items are packed toward the end of the `writing-mode` direction.
    
* `left`: items are packed toward the left edge of the container unless that doesn’t make sense with the `flex-direction`, then it behaves like `start`.
    
* `right`: items are packed toward the right edge of the container unless that doesn’t make sense with the `flex-direction`, then it behaves like `end`.
    
* `center`: items are centered along the line
    
* `space-between`: items are evenly distributed in the line; the first item is on the start line, the last item is on the end line
    
* `space-around`: items are evenly distributed in the line with equal space around them. Note that visually the spaces aren’t equal, since all the items have equal space on both sides. The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.
    
* `space-evenly`: items are distributed so that the spacing between any two items is equal.
    

```xml
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}
```

### align-items

This works towards the column all items are distributed vertically.

* `flex-start`: The items are placed at the start of the flex axis.
    
* `flex-end`: The items are placed at the end of the flex axis.
    
* `stretch`: This fills the container max width and height of the container.
    
* `center`: The items are placed at the center of the container.
    
* `baseline`: The items are aligned based on the baseline.
    

```xml
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}
```

### align-content

If there is free space in the cross-axis (column-wise) the content is distributed across the container. It is the same as justify-content but it applies when the container has multiple lines.

> Note: If a container has a single line it will not apply.

* `normal` (default): items are packed in their default position as if no value was set.
    
* `flex-start` / `start`: items packed to the start of the container. The (more supported) `flex-start` honors the `flex-direction` while `start` honors the `writing-mode` direction.
    
* `flex-end` / `end`: items packed to the end of the container. The `flex-end` honors the `flex-direction` while the end honors the `writing-mode` direction.
    
* `center`: items centered in the container.
    
* `space-between`: items evenly distributed; the first line is at the start of the container while the last one is at the end.
    
* `space-around`: items evenly distributed with equal space around each line.
    
* `space-evenly`: items are evenly distributed with equal space around them.
    
* `stretch`: lines stretch to take up the remaining space.
    

### gap

The gap property applies between the items based on the gap direction.

`row-gap` : The gap will apply to the row-wise.

`column-gap` : The column gap applies to the all columns.

`gap` : Applies to the row and column.

```xml
.container {
  display: flex;
  ...
  gap: 10px;
  gap: 10px 20px; /* row-gap column gap */
  row-gap: 10px;
  column-gap: 20px;
}
```

## **Child Properties(items)**

### order

The order works by default in the source order. All items have zero order by default it works on flex-direction.

```xml
/* the order ex: 0 1 2 3 4 5...so on */
.item {
  order: 5; /* default is 0 , item goes and settle at 5th position.*/
}
```

### flex-grow

The ability to grow the item across the free space of the container. The by default flex-grow is 0. If we give the `flex-grow:1;` it will take double the item's size. If one of the children has a value of `2`, that child would take up twice as much of the space as either one of the others (or it will try, at least).

> Note: Negative numbers are invalid.

```xml
.item {
  flex-grow: 2; /* default 0 */
}
```

### flex-**shrink**

The ability of an item to shrink. Here we are telling the particular item to shrink first after it shrink all other items will get shrink.

> Note: Negative numbers are invalid.

```xml
.item {
  flex-shrink: 3; /* default 1 */
}
```

### flex-basis

This defines the default size of an element before the remaining space is distributed. The auto keyword distribute the space according to the size and hight remaining after flex-grow.

```xml
.item {
  flex-basis:  | auto; /* default auto or if we set 0 the space is not distributed*/
}
```

### flex

The flex property is shorthand for the `flex-grow`, `flex-shrink`, `flex-basis` . The default values is the `flex-grow:0;`, `flex-shrink:1;`, `flex-basis:auto;` .

```xml
.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
```

### **align-self**

This allows the default alignment to be overridden for individual flex items.

```xml
.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```