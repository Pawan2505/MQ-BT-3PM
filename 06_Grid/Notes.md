## **Lecture Notes: Bootstrap Grid System** 

The **Bootstrap Grid System** is a **responsive, mobile-first** layout system that divides a page into **12 equal columns**. Using rows and columns, we can create **flexible and dynamic** layouts.  

---

## **Why Use Bootstrap Grid?**  
✅ **Responsive Design** – Automatically adjusts for different screen sizes.  
✅ **Mobile-First Approach** – Works well on all devices.  
✅ **Easy to Use** – Predefined classes for layouts.  
✅ **Customizable** – Define how elements should behave at different breakpoints.  

---

## **Grid System Basics**  

### **1. Container & Container-Fluid**  
In Bootstrap, every row and column must be inside a **container** to maintain proper alignment.

| Class Name       | Description |
|-----------------|-------------|
| `.container`   | Fixed-width container (changes at breakpoints) |
| `.container-fluid` | Full-width container (always 100% width) |

**Example:**
```html
<!-- Fixed width container -->
<div class="container">
    <h3>Fixed Container</h3>
</div>

<!-- Full width container -->
<div class="container-fluid">
    <h3>Full Width Container</h3>
</div>
```

---

### **2. Row and Column Structure**  
A **row** contains **12 columns** in total. We can divide them into **equal or custom-sized** columns.

**Example: Equal Columns**  
```html
<div class="container">
    <div class="row">
        <div class="col bg-primary">Column 1</div>
        <div class="col bg-danger">Column 2</div>
        <div class="col bg-success">Column 3</div>
    </div>
</div>
```
🔹 Here, each `.col` class automatically divides the row into **equal-width** columns.

**Example: Custom Column Widths**  
```html
<div class="container">
    <div class="row">
        <div class="col-6 bg-warning">Column 1 (6 columns)</div>
        <div class="col-3 bg-info">Column 2 (3 columns)</div>
        <div class="col-3 bg-secondary">Column 3 (3 columns)</div>
    </div>
</div>
```
🔹 **`.col-6` means the column takes 6 out of 12** (half the row).  
🔹 **`.col-3` means the column takes 3 out of 12** (one-fourth of the row).

---

### **3. Responsive Column Layout**  
Bootstrap allows you to define how many columns an element should take up at different screen sizes.

| Class Name  | Extra Small (<576px) | Small (≥576px) | Medium (≥768px) | Large (≥992px) | Extra Large (≥1200px) |
|------------|-----------------|-----------------|-----------------|-----------------|-----------------|
| `.col-`    | Auto width      | Auto width      | Auto width      | Auto width      | Auto width      |
| `.col-sm-` | 12 Columns (Full Width) | Custom Width | Custom Width | Custom Width | Custom Width |
| `.col-md-` | 12 Columns (Full Width) | 12 Columns (Full Width) | Custom Width | Custom Width | Custom Width |
| `.col-lg-` | 12 Columns (Full Width) | 12 Columns (Full Width) | 12 Columns (Full Width) | Custom Width | Custom Width |

**Example: Different Column Sizes for Different Screens**  
```html
<div class="container">
    <div class="row text-center">
        <div class="col-sm-12 col-md-6 col-lg-4 bg-primary">Column 1</div>
        <div class="col-sm-12 col-md-6 col-lg-4 bg-danger">Column 2</div>
        <div class="col-sm-12 col-md-12 col-lg-4 bg-success">Column 3</div>
    </div>
</div>
```
🔹 **Small Screens (`col-sm-12`)** – Each column takes full width.  
🔹 **Medium Screens (`col-md-6`)** – Each column takes half the row.  
🔹 **Large Screens (`col-lg-4`)** – Each column takes one-third of the row.

---

### **4. Auto-Responsive Columns (`row-cols`)**  
If you don’t want to define column sizes manually, you can use `row-cols` classes.

**Example: Auto-Responsive Layout**  
```html
<div class="container">
    <div class="row row-cols-2 row-cols-md-3 row-cols-lg-4">
        <div class="col bg-warning">Column 1</div>
        <div class="col bg-info">Column 2</div>
        <div class="col bg-dark">Column 3</div>
        <div class="col bg-white">Column 4</div>
    </div>
</div>
```
🔹 **`row-cols-2`** – 2 columns per row on small screens.  
🔹 **`row-cols-md-3`** – 3 columns per row on medium screens.  
🔹 **`row-cols-lg-4`** – 4 columns per row on large screens.

---

### **5. Nested Grid (Grid inside Grid)**  
Sometimes, we need to create **nested grids** inside a column.

**Example: Nested Grid**  
```html
<div class="container">
    <div class="row">
        <div class="col-8 bg-primary">
            Parent Column (8 Columns)
            <div class="row">
                <div class="col-6 bg-warning">Nested Column 1</div>
                <div class="col-6 bg-success">Nested Column 2</div>
            </div>
        </div>
        <div class="col-4 bg-danger">Parent Column (4 Columns)</div>
    </div>
</div>
```
🔹 The **nested row** follows the **12-column rule** inside its parent column.

---

### **6. Offset & Alignment in Grid**  
Bootstrap allows **offsetting** columns to create spacing.

**Example: Column Offset**  
```html
<div class="container">
    <div class="row">
        <div class="col-4 offset-2 bg-primary">Offset by 2</div>
        <div class="col-4 bg-danger">Column 2</div>
    </div>
</div>
```
🔹 **`offset-2`** shifts the column by **2 spaces** from the left.

---

### **7. Column Ordering**  
You can change the order of columns using `.order-*` classes.

**Example: Column Order**  
```html
<div class="container">
    <div class="row">
        <div class="col order-3 bg-primary">Column 1 (Last)</div>
        <div class="col order-1 bg-danger">Column 2 (First)</div>
        <div class="col order-2 bg-success">Column 3 (Middle)</div>
    </div>
</div>
```
🔹 **`.order-1`** – Appears first.  
🔹 **`.order-2`** – Appears second.  
🔹 **`.order-3`** – Appears last.

---

## **Note:**  

| Concept        | Description |
|---------------|-------------|
| **Container** | Wraps the grid system (`.container`, `.container-fluid`) |
| **Row** | Defines a horizontal group of columns |
| **Column (`.col-`)** | Defines column width (max 12 per row) |
| **Responsive Columns** | `col-sm-*`, `col-md-*`, `col-lg-*`, `col-xl-*` |
| **Auto Columns** | `row-cols-2`, `row-cols-md-3`, etc. |
| **Nested Grid** | A grid inside another column |
| **Offset** | Moves columns to the right using `offset-*` |
| **Column Order** | Reorders columns with `order-*` |

---
