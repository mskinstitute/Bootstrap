# Stacked Form

All textual `<input>` and  `<textarea>` elements with class .form-control get proper form styling:
```html
<form>
    <div class="mb-3 mt-3">
        <label for="email" class="form-label">Email:</label>
        <input type="email" class="form-control" id="email" placeholder="Enter email" name="email">
    </div>

    <button type="submit" class="btn btn-primary">Create Account</button>
</form>
```
> Also note that we add a `.form-label` class to each label element to ensure correct padding.

Checkboxes have different markup. They are wrapped around a container element with `.form-check`, and labels have a class of `.form-check-label`, while checkboxes and radio buttons use `.form-check-input`.

## Textarea
```html
<label for="comment">Comments:</label>
<textarea class="form-control" rows="5" id="comment" name="text"></textarea>
```

## Form Row/Grid (Inline Forms)

If you want your form elements to appear side by side, use `.row` and `.col`:
```html
<form>
  <div class="row">
    <div class="col">
      <input type="text" class="form-control" placeholder="Enter email" name="email">
    </div>
    <div class="col">
      <input type="password" class="form-control" placeholder="Enter password" name="pswd">
    </div>
  </div>
</form>
```
## Form Control Size

You can change the size of `.form-control` inputs with `.form-control-lg` or `.form-control-sm`:
```html
<input type="text" class="form-control form-control-lg" placeholder="Large input">
<input type="text" class="form-control" placeholder="Normal input">
<input type="text" class="form-control form-control-sm" placeholder="Small input">
```

## Disabled and Readonly

Use the `disabled` and/or `readonly` attributes to disable the input field:
```html
<input type="text" class="form-control" placeholder="Normal input">
<input type="text" class="form-control" placeholder="Disabled input" disabled>
<input type="text" class="form-control" placeholder="Readonly input" readonly>
```

## Plain text Inputs

Use the `.form-control-plaintext` class to style an input field without borders, but keep proper marigins and padding:
```html
<input type="text" class="form-control-plaintext" placeholder="Plaintext input">
<input type="text" class="form-control" placeholder="Normal input">
```

## Color Picker

To style an input with type="color" properly, use the `.form-control-color` class:
```html
<input type="color" class="form-control form-control-color" value="#CCCCCC">
```


# Select

Select menus are used if you want to allow the user to pick from multiple options.

To style a select menu in Bootstrap 5, add the `.form-select` class to the `<select>` element:
```html
<select class="form-select">
  <option>Home</option>
  <option>About</option>
  <option>Contact</option>
</select>
```

## Select Menu Size

Use the `.form-select-lg` or `.form-select-sm` class to change the size of the select menu:
```html
<select class="form-select form-select-lg">
<select class="form-select">
<select class="form-select form-select-sm">
```

## Disabled Select Menu
```html
<select class="form-select" disabled>
  <option>Home</option>
  <option>About</option>
  <option>Contact</option>
</select>
```

## Data Lists

Bootstrap will also style data lists, which is a list of pre-defined options for an `<input>` element:
```html
<label for="browser" class="form-label">Your favorite Programming:</label>
<input class="form-control" list="browsers" name="browser" id="browser">
<datalist id="browsers">
  <option value="HTML">
  <option value="CSS">
  <option value="JavaScript">
  <option value="Bootstrap">
</datalist>
```

# Checkboxes and Radio buttons

## Checkboxes

Checkboxes are used if you want the user to select any number of options from a list of preset options.
```html
<div class="form-check">
  <input class="form-check-input" type="checkbox" id="check1" name="html" value="html" checked>
  <label class="form-check-label" for="check1">HTML</label>
</div>
```

#### Example Explained

To style checkboxes, use a wrapper element with `class="form-check"` to ensure proper margins for labels and checkboxes.

Then, add the `.form-check-label` class to label elements, and `.form-check-input` to style checkboxes properly inside the `.form-check` container.

Use the `checked` attribute if you want the checkbox to be checked by default.

___

## Radio buttons

Radio buttons are used if you want to limit the user to just one selection from a list of preset options.
```html
<div class="form-check">
  <input type="radio" class="form-check-input" id="radio1" name="optradio" value="html" checked>html
  <label class="form-check-label" for="radio1"></label>
</div>
<div class="form-check">
  <input type="radio" class="form-check-input" id="radio2" name="optradio" value="CSS">CSS
  <label class="form-check-label" for="radio2"></label>
</div>
<div class="form-check">
  <input type="radio" class="form-check-input" disabled>JavaScript
  <label class="form-check-label"></label>
</div>
```

## Toggle Switches

If you want your checkbox to be styled as a toggle switch, use the `.form-switch` class together with the `.form-check` container:
```html
<div class="form-check form-switch">
  <input class="form-check-input" type="checkbox" id="mySwitch" name="darkmode" value="yes" checked>
  <label class="form-check-label" for="mySwitch">Dark Mode</label>
</div>
```

# Range

## Custom Range

To style a range menu, add the `.form-range` class to the input element with type="range":
```html
<label for="customRange" class="form-label">Custom range</label>
<input type="range" class="form-range" id="customRange">
```

## Steps

By default, the interval between the range numbers is 1. You can change it by using the `step` attribute:

### Example
```html
<input type="range" class="form-range" step="10">
```

## Min and Max

By default, the minimum value is 0 and maximum value is 100. You can use the `min` and/or `max` attribute change it:
```html
<input type="range" class="form-range" min="0" max="4">
```

# Input Groups

The `.input-group` class is a container to enhance an input by adding an icon, text or a button in front or behind the input field as a "help text".

