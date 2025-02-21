### **Lecture Notes: Card Component in Bootstrap**

---

### **Introduction to Card Component in Bootstrap**

The **Card** component in Bootstrap is a flexible and extensible container for content. It provides a clean and consistent way to present content such as text, images, links, and more in an organized, attractive layout. The **Card** component is widely used for building UI elements such as blog posts, product listings, user profiles, and much more.

In this lecture, we will explore the **Card** component in Bootstrap, how to use it, and how to customize it for various design patterns.

---

### **1. Basic Card Structure**

A basic card in Bootstrap is created using the following structure:

```html
<div class="card" style="width: 18rem;">
  <img src="image.jpg" class="card-img-top" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Card Title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

- **`card`**: The main class for the card component.
- **`card-img-top`**: Adds an image at the top of the card.
- **`card-body`**: Contains the content such as the title, text, and button.
- **`card-title`**: A heading for the card.
- **`card-text`**: A paragraph of text inside the card.
- **`btn btn-primary`**: A Bootstrap button inside the card.

#### Breakdown of the Card:
- **Card Image**: The `img` tag with the class `card-img-top` is used to display an image inside the card at the top.
- **Card Body**: The `div` with class `card-body` contains the content such as a title (`card-title`), description (`card-text`), and actions like buttons or links.

---

### **2. Card with Header and Footer**

You can add headers and footers to cards for more structured content.

#### Example (Card with Header and Footer):

```html
<div class="card" style="width: 18rem;">
  <div class="card-header">
    Featured
  </div>
  <img src="image.jpg" class="card-img-top" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Card Title</h5>
    <p class="card-text">Some content inside the card body.</p>
  </div>
  <div class="card-footer text-muted">
    2 days ago
  </div>
</div>
```

- **`card-header`**: This class is used for adding a header to the card, typically for titles or section identifiers.
- **`card-footer`**: This class is used for adding a footer to the card, often for timestamps, footnotes, or additional actions.

---

### **3. Card Variants (Text Alignment, Color, and Styles)**

Bootstrap provides several utility classes to customize cards for different themes and layouts.

#### Example (Card with Text Alignment and Color):

```html
<div class="card text-center" style="width: 18rem;">
  <div class="card-header">
    Featured
  </div>
  <img src="image.jpg" class="card-img-top" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Card Title</h5>
    <p class="card-text">Some content inside the card body.</p>
    <a href="#" class="btn btn-success">Go somewhere</a>
  </div>
  <div class="card-footer text-muted">
    2 days ago
  </div>
</div>
```

- **`text-center`**: Centers the text inside the card.
- **`text-muted`**: Applies a muted color to the footer text.
- **`btn-success`**: Applies a green color to the button.

#### Example (Card with Background Color):

```html
<div class="card bg-primary text-white" style="width: 18rem;">
  <img src="image.jpg" class="card-img-top" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Card Title</h5>
    <p class="card-text">Some content inside the card body with a primary background.</p>
  </div>
</div>
```

- **`bg-primary`**: Applies a primary background color to the card.
- **`text-white`**: Changes the text color to white to improve contrast against the primary background.

---

### **4. Card Groups**

When you have multiple cards that should be displayed together, you can use **Card Groups**. This ensures that all cards are the same height and are aligned properly.

#### Example (Card Group):

```html
<div class="card-group">
  <div class="card">
    <img src="image1.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 1</h5>
      <p class="card-text">Content for card 1</p>
    </div>
  </div>
  <div class="card">
    <img src="image2.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 2</h5>
      <p class="card-text">Content for card 2</p>
    </div>
  </div>
  <div class="card">
    <img src="image3.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 3</h5>
      <p class="card-text">Content for card 3</p>
    </div>
  </div>
</div>
```

- **`card-group`**: This class is used to group multiple cards into one section. Cards inside the group will be evenly sized and aligned.

---

### **5. Card Decks**

If you want to create more complex layouts for your cards, such as arranging them in rows and ensuring they are the same height, you can use **Card Decks**.

#### Example (Card Deck):

```html
<div class="card-deck">
  <div class="card">
    <img src="image1.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 1</h5>
      <p class="card-text">Content for card 1</p>
    </div>
  </div>
  <div class="card">
    <img src="image2.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 2</h5>
      <p class="card-text">Content for card 2</p>
    </div>
  </div>
  <div class="card">
    <img src="image3.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 3</h5>
      <p class="card-text">Content for card 3</p>
    </div>
  </div>
</div>
```

- **`card-deck`**: This class creates a flexible, responsive grid of cards where each card is the same height. The cards automatically adjust for smaller screens.

---

### **6. Card Columns**

**Card Columns** is a layout where cards are arranged in a masonry-style grid.

#### Example (Card Columns):

```html
<div class="card-columns">
  <div class="card">
    <img src="image1.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 1</h5>
      <p class="card-text">Content for card 1</p>
    </div>
  </div>
  <div class="card">
    <img src="image2.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 2</h5>
      <p class="card-text">Content for card 2</p>
    </div>
  </div>
  <div class="card">
    <img src="image3.jpg" class="card-img-top" alt="Card image cap">
    <div class="card-body">
      <h5 class="card-title">Card 3</h5>
      <p class="card-text">Content for card 3</p>
    </div>
  </div>
</div>
```

- **`card-columns`**: This class applies a masonry-style layout to the cards, allowing them to be arranged dynamically based on the content. Cards in this layout will have varying heights.

---

### **7. Practical Examples and Use Cases**

#### Example (Product Cards):

```html
<div class="card-deck">
  <div class="card">
    <img src="product1.jpg" class="card-img-top" alt="Product 1">
    <div class="card-body">
      <h5 class="card-title">Product 1</h5>
      <p class="card-text">A great product for your needs.</p>
      <a href="#" class="btn btn-success">Buy Now</a>
    </div>
  </div>
  <div class="card">
    <img src="product2.jpg" class="card-img-top" alt="Product 2">
    <div class="card-body">
      <h5 class="card-title">Product 2</h5>
      <p class="card-text">An excellent choice for your collection.</p>
      <a href="#" class="btn btn-success">Buy Now</a>
    </div>
  </div>
</div>
```

#### Example (User Profile Card):

```html
<div class="card" style="width: 18rem;">
  <img src="user.jpg" class="card-img-top" alt="User Profile">
  <div class="card-body text-center">
    <h5 class="card-title">Pawan Maurya</h5>
    <p class="card-text">Web Developer</p>
    <a href="#" class="btn btn-info">Follow</a>
  </div>
</div>
```

---

### **Note:**

The **Card** component in Bootstrap provides a flexible and organized way to display content. It is highly customizable with support for:
- Images, titles, text, and buttons
- Headers and footers
- Grouping multiple cards into a cohesive layout with **Card Groups** and **Card Decks**
- Responsive grid layouts with **Card Columns**

