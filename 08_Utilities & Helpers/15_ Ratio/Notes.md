## **Lecture Notes: Aspect Ratios in Bootstrap**

### **What are Aspect Ratios?**
An **aspect ratio** is the ratio of the width to the height of an element, typically used in media content like **videos**, **images**, or **slideshows**. It ensures that the content maintains the correct proportion when displayed.

### **Bootstrap Aspect Ratio Utilities**
Bootstrap provides an easy way to maintain the aspect ratio of embedded content like videos, iframes, and images. It uses **pseudo-elements** to create the desired ratio for responsive content.

### **How to Use Aspect Ratio Utilities**
To use the aspect ratio utilities:
1. Wrap your embedded content (like an `<iframe>`) in a parent `<div>` with the class `.ratio`.
2. Add a modifier class (like `.ratio-16x9`) to set the aspect ratio.

#### **Example: Using Aspect Ratio Utilities**

```html
<div class="ratio ratio-16x9">
  <iframe src="https://www.youtube.com/embed/zpOULjyy-n8?rel=0" title="YouTube video" allowfullscreen></iframe>
</div>
```

### **Aspect Ratios**
Bootstrap provides several default aspect ratios, including:
- **1x1**: Square aspect ratio (1:1).
- **4x3**: Traditional television aspect ratio (4:3).
- **16x9**: Widescreen aspect ratio (16:9).
- **21x9**: Ultra-widescreen aspect ratio (21:9).

#### **Example: Aspect Ratios**

```html
<div class="ratio ratio-1x1">
  <div>1x1</div>
</div>
<div class="ratio ratio-4x3">
  <div>4x3</div>
</div>
<div class="ratio ratio-16x9">
  <div>16x9</div>
</div>
<div class="ratio ratio-21x9">
  <div>21x9</div>
</div>
```
