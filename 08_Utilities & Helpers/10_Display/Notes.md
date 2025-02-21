## **Lecture Notes: Bootstrap Display Classes**

### **Introduction**
Bootstrap is a powerful front-end framework that simplifies responsive web design. It includes a series of utility classes that help you quickly control the layout of elements, including how and when elements are displayed on the page. One of these utilities is the **display classes**.

**Display Classes** are used to control the visibility and layout of elements in different screen sizes. Bootstrap provides a set of predefined classes to manage how elements are shown or hidden based on breakpoints, making your website responsive and adaptable to various devices.

---

### **1. Basics of Display Classes in Bootstrap**

In Bootstrap, display classes are used to change the CSS `display` property of an element. This property dictates how an element behaves in the layout (inline, block, grid, flex, etc.).

Bootstrap provides several utility classes for this purpose, ranging from displaying elements as block, inline-block, inline, flex, grid, or none.

Here’s a breakdown of the primary **display classes**:

#### **Class Structure:**
```html
.d-{value}
```

Where `value` can be one of the following options:

- `none`: Hide the element
- `inline`: Display the element as an inline element
- `inline-block`: Display the element as an inline-block element
- `block`: Display the element as a block element
- `flex`: Display the element as a flex container
- `grid`: Display the element as a grid container
- `table`: Display the element as a table element

---

### **2. Display Classes for Different Breakpoints**

Bootstrap allows you to modify the display property at different breakpoints (screen widths) using the **responsive display classes**. This is especially useful when you need elements to behave differently based on the size of the screen.

Here’s how you can use display classes with breakpoints:

```html
.d-{value}           /* Applies to all screen sizes */
.d-{value}-sm        /* Applies from small screens (≥576px) and up */
.d-{value}-md        /* Applies from medium screens (≥768px) and up */
.d-{value}-lg        /* Applies from large screens (≥992px) and up */
.d-{value}-xl        /* Applies from extra-large screens (≥1200px) and up */
.d-{value}-xxl       /* Applies from extra-extra-large screens (≥1400px) and up */
```

### **3. Example: Display Classes in Action**

#### **Example 1: Hiding Elements on Small Screens**

Let’s say we want to hide a navigation element on smaller screens but show it on larger screens:

```html
<!-- This navigation bar will be hidden on small screens and displayed on larger screens -->
<nav class="d-none d-md-block">
  <ul>
    <li>Home</li>
    <li>About</li>
    <li>Contact</li>
  </ul>
</nav>
```

In this example:
- `.d-none`: Hides the navigation on all screen sizes.
- `.d-md-block`: Displays it as a block on medium (`md`) screens and above (≥768px).

#### **Example 2: Showing an Element Only on Small Screens**

If you want an element to appear only on small screens and be hidden on larger ones, you can use this:

```html
<div class="d-block d-md-none">
  <p>This content is only visible on small screens.</p>
</div>
```

Here:
- `.d-block`: Makes the element a block on all screen sizes.
- `.d-md-none`: Hides the element on medium and larger screens.

#### **Example 3: Display Flex at Different Screen Sizes**

You can use the `flex` display class to create flexible layouts that change based on screen size. This is particularly useful for building responsive grid systems.

```html
<div class="d-flex d-sm-block">
  <div class="flex-fill">Item 1</div>
  <div class="flex-fill">Item 2</div>
  <div class="flex-fill">Item 3</div>
</div>
```

In this example:
- `.d-flex`: Displays the container as a flex container on all screen sizes.
- `.d-sm-block`: Changes the display to block (stack items) on small screens and larger.

---

### **4. Combining Display Classes with Other Bootstrap Utilities**

Bootstrap display classes can be combined with other utility classes for more complex layouts.

#### **Example 1: Combining with `align-items` and `justify-content`**

```html
<div class="d-flex justify-content-between align-items-center">
  <div>Left</div>
  <div>Center</div>
  <div>Right</div>
</div>
```

In this example:
- `.d-flex`: Defines the container as a flex container.
- `.justify-content-between`: Distributes items with space between them.
- `.align-items-center`: Vertically centers the items inside the flex container.

#### **Example 2: Using Display Classes in Grids**

You can also use display classes in combination with Bootstrap’s grid system to create responsive layouts.

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 d-none d-md-block">Left Column</div>
    <div class="col-12 col-md-6 d-block d-md-none">Right Column</div>
  </div>
</div>
```

In this example:
- The first column (`col-12 col-md-6`) is displayed on all screen sizes but is hidden on small screens (`d-none d-md-block`).
- The second column is shown only on small screens (`d-block d-md-none`).

---

### **5. Practical Examples**

#### **Example 1: Toggle Content Visibility**

A common use case is showing and hiding content based on user interactions. You can use display classes to hide or show elements dynamically.

```html
<button class="btn btn-primary" onclick="toggleVisibility()">Toggle Content</button>

<div id="content" class="d-none">
  <p>This content can be toggled.</p>
</div>

<script>
  function toggleVisibility() {
    const content = document.getElementById('content');
    content.classList.toggle('d-none');
  }
</script>
```

#### **Example 2: Grid Layout Example**

You can create a responsive grid layout using Bootstrap’s display classes.

```html
<div class="d-grid gap-3 grid-template-columns">
  <div>1st Item</div>
  <div>2nd Item</div>
  <div>3rd Item</div>
</div>
```

This layout will display a responsive grid, changing the number of columns depending on the screen size.

---

### **6. Notes:**

**Bootstrap's display classes** are an essential tool for building responsive layouts and controlling the visibility of elements across different screen sizes. With the combination of `d-{value}` classes and breakpoints, you can easily show or hide content based on the user's device or window size.

#### Key Takeaways:
- **`d-none`**: Hide an element.
- **`d-block`**: Display an element as a block.
- **`d-inline`**: Display an element as inline.
- **`d-flex`**: Display an element as a flex container.
- **Responsive variants** (`d-sm-none`, `d-md-block`, etc.) allow you to control display properties based on screen size.

These classes offer a fast way to manage layout and visibility for building mobile-first, responsive websites.

---

### **Questions**

1. What class would you use to hide an element on medium screens and larger?
2. How can you make a layout element visible only on extra-small screens?
3. What is the difference between `d-flex` and `d-grid` in Bootstrap?
4. How do you make a flex container and center its items vertically and horizontally?

---
