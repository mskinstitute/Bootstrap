## How To Create an Offcanvas Sidebar

The following example shows how to create an offcanvas sidebar:
```html
<!-- Offcanvas Sidebar -->
<div class="offcanvas offcanvas-start" id="demo">
  <div class="offcanvas-header">
    <h1 class="offcanvas-title">Heading</h1>
    <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas"></button>
  </div>
  <div class="offcanvas-body">
    <p>Some text lorem ipsum.</p>
    <p>Some text lorem ipsum.</p>
    <button class="btn btn-secondary" type="button">A Button</button>
  </div>
</div>

<!-- Button to open the offcanvas sidebar -->
<button class="btn btn-primary" type="button" data-bs-toggle="offcanvas" data-bs-target="#demo">
  Open Offcanvas Sidebar
</button>
```

### Example Explained

The `.offcanvas` class creates the offcanvas sidebar.

The `.offcanvas-start` class positions the offcanvas, and makes it 400px wide. See examples below for more positioning classes.

The `.offcanvas-title` class ensures proper margins and line-height.

Then, add your content inside the `.offcanvas-body` class.

To open the offcanvas sidebar, you must use a `<button>` or an `<a>` element that points to the id of the `.offcanvas` container (`#demo` in our example).

To open the offcanvas sidebar with an `<a>` element, you can point to `#demo` with the href attribute, instead of `data-bs-target` attribute.

___

## Offcanvas Position

Use the `.offcanvas-start|end|top|bottom` to position the offcanvas to the left, right, top or bottom:

### Right Example
```html
<div class="offcanvas offcanvas-end" id="demo">
```

### Top Example
```html
<div class="offcanvas offcanvas-top" id="demo">
```

### Bottom Example
```html
<div class="offcanvas offcanvas-bottom" id="demo">
```

## Responsive OffCanvas Menu

You can also control when you want to hide or show the offcanvas menu on different screen widths, with the `.offcanvas-sm|md|lg|xl|xxl` classes:

### Example
```html
<div class="offcanvas offcanvas-start offcanvas-lg" id="demo">
```

## Dark OffCanvas Menu

Use the `.text-bg-dark` class to create a dark offcanvas menu.

**Tip:** We have also added the `.btn-close-white` class to `.btn-close`, to create a white close button that looks nice with the dark background:

### Example
```html
<div class="offcanvas offcanvas-end" id="demo">
<button type="button" class="btn-close btn-close-white" data-bs-dismiss="offcanvas"></button>
```