## Utilities / Helper Classes

Bootstrap 5 has a lot of utility/helper classes to quickly style elements without using any CSS code.

## Borders

Use the `border` classes to add or remove borders from an element:

### Example
```html
<span class="border"></span>
<span class="border-top"></span>
<hr>
<span class="border border-0"></span>
<span class="border border-bottom-0"></span>
```
## Border Width

Use `.border-1` to `.border-5` to change the width of the border:

### Example
```html
<span class="border border-1"></span>
<span class="border border-5"></span>
```

___

## Border Color

Add a color to the border with any of the contextual border color classes:

### Example
```html
<span class="border border-primary"></span>
```

## Border Radius

Add rounded corners to an element with the `rounded` classes:

### Example
```html
<span class="rounded"></span>
<span class="rounded-end"></span>
<span class="rounded-circle"></span>
<span class="rounded-pill" style="width:130px"></span>
<span class="rounded-0"></span>
<span class="rounded-5"></span>
```

## Float and Clearfix

Float an element to the right with the `.float-end` class or to the left with `.float-start`, and clear floats with the `.clearfix` class:

### Example

```html
<div class="clearfix">
  <span class="float-start">Float left</span>
  <span class="float-end">Float right</span>
</div>
```

## Responsive Floats

Float an element to the left or to the right depending on screen width, with the responsive float classes (`.float-*-start|end` - where \* is `sm` (>=576px), `md` (>=768px), `lg` (>=992px), `xl` (>=1200px) or `xxl` (>=1400px)):

### Example
```html
<div class="float-sm-end">Float right on small screens or wider</div><br>
<div class="float-md-end">Float right on medium screens or wider</div><br>
<div class="float-lg-end">Float right on large screens or wider</div><br>
<div class="float-xl-end">Float right on extra large screens or wider</div><br>
<div class="float-xxl-end">Float right on XXL screens or wider</div><br>
<div class="float-none">Float none</div>
```

## Center Align

Center an element with the `.mx-auto` class (adds margin-left and margin-right: auto):

### Example
```html
<div class="mx-auto bg-warning" style="width:150px">Centered</div>
```

## Width

Set the width of an element with the w-\* classes (`.w-25`, `.w-50`, `.w-75`, `.w-100`, `.w-auto`, and `.mw-100`):

### Example
```html
<div class="w-25 bg-warning">Width 25%</div>
<div class="w-50 bg-warning">Width 50%</div>
<div class="w-75 bg-warning">Width 75%</div>
<div class="w-100 bg-warning">Width 100%</div>
<div class="w-auto bg-warning">Auto Width</div>
<div class="mw-100 bg-warning">Max Width 100%</div>
```

## Height

Set the height of an element with the h-\* classes (`.h-25`, `.h-50`, `.h-75`, `.h-100`, `.h-auto`, and `.mh-100`):

### Example
```html
<div style="height:200px;background-color:#ddd">
  <div class="h-25 bg-warning">Height 25%</div>
  <div class="h-50 bg-warning">Height 50%</div>
  <div class="h-75 bg-warning">Height 75%</div>
  <div class="h-100 bg-warning">Height 100%</div>
  <div class="h-auto bg-warning">Auto Height</div>
  <div class="mh-100 bg-warning" style="height:500px">Max Height 100%</div>
</div>
```

## Spacing

Bootstrap 5 has a wide range of responsive margin and padding utility classes. They work for all breakpoints: `xs` (<=576px), `sm` (>=576px), `md` (>=768px), `lg` (>=992px), `xl` (>=1200px) or `xxl` (>=1400px)):

The classes are used in the format: `{property}{sides}-{size}` for `xs` and `{property}{sides}-{breakpoint}-{size}` for `sm`, `md`, `lg`, `xl` and `xxl`.

Where _property_ is one of:

-   `m` - sets `margin`
-   `p` - sets `padding`

Where _sides_ is one of:

-   `t` - sets `margin-top` or `padding-top`
-   `b` - sets `margin-bottom` or `padding-bottom`
-   `s` - sets `margin-left` or `padding-left`
-   `e` - sets `margin-right` or `padding-right`
-   `x` - sets both `padding-left` and `padding-right` or `margin-left` and `margin-right`
-   `y` - sets both `padding-top` and `padding-bottom` or `margin-top` and `margin-bottom`
-   blank - sets a `margin` or `padding` on all 4 sides of the element

Where _size_ is one of:

-   `0` - sets `margin` or `padding` to `0`
-   `1` - sets `margin` or `padding` to `.25rem`
-   `2` - sets `margin` or `padding` to `.5rem`
-   `3` - sets `margin` or `padding` to `1rem`
-   `4` - sets `margin` or `padding` to `1.5rem`
-   `5` - sets `margin` or `padding` to `3rem`
-   `auto` - sets `margin` to auto

### Example

