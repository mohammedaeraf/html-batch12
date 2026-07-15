# Lesson Notes – Bootstrap Grid Layout

## Learning Objectives

By the end of this lesson, you will be able to:

* Understand the Bootstrap Grid System.
* Create rows and columns.
* Divide a page into 12 equal columns.
* Build responsive layouts.
* Display Bootstrap cards side by side.

---

# 1. What is the Bootstrap Grid System?

Bootstrap provides a **12-column responsive grid system** for arranging content.

It helps create layouts that automatically adjust to different screen sizes.

The Grid System is based on three main elements:

* Container
* Row
* Column

```
Container
    └── Row
            ├── Column
            ├── Column
            └── Column
```

---

# 2. Grid Structure

Every Bootstrap grid follows this structure:

```html
<div class="container">

    <div class="row">

        <div class="col">
            Column 1
        </div>

        <div class="col">
            Column 2
        </div>

    </div>

</div>
```

---

# 3. Equal Width Columns

Bootstrap automatically divides available space equally.

```html
<div class="container">

<div class="row">

<div class="col bg-primary text-white p-3">
Column 1
</div>

<div class="col bg-success text-white p-3">
Column 2
</div>

</div>

</div>
```

---

### Output

```
-------------------------------
| Column 1 | Column 2 |
-------------------------------
```

---

# 4. Three Equal Columns

```html
<div class="container">

<div class="row">

<div class="col bg-primary text-white p-3">
Column 1
</div>

<div class="col bg-success text-white p-3">
Column 2
</div>

<div class="col bg-warning p-3">
Column 3
</div>

</div>

</div>
```

---

# 5. Fixed Column Sizes

Bootstrap divides each row into **12 columns**.

Example:

```html
<div class="row">

<div class="col-4 bg-primary text-white">
4 Columns
</div>

<div class="col-8 bg-success text-white">
8 Columns
</div>

</div>
```

Since:

```
4 + 8 = 12
```

---

More examples:

| Layout        | Classes        |
| ------------- | -------------- |
| 6 + 6         | `col-6 col-6`  |
| 3 + 9         | `col-3 col-9`  |
| 2 + 10        | `col-2 col-10` |
| 3 + 3 + 3 + 3 | `col-3` ×4     |

---

# 6. Responsive Columns

Columns can change based on screen size.

```html
<div class="row">

<div class="col-md-6">
Column 1
</div>

<div class="col-md-6">
Column 2
</div>

</div>
```

### Behavior

Small screen

```
Column 1
Column 2
```

Medium and larger

```
Column 1 | Column 2
```

---

# 7. Three Responsive Cards

This is the real-world use of the grid system.

```html
<div class="container">

<div class="row">

<div class="col-md-4">

<div class="card shadow">

<img src="images/laptop.jpg"
class="card-img-top">

<div class="card-body">

<h5>Laptop</h5>

<p>Powerful laptop for professionals.</p>

<button class="btn btn-primary">
Buy Now
</button>

</div>

</div>

</div>

<div class="col-md-4">

<div class="card shadow">

<img src="images/mobile.jpg"
class="card-img-top">

<div class="card-body">

<h5>Smartphone</h5>

<p>Latest Android smartphone.</p>

<button class="btn btn-primary">
Buy Now
</button>

</div>

</div>

</div>

<div class="col-md-4">

<div class="card shadow">

<img src="images/headphones.jpg"
class="card-img-top">

<div class="card-body">

<h5>Headphones</h5>

<p>Wireless Bluetooth headphones.</p>

<button class="btn btn-primary">
Buy Now
</button>

</div>

</div>

</div>

</div>

</div>
```

### On Large Screens

```
-----------------------------------------
| Card | Card | Card |
-----------------------------------------
```

### On Mobile

```
Card

Card

Card
```

---

# 8. Gap Between Columns

Use `g-*` classes.

```html
<div class="row g-4">

<div class="col">
...
</div>

<div class="col">
...
</div>

</div>
```

Examples:

* `g-1`
* `g-2`
* `g-3`
* `g-4`
* `g-5`

---

# Complete Demo

```html
<!DOCTYPE html>
<html>

<head>

<title>Bootstrap Grid</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
rel="stylesheet">

</head>

<body>

<div class="container my-5">

<h1 class="text-center text-primary mb-5">
Electronic Store
</h1>

<div class="row g-4">

<div class="col-md-4">

<div class="card shadow">

<img src="images/laptop.jpg"
class="card-img-top">

<div class="card-body">

<h4>Laptop</h4>

<p>High-performance laptop.</p>

<button class="btn btn-primary">
Buy Now
</button>

</div>

</div>

</div>

<div class="col-md-4">

<div class="card shadow">

<img src="images/mobile.jpg"
class="card-img-top">

<div class="card-body">

<h4>Smartphone</h4>

<p>Latest Android smartphone.</p>

<button class="btn btn-primary">
Buy Now
</button>

</div>

</div>

</div>

<div class="col-md-4">

<div class="card shadow">

<img src="images/headphones.jpg"
class="card-img-top">

<div class="card-body">

<h4>Headphones</h4>

<p>Wireless Bluetooth headphones.</p>

<button class="btn btn-primary">
Buy Now
</button>

</div>

</div>

</div>

</div>

</div>

</body>

</html>
```

---

# Common Grid Classes

| Class               | Description                            |
| ------------------- | -------------------------------------- |
| `container`         | Holds the grid                         |
| `row`               | Creates a horizontal row               |
| `col`               | Equal-width column                     |
| `col-1` to `col-12` | Fixed-width columns                    |
| `col-sm-*`          | Small devices (≥576px)                 |
| `col-md-*`          | Medium devices (≥768px)                |
| `col-lg-*`          | Large devices (≥992px)                 |
| `col-xl-*`          | Extra-large devices (≥1200px)          |
| `col-xxl-*`         | Extra-extra-large devices (≥1400px)    |
| `g-*`               | Adds spacing (gutters) between columns |

---

# Summary

* A Bootstrap grid is built using **Container → Row → Column**.
* Every row is divided into **12 columns**.
* Use `col` for equal-width columns.
* Use `col-4`, `col-6`, etc., for fixed-width layouts.
* Use responsive classes like `col-md-4` to create layouts that stack on smaller screens.
* The Grid System is commonly used to arrange **Cards**, images, forms, and other page sections side by side.

---

# Practice Exercise

Create a webpage titled **"Our Products"**.

Requirements:

* Add a `container` with a page heading.
* Create a `row` with a **gap of 4** (`g-4`).
* Add **three `col-md-4` columns**.
* Inside each column, create a Bootstrap card for:

  * Laptop
  * Smartphone
  * Smart Watch
* Each card should include:

  * Product image
  * Product name
  * Short description
  * Price
  * **Buy Now** button

**Expected Result:**

* On **large screens**, the three cards should appear **side by side**.
* On **mobile devices**, the cards should **stack vertically** automatically.
