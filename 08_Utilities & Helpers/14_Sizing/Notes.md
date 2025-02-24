## **Lecture Notes: Sizing in Bootstrap**

### **What is Sizing?**
Sizing allows us to easily control the **width** and **height** of elements on a webpage. Bootstrap provides utility classes to set the **width** and **height** in various ways.

### **Width Utilities**

You can control the width of elements using Bootstrap's predefined width utilities. These include:

- `.w-25`: Set width to 25% of the parent container.
- `.w-50`: Set width to 50% of the parent container.
- `.w-75`: Set width to 75% of the parent container.
- `.w-100`: Set width to 100% of the parent container.
- `.w-auto`: Set width to auto (default width based on content).

#### **Example: Width Utilities**

```html
<div class="w-25 p-3">Width 25%</div>
<div class="w-50 p-3">Width 50%</div>
<div class="w-75 p-3">Width 75%</div>
<div class="w-100 p-3">Width 100%</div>
<div class="w-auto p-3">Width auto</div>
```

### **Height Utilities**

Similarly, you can control the height of elements using height utilities. These include:

- `.h-25`: Set height to 25% of the parent container.
- `.h-50`: Set height to 50% of the parent container.
- `.h-75`: Set height to 75% of the parent container.
- `.h-100`: Set height to 100% of the parent container.
- `.h-auto`: Set height to auto (based on content).

#### **Example: Height Utilities**

```html
<div style="height: 100px;">
  <div class="h-25 d-inline-block" style="width: 120px;">Height 25%</div>
  <div class="h-50 d-inline-block" style="width: 120px;">Height 50%</div>
  <div class="h-75 d-inline-block" style="width: 120px;">Height 75%</div>
  <div class="h-100 d-inline-block" style="width: 120px;">Height 100%</div>
  <div class="h-auto d-inline-block" style="width: 120px;">Height auto</div>
</div>
```

### **Max Width and Max Height Utilities**

- `.mw-100`: Set max-width to 100%.
- `.mh-100`: Set max-height to 100%.

#### **Example: Max Width**

```html
<div style="width: 50%; height: 100px;">
  <div class="mw-100" style="width: 200%;">Max-width 100%</div>
</div>
```

#### **Example: Max Height**

```html
<div style="height: 100px;">
  <div class="mh-100" style="width: 100px; height: 200px;">Max-height 100%</div>
</div>
```

### **Relative to the Viewport**

You can also set width and height relative to the viewport (the visible part of the browser window):

- `.vw-100`: Set width to 100% of the viewport width.
- `.vh-100`: Set height to 100% of the viewport height.
- `.min-vw-100`: Set minimum width to 100% of the viewport width.
- `.min-vh-100`: Set minimum height to 100% of the viewport height.

#### **Example: Relative to Viewport**

```html
<div class="min-vw-100">Min-width 100vw</div>
<div class="min-vh-100">Min-height 100vh</div>
<div class="vw-100">Width 100vw</div>
<div class="vh-100">Height 100vh</div>
```

---