To style the specified help text, use the `.input-group-text` class:
```html
<form>
  <div class="input-group">
    <span class="input-group-text">@</span>
    <input type="text" class="form-control" placeholder="Username">
  </div>

  <div class="input-group">
    <input type="text" class="form-control" placeholder="Your Email">
    <span class="input-group-text">@example.com</span>
  </div>
</form>
```

## Input Group Size

Use the `.input-group-sm` class for small input groups and `.input-group-lg` for large inputs groups:
```html
<div class="input-group mb-3 input-group-sm">
   <span class="input-group-text">Small</span>
  <input type="text" class="form-control">
</div>

<div class="input-group mb-3">
  <span class="input-group-text">Default</span>
  <input type="text" class="form-control">
</div>

<div class="input-group mb-3 input-group-lg">
  <span class="input-group-text">Large</span>
  <input type="text" class="form-control">
</div>
```

## Multiple Inputs and Helpers

Add multiple inputs or addons:
```html
<!-- Multiple inputs -->
<div class="input-group mb-3">
  <span class="input-group-text">Person</span>
  <input type="text" class="form-control" placeholder="First Name">
  <input type="text" class="form-control" placeholder="Last Name">
</div>

<!-- Multiple addons / help text -->
<div class="input-group mb-3">
  <span class="input-group-text">One</span>
  <span class="input-group-text">Two</span>
  <span class="input-group-text">Three</span>
  <input type="text" class="form-control">
</div>
```

## Input Group with Checkboxes and Radios

You can also use checkboxes or radio buttons instead of text:
```html
<div class="input-group mb-3">
  <div class="input-group-text">
    <input type="checkbox">
  </div>
  <input type="text" class="form-control" placeholder="Some text">
</div>

<div class="input-group mb-3">
  <div class="input-group-text">
    <input type="radio">
  </div>
  <input type="text" class="form-control" placeholder="Some text">
</div>
```

## Input Group Buttons
```html
<div class="input-group mb-3">
  <button class="btn btn-outline-primary" type="button">Basic Button</button>
  <input type="text" class="form-control" placeholder="Some text">
</div>

<div class="input-group mb-3">
  <input type="text" class="form-control" placeholder="Search">
  <button class="btn btn-success" type="submit">Go</button>
</div>

<div class="input-group mb-3">
  <input type="text" class="form-control" placeholder="Something clever..">
  <button class="btn btn-primary" type="button">OK</button>
  <button class="btn btn-danger" type="button">Cancel</button>
</div>
```

## Input Group with Dropdown Button

Add a dropdown button in the input group. Note that you don't need the .dropdown wrapper, as you normally would.
```html
<div class="input-group mt-3 mb-3">
  <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown">
    Dropdown button
  </button>
  <ul class="dropdown-menu">
    <li><a class="dropdown-item" href="#">Link 1</a></li>
    <li><a class="dropdown-item" href="#">Link 2</a></li>
    <li><a class="dropdown-item" href="#">Link 3</a></li>
  </ul>
  <input type="text" class="form-control" placeholder="Username">
</div>
```

# Floating Labels / Animated Labels

By default, when using labels, they normally appear on top of the input field:

With floating labels, you can insert the label inside the input field, and make them float/animate when you click on the input field:

### Example
```html
<div class="form-floating mb-3 mt-3">
  <input type="text" class="form-control" id="email" placeholder="Enter email" name="email">
  <label for="email">Email</label>
</div>

<div class="form-floating mt-3 mb-3">
  <input type="text" class="form-control" id="pwd" placeholder="Enter password" name="pswd">
  <label for="pwd">Password</label>
</div>
```

**Notes on floating labels:** The `<label>` elements must come after the `<input>` element, and the `placeholder` attribute is required for each `<input>` element (even though it is not shown).

## Textarea

It also works for textareas:

Comments

### Example
```html
<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Comments</label>
</div>
```

## Select Menus

You can also use "floating-labels" on select menus. However, they will not float/get animated. The label will always appear in the top left corner, inside the select menu:

1 2 3 4 Select list (select one):

### Example
```html
<div class="form-floating">
  <select class="form-select" id="sel1" name="sellist">
    <option>HTMl</option>
    <option>CSS</option>
    <option>JavaScript</option>
  </select>
  <label for="sel1" class="form-label">Select list (select one):</label>
</div>
```

# Form Validation

You can use different validation classes to provide valuable feedback to users. Add either `.was-validated` or `.needs-validation` to the `<form>` element, depending on whether you want to provide validation feedback before or after submitting the form. The input fields will have a green (valid) or red (invalid) border to indicate what's missing in the form. You can also add a `.valid-feedback` or `.invalid-feedback` message to tell the user explicitly what's missing, or needs to be done before submitting the form.

### Example

In this example, we use `.was-validated` to indicate what's missing before submitting the form:
```html
<form action="/action_page.php" class="was-validated">
  <div class="mb-3 mt-3">
    <label for="uname" class="form-label">Username:</label>
    <input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname" required>
    <div class="valid-feedback">Valid.</div>
    <div class="invalid-feedback">Please fill out this field.</div>
  </div>
  <div class="mb-3">
    <label for="pwd" class="form-label">Password:</label>
    <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd" required>
    <div class="valid-feedback">Valid.</div>
    <div class="invalid-feedback">Please fill out this field.</div>
  </div>
  <div class="form-check mb-3">
    <input class="form-check-input" type="checkbox" id="myCheck" name="remember" required>
    <label class="form-check-label" for="myCheck">I agree on blabla.</label>
    <div class="valid-feedback">Valid.</div>
    <div class="invalid-feedback">Check this checkbox to continue.</div>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```