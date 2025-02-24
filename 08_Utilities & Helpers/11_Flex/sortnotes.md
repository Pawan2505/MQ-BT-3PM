## **Lecture Notes: Flex in Bootstrap**

### **Introduction to Flexbox in Bootstrap**

Flexbox is a layout model that makes it easier to design flexible and responsive web pages. Bootstrap 5 provides utilities to quickly create flexible layouts using Flexbox.

### **1. Enable Flex Behaviors**

To start using Flexbox, apply the `.d-flex` class to the container. You can also use `.d-inline-flex` to create inline flex containers.

```html
<div class="d-flex">
  I'm a flexbox container!
</div>

<div class="d-inline-flex">
  I'm an inline flexbox container!
</div>
```

### **2. Flex Direction**

Control the direction of flex items using `.flex-row` (default), `.flex-row-reverse`, `.flex-column`, or `.flex-column-reverse`.

```html
<div class="d-flex flex-row">
  <div>Item 1</div>
  <div>Item 2</div>
</div>

<div class="d-flex flex-column">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

Responsive variations:
- `.flex-sm-row`, `.flex-md-column`, etc.

### **3. Justify Content**

Align items along the main axis (x-axis by default) using:
- `.justify-content-start`
- `.justify-content-end`
- `.justify-content-center`
- `.justify-content-between`
- `.justify-content-around`
- `.justify-content-evenly`

```html
<div class="d-flex justify-content-center">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### **4. Align Items**

Align items along the cross axis (y-axis by default) using:
- `.align-items-start`
- `.align-items-center`
- `.align-items-end`
- `.align-items-baseline`
- `.align-items-stretch`

```html
<div class="d-flex align-items-center">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### **5. Align Self**

Use `.align-self-*` to align individual flex items differently on the cross axis.

```html
<div class="d-flex">
  <div class="align-self-start">Item 1</div>
  <div class="align-self-center">Item 2</div>
</div>
```

### **6. Flex Grow and Shrink**

- **Flex Grow:** Use `.flex-grow-1` to allow an item to grow and fill available space.
- **Flex Shrink:** Use `.flex-shrink-0` to prevent shrinking.

```html
<div class="d-flex">
  <div class="flex-grow-1">Item 1</div>
  <div>Item 2</div>
</div>
```

### **7. Auto Margins**

Use `.ms-auto` and `.me-auto` to push flex items to the left or right respectively.

```html
<div class="d-flex">
  <div class="ms-auto">Item 1</div>
  <div>Item 2</div>
</div>
```

### **8. Flex Wrap**

Control wrapping of flex items using:
- `.flex-wrap`: Allows items to wrap.
- `.flex-nowrap`: Prevents wrapping.
- `.flex-wrap-reverse`: Wraps in reverse order.

```html
<div class="d-flex flex-wrap">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

### **9. Flex Order**

Change the order of flex items using the `.order-*` classes.

```html
<div class="d-flex">
  <div class="order-3">Item 1</div>
  <div class="order-1">Item 2</div>
</div>
```

### **10. Align Content**

Align multiple rows of flex items using `.align-content-*`. It only works if you have multiple rows of items (when `flex-wrap: wrap`).

```html
<div class="d-flex flex-wrap align-content-between">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

---

### **Note:**

Using Flexbox in Bootstrap allows for the quick and responsive design of layouts with minimal effort. Utilize the utilities provided by Bootstrap to control direction, alignment, growth, shrinking, wrapping, and more.

---

### **Further Reading & Resources**
- Official [Bootstrap Flex Documentation](https://getbootstrap.com/docs/5.0/utilities/flex/)
