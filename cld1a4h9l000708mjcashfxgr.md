# Learn: Position and its value's

## position

The position is used for changing the element position based on values. And the position will work only if we give properties like `top`, `bottom`, `left`, `right` .

```xml
.element {
  position: value;
}
```

## values

### Static

The static position is not affected by the `top` `bottom` `left` `right` properties. It will remain sick to the document.

```xml
div {
  position: static;
  border: 3px solid #73AD21;
}
```

### Relative

It is relative to its normal position if we apply any `top` `bottom` `left` `right` it will change position based on the relative to its original position.

```xml
div {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
```

### Absolute

If a child element has an `absolute` value then the parent has the `position: relative;` .

An element with `position: absolute;` is positioned relative to the nearest positioned ancestor. If an absolute positioned element has no positioned ancestors(parent), it uses the document body and moves along with page scrolling.

```xml
.element {
  position: absolute;
}
```

If the parent does not have a relative position the child will change the position according to the document, not the parent. So we have to set the position of the parent element as relative.

```xml
.parent {
  position: relative;
}
```

Now properties such as `left`, `right`, `bottom` and `top` will refer to the parent element.

### Fixed

The element `position: fixed;` will not effect by the `top`, `bottom` , `left` , `right` it is fixed in one position even if the page is scrolled. It is relative to the `viewport`.

```xml
div {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
```

### Sticky

An element with `position: sticky;` is positioned based on the user's scroll position.

A sticky element toggles between `relative` and `fixed`, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like position: fixed).

You have to must give properties like `top`, `bottom` , `left` , `right` otherwise, it will not work.

```xml
div {
  position: sticky;
  top: 0;
  background-color: green;
  border: 2px solid #4CAF50;
}
```