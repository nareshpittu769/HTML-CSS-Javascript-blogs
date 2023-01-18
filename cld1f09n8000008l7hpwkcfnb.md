# Learn: Box-Model

Every HTML element is treated as a box, the box model is nothing but the element has the `margin` , `border` , `padding` , `content` . It mainly talks about the layout of the element.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674028426162/3be99217-5781-45d5-b74a-f1893f20f0c5.png align="center")

### Margin

The margin is nothing but we are giving the space outside the border. Here we can give space to all four sides or `top`, `left-right`, `bottom` or `top-bottom`, `left-right`.

```xml
div {
    margin: 10px; /* for all sides */
    margin: 10px 25px; /* for top-bottom and left-right */
    margin: 10px 25px 10px; /* Top, left-right, bottom */
    margin: 10px 10px 10px 10px; /* top , right, bottom , left */
}
```

The values are taken in order as TOP-&gt;RIGHT-&gt;BOTTOM-&gt;LEFT.

We can also specify individual margin like; `margin-top` , `margin-right` , `margin-bottom` , `margin-left` . Here we can specify the margin as `auto`.

### Padding

The padding is nothing but space inside the border. we can give space to all four sides *or* `top`, `left-right`, `bottom` *or* `top-bottom`, `left-right`. It is the same as the margin.

```xml
div {
    padding: 10px; /* for all sides */
    padding: 10px 25px; /* for top-bottom and left-right */
    padding: 10px 25px 10px; /* Top, left-right, bottom */
    padding: 10px 10px 10px 10px; /* top , right, bottom , left */
/* "%" - Specifies the padding in percent of the width of the containing element  */
}
```

The values are taken in order as TOP-&gt;RIGHT-&gt;BOTTOM-&gt;LEFT.

We can also specify individual padding like; `padding-top` , `padding-right` , `padding-bottom` , `padding-left` .

### Border

The border came in between the padding and margin.

Syntax: `border: 1px solid black;`

The `border-style` property specifies what kind of border to display.

The following values are allowed:

* `dotted` - Defines a dotted border
    
* `dashed` - Defines a dashed border
    
* `solid` - Defines a solid border
    
* `double` - Defines a double border
    
* `groove` - Defines a 3D grooved border. The effect depends on the border-color value
    
* `ridge` - Defines a 3D ridged border. The effect depends on the border-color value
    
* `inset` - Defines a 3D inset border. The effect depends on the border-color value
    
* `outset` - Defines a 3D outset border. The effect depends on the border-color value
    
* `none` - Defines no border
    
* `hidden` - Defines a hidden border
    

```xml
<!DOCTYPE html>
<html>
<head>
<style>
p.dotted {
    border-style: dotted;
}
p.dashed {
    border-style: dashed;
}
p.solid {
    border-style: solid;
}
p.double {
    border-style: double;
}
p.groove {
    border-style: groove;
}
p.ridge {
    border-style: ridge;
}
p.inset {
    border-style: inset;
}
p.outset {
    border-style: outset;
}
p.none {
    border-style: none;
}
p.hidden {
    border-style: hidden;
}
p.mix {
    border-style: dotted dashed solid double;
}
</style>
</head>
<body>

<h2>The border-style Property</h2>
<p>This property specifies what kind of border to display:</p>

<p class="dotted">A dotted border.</p>
<p class="dashed">A dashed border.</p>
<p class="solid">A solid border.</p>
<p class="double">A double border.</p>
<p class="groove">A groove border.</p>
<p class="ridge">A ridge border.</p>
<p class="inset">An inset border.</p>
<p class="outset">An outset border.</p>
<p class="none">No border.</p>
<p class="hidden">A hidden border.</p>
<p class="mix">A mixed border.</p>

</body>
</html>
```

> **Note**: When you set the width and height properties of an element with CSS, you just set the width and height of the **content area**. To calculate the full size of an element, you must also add padding, borders and margins.

### Content

The content is nothing but **data** like text, images, videos etc.