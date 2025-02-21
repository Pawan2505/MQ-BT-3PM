### **Lecture Notes: Tables in Bootstrap**

---

### **Introduction to Tables in Bootstrap**

In this lecture Notes, We will learn to use Bootstrap's table utilities like striped rows, bordered tables, and responsive tables.

---

### **1. Basic Table Structure**


```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">State</th>
      <th scope="col">City</th>
      <th scope="col">Population (in millions)</th>
      <th scope="col">Area (in km²)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Uttar Pradesh</td>
      <td>Lucknow</td>
      <td>3.2</td>
      <td>35,878</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Maharashtra</td>
      <td>Mumbai</td>
      <td>20.4</td>
      <td>603</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>West Bengal</td>
      <td>Kolkata</td>
      <td>4.5</td>
      <td>185</td>
    </tr>
    <tr>
      <th scope="row">4</th>
      <td>Tamil Nadu</td>
      <td>Chennai</td>
      <td>8.9</td>
      <td>1,264</td>
    </tr>
  </tbody>
</table>
```

This is a basic structure where:
- **`<thead>`** contains the table headers.
- **`<tbody>`** contains the rows with data such as state, city, population, and area.

---

### **2. Styling Tables with Bootstrap Classes**

Let's add some Bootstrap classes to style the table and make it look better.

#### **Striped Rows**

The **`table-striped`** class adds alternating row colors for better readability.

```html
<table class="table table-striped">
  <!-- Table content here -->
</table>
```

#### **Hoverable Rows**

The **`table-hover`** class adds a hover effect to the rows, making the user experience more interactive.

```html
<table class="table table-striped table-hover">
  <!-- Table content here -->
</table>
```

#### **Bordered Tables**

To add borders around all the cells, we use the **`table-bordered`** class.

```html
<table class="table table-bordered">
  <!-- Table content here -->
</table>
```

#### **Table with Contextual Classes**

Using **contextual classes** such as `table-success`, `table-danger`, `table-warning`, etc., to highlight specific rows based on the data.

Example: We can use `table-success` to highlight the states with larger populations and `table-warning` for smaller ones.

```html
<table class="table table-bordered">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">State</th>
      <th scope="col">City</th>
      <th scope="col">Population (in millions)</th>
      <th scope="col">Area (in km²)</th>
    </tr>
  </thead>
  <tbody>
    <tr class="table-success">
      <th scope="row">1</th>
      <td>Uttar Pradesh</td>
      <td>Lucknow</td>
      <td>3.2</td>
      <td>35,878</td>
    </tr>
    <tr class="table-danger">
      <th scope="row">2</th>
      <td>Maharashtra</td>
      <td>Mumbai</td>
      <td>20.4</td>
      <td>603</td>
    </tr>
    <tr class="table-warning">
      <th scope="row">3</th>
      <td>West Bengal</td>
      <td>Kolkata</td>
      <td>4.5</td>
      <td>185</td>
    </tr>
    <tr class="table-success">
      <th scope="row">4</th>
      <td>Tamil Nadu</td>
      <td>Chennai</td>
      <td>8.9</td>
      <td>1,264</td>
    </tr>
  </tbody>
</table>
```

- **`table-success`**: Highlights the row with a green background for states with large populations.
- **`table-danger`**: Highlights the row with a red background for high-density areas.
- **`table-warning`**: Yellow background for moderate population areas.

---

### **3. Making Tables Responsive**

To make the table scrollable horizontally on smaller screens, use the **`table-responsive`** class.

```html
<div class="table-responsive">
  <table class="table table-striped table-hover">
    <!-- Table content here -->
  </table>
</div>
```

- **`table-responsive`**: Ensures the table is scrollable horizontally on small devices.

---

### **4. Table with Bootstrap**

```html
<div class="container mt-5">
  <h2>Indian States and Cities Data</h2>
  <div class="table-responsive">
    <table class="table table-striped table-hover table-bordered">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">State</th>
          <th scope="col">City</th>
          <th scope="col">Population (in millions)</th>
          <th scope="col">Area (in km²)</th>
        </tr>
      </thead>
      <tbody>
        <tr class="table-success">
          <th scope="row">1</th>
          <td>Uttar Pradesh</td>
          <td>Lucknow</td>
          <td>3.2</td>
          <td>35,878</td>
        </tr>
        <tr class="table-danger">
          <th scope="row">2</th>
          <td>Maharashtra</td>
          <td>Mumbai</td>
          <td>20.4</td>
          <td>603</td>
        </tr>
        <tr class="table-warning">
          <th scope="row">3</th>
          <td>West Bengal</td>
          <td>Kolkata</td>
          <td>4.5</td>
          <td>185</td>
        </tr>
        <tr class="table-success">
          <th scope="row">4</th>
          <td>Tamil Nadu</td>
          <td>Chennai</td>
          <td>8.9</td>
          <td>1,264</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
```

---

### **5. Practical Use Cases for Tables**

- **Census Data**: Display population data of Indian states, cities, and districts.
- **Education Statistics**: Organize information about Indian universities, their courses, and enrollment numbers.
- **Weather Reports**: Display daily weather data for Indian cities.

---

### **Note:**

In this lecture Notes, we have:
- Learned how to create and style tables using Bootstrap with Indian data.
- Discussed and implemented Bootstrap classes like `table-striped`, `table-bordered`, `table-hover`, and contextual classes.
- Made tables responsive for mobile and tablet devices.
- Explored practical use cases of tables with real-world data.
