## **Lecture Notes: Z-index in Bootstrap**

### **What is Z-index?**
- **Z-index** controls the order of elements when they overlap on a page.
- Higher Z-index values make elements appear on top of others.
- It only works on **positioned elements** (`relative`, `absolute`, `fixed`, or `sticky`).

### **Bootstrap Z-index Utilities**
Bootstrap provides utility classes to set Z-index easily. These values range from `-1` to `3`.

#### **Z-index Classes in Bootstrap:**
- `.z-0`: Z-index value of 0 (default).
- `.z-1`: Z-index value of 1.
- `.z-2`: Z-index value of 2.
- `.z-3`: Z-index value of 3.
- `.z-n1`: Z-index value of -1 (pushes element behind others).

### **Example: Stacking Elements with Z-index**

```html
<div class="z-3 position-absolute p-5"><span>z-3</span></div>
<div class="z-2 position-absolute p-5"><span>z-2</span></div>
<div class="z-1 position-absolute p-5"><span>z-1</span></div>
<div class="z-0 position-absolute p-5"><span>z-0</span></div>
<div class="z-n1 position-absolute p-5"><span>z-n1</span></div>
```

- **Positioning**: `position-absolute` makes the elements stack properly.
- **Z-index**: Higher values stack on top of lower ones.

### **Overlay Components in Bootstrap**
Bootstrap components like **modals**, **tooltips**, and **dropdowns** use higher Z-index values to appear on top of other content.

---