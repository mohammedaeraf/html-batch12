# Lesson Notes – Bootstrap Cards

## Learning Objectives

By the end of this lesson, you will be able to:

- Understand what a Bootstrap Card is.
- Create simple and attractive cards.
- Add images, titles, text, and buttons to cards.
- Apply Bootstrap utility classes to enhance card appearance.

---

# 1. What is a Bootstrap Card?

A **Bootstrap Card** is a flexible and responsive container used to display content such as:

- Images
- Titles
- Text
- Buttons
- Links

Cards are commonly used for:

- Product listings
- Course information
- Team members
- Blog posts
- News articles
- Hotel and restaurant listings

---

# 2. Basic Card

A card consists of a container with a **card body** that holds its content.

## Syntax

```html
<div class="card">
  <div class="card-body">
    <h5 class="card-title">Card Title</h5>

    <p class="card-text">This is a simple Bootstrap card.</p>
  </div>
</div>
```

---

# Output

```
+-----------------------------+
| Card Title                  |
|                             |
| This is a simple card.      |
+-----------------------------+
```

---

# 3. Card with Image

Images can be displayed at the top of the card using the `card-img-top` class.

## Example

```html
<div class="card" style="width:22rem;">
  <img src="images/laptop.jpg" class="card-img-top" alt="Laptop" />

  <div class="card-body">
    <h4 class="card-title">Laptop</h4>

    <p class="card-text">
      A powerful laptop suitable for programming, designing and office work.
    </p>
  </div>
</div>
```

---

# 4. Card with Button

Buttons can be added inside the card body.

```html
<div class="card" style="width:22rem;">
  <img src="images/mobile.jpg" class="card-img-top" alt="Mobile" />

  <div class="card-body">
    <h4 class="card-title">Samsung Galaxy</h4>

    <p class="card-text">
      A modern smartphone with an excellent camera and long-lasting battery.
    </p>

    <button class="btn btn-primary">Buy Now</button>
  </div>
</div>
```

---

# 5. Card with Two Buttons

Multiple buttons can be added for different actions.

```html
<div class="card" style="width:22rem;">
  <img src="images/headphones.jpg" class="card-img-top" alt="Headphones" />

  <div class="card-body">
    <h4 class="card-title">Wireless Headphones</h4>

    <p class="card-text">
      Enjoy crystal-clear sound with wireless Bluetooth connectivity.
    </p>

    <button class="btn btn-success me-2">Buy Now</button>

    <button class="btn btn-outline-primary">View Details</button>
  </div>
</div>
```

---

# 6. Card with Shadow and Rounded Corners

Bootstrap utility classes can make cards look more attractive.

```html
<div class="card shadow rounded p-2" style="width:22rem;">
  <img src="images/camera.jpg" class="card-img-top rounded" alt="Camera" />

  <div class="card-body">
    <h4 class="card-title">DSLR Camera</h4>

    <p class="card-text">
      Capture stunning photos with professional image quality.
    </p>

    <a href="#" class="btn btn-dark"> Learn More </a>
  </div>
</div>
```

---

# 7. Common Card Classes

| Class                 | Description                            |
| --------------------- | -------------------------------------- |
| `card`                | Creates the card container             |
| `card-body`           | Holds the card content                 |
| `card-title`          | Displays the card heading              |
| `card-text`           | Displays the card description          |
| `card-img-top`        | Places an image at the top of the card |
| `btn`                 | Creates a Bootstrap button             |
| `btn-primary`         | Blue button                            |
| `btn-success`         | Green button                           |
| `btn-danger`          | Red button                             |
| `btn-warning`         | Yellow button                          |
| `btn-dark`            | Black button                           |
| `btn-outline-primary` | Blue outlined button                   |
| `shadow`              | Adds a shadow                          |
| `shadow-lg`           | Adds a larger shadow                   |
| `rounded`             | Adds rounded corners                   |
| `p-2`                 | Adds padding                           |
| `mb-4`                | Adds bottom margin                     |
| `me-2`                | Adds space to the right of an element  |

---

# Complete Demo

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>Bootstrap Cards</title>

    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
  </head>

  <body>
    <div class="container my-5">
      <h1 class="text-center text-primary display-4 fw-bold mb-5">
        Electronic Store
      </h1>

      <div class="card shadow rounded mb-4" style="width:22rem;">
        <img src="images/laptop.jpg" class="card-img-top" alt="Laptop" />

        <div class="card-body">
          <h4 class="card-title">Laptop</h4>

          <p class="card-text">
            Powerful laptop with Intel Core i7 processor, 16GB RAM and 512GB
            SSD.
          </p>

          <h5 class="text-success">₹59,999</h5>

          <button class="btn btn-primary me-2">Buy Now</button>

          <button class="btn btn-outline-primary">View Details</button>
        </div>
      </div>
    </div>
  </body>
</html>
```

---

# Summary

| Bootstrap Class       | Purpose                      |
| --------------------- | ---------------------------- |
| `card`                | Creates the card             |
| `card-body`           | Contains the card content    |
| `card-title`          | Card heading                 |
| `card-text`           | Card description             |
| `card-img-top`        | Image at the top of the card |
| `btn`                 | Creates a button             |
| `btn-primary`         | Blue button                  |
| `btn-outline-primary` | Outlined blue button         |
| `shadow`              | Adds a shadow                |
| `rounded`             | Rounds the card corners      |
| `me-2`                | Adds spacing between buttons |
| `mb-4`                | Adds bottom margin           |

---