```html
<div class="pt-4 bg-warning">I only have a top padding (1.5rem)</div>
<div class="p-5 bg-success">I have a padding on all sides (3rem)</div>
<div class="m-5 pb-5 bg-info">I have a margin on all sides (3rem) and a bottom padding (3rem)</div>
```

### More Spacing Examples
| Class | Objective | Example |
|-------|-----------------------|-----------|
| `.m-*`	| margin on all sides	| Check Now |
| `.mt-*`	| margin top	| Check Now |
| `.mb-*`	| margin bottom	| Check Now |
| `.ms-*`	| margin left	| Check Now |
| `.me-*`	| margin right	| Check Now |
| `.mx-*`	| margin left and right	| Check Now |
| `.my-*`	| margin top and bottom	| Check Now |
| `.p-*`	| padding on all sides	| Check Now |
| `.pt-*`	| padding top	| Check Now |
| `.pb-*`	| padding bottom	| Check Now |
| `.ps-*`	| padding left	| Check Now |
| `.pe-*`	| padding right	| Check Now |
| `.py-*`	| padding top and bottom	| Check Now |
| `.px-*`	| padding left and right	| Check Now |


## Shadows

Use the `shadow-` classes to add shadows to an element:

### Example
```html
<div class="shadow-none p-4 mb-4 bg-light">No shadow</div>
<div class="shadow-sm p-4 mb-4 bg-white">Small shadow</div>
<div class="shadow p-4 mb-4 bg-white">Default shadow</div>
<div class="shadow-lg p-4 mb-4 bg-white">Large shadow</div>
```

## Vertical Align

Use the `align-` classes to change the alignment of elements (only works on inline, inline-block, inline-table and table cell elements):

### Example
```html
<span class="align-baseline">baseline</span>
<span class="align-top">top</span>
<span class="align-middle">middle</span>
<span class="align-bottom">bottom</span>
<span class="align-text-top">text-top</span>
<span class="align-text-bottom">text-bottom</span>
```

## Aspect Ratio

Create responsive video or slideshows based on the width of the parent.

Add the `.ratio` class together with an aspect ratio of your choice `.ratio-*` to a parent element, and add the embed (video or iframe) inside of it:

### Example
```html
<!-- Aspect ratio 1:1 -->
<div class="ratio ratio-1x1">
  <iframe src="https://www.youtube.com/embed/tgbNymZ7vqY"></iframe>
</div>

<!-- Aspect ratio 4:3 -->
<div class="ratio ratio-4x3">
  <iframe src="https://www.youtube.com/embed/tgbNymZ7vqY"></iframe>
</div>

<!-- Aspect ratio 16:9 -->
<div class="ratio ratio-16x9">
  <iframe src="https://www.youtube.com/embed/tgbNymZ7vqY"></iframe>
</div>

<!-- Aspect ratio 21:9 -->
<div class="ratio ratio-21x9">
  <iframe src="https://www.youtube.com/embed/tgbNymZ7vqY"></iframe>
</div>
```

## Visibility

Use the `.visible` or `.invisible` classes to control the visibility of elements. **Note:** These classes do not change the CSS display value. They only add `visibility:visible` or `visibility:hidden`:

### Example
```html
<div class="visible">I am visible</div>
<div class="invisible">I am invisible</div>
```

## Close icon

Use the `.btn-close` class to style a close icon. This is often used for alerts and modals.

### Example
```html
<button type="button" class="btn-close"></button>
```

## Screenreaders

Use the `.visually-hidden` class to hide an element on all devices, except screen readers:

### Example
```html
<span class="visually-hidden">I will be hidden on all screens except for screen readers.</span>
```
## Colors

As described in the [Colors]() chapter, here is a list of all text and background color classes:

The classes for text colors are: `.text-muted`, `.text-primary`, `.text-success`, `.text-info`, `.text-warning`, `.text-danger`, `.text-secondary`, `.text-white`, `.text-dark`, `.text-body` (default body color/often black) and `.text-light`:

### Example
```html
<p class="text-primary">This text is important.</p>
```

Contextual text classes can also be used on links:

### Example
```html
<a href="#" class="text-warning">Warning link.</a>
```

You can also add 50% opacity for black or white text with the `.text-black-50` or `.text-white-50` classes:

### Example
```html
<p class="text-black-50">Black text with 50% opacity on white background</p>
<p class="text-white-50 bg-dark">White text with 50% opacity on black background</p>
```

## Background Colors

The classes for background colors are: `.bg-primary`, `.bg-success`, `.bg-info`, `.bg-warning`, `.bg-danger`, `.bg-secondary`, `.bg-dark` and `.bg-light`.

### Example
```html
<div class="bg-warning p-3"></div>
```

The `.bg-_color_` classes above does not work well with text, or atleast then you have to specify a proper `.text-_color_` class to get the right text color for each background.

However, you can use the `.text-bg-_color_` classes and Bootstrap will automatically handle the appropriate text color for each background color:

### Example
```html
<p class="text-bg-warning">This text represents a warning.</p>
```
