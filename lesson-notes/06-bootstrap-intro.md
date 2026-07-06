# Introduction to Bootstrap – Quick Notes

## What is Bootstrap?

**Bootstrap** is a free and popular **CSS framework** used to create modern, responsive websites quickly.

Instead of writing CSS for common styles, Bootstrap provides **ready-made classes** that you can directly use in your HTML.

---

# Why Use Bootstrap?

* Faster web development
* Less CSS to write
* Responsive design (works on mobile, tablet, and desktop)
* Ready-made components and utilities
* Easy to learn and use

---

# Adding Bootstrap

Include the Bootstrap CSS file in the `<head>` section.

```html id="kz5wbg"
<link
rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/css/bootstrap.min.css">
```

---

# Bootstrap Example

```html id="gj5z5e"
<!DOCTYPE html>
<html>
<head>

<link
rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/css/bootstrap.min.css">

</head>

<body class="bg-light">

<h1 class="text-primary text-center mt-4">
    Welcome to Bootstrap
</h1>

<p class="text-secondary fs-5 p-3 m-4 bg-warning fw-bold rounded">
    Bootstrap makes web design faster and easier.
</p>

</body>
</html>
```

---

# Text Color Classes

| Class            | Color         |
| ---------------- | ------------- |
| `text-primary`   | Blue          |
| `text-secondary` | Gray          |
| `text-success`   | Green         |
| `text-danger`    | Red           |
| `text-warning`   | Orange/Yellow |
| `text-info`      | Cyan          |
| `text-dark`      | Black         |
| `text-light`     | White         |
| `text-white`     | White         |

### Example

```html id="wqkqva"
<p class="text-danger">This text is red.</p>

<p class="text-success">This text is green.</p>

<p class="text-primary">This text is blue.</p>
```

---

# Background Color Classes

| Class        | Background Color |
| ------------ | ---------------- |
| `bg-primary` | Blue             |
| `bg-success` | Green            |
| `bg-danger`  | Red              |
| `bg-warning` | Yellow           |
| `bg-info`    | Cyan             |
| `bg-dark`    | Black            |
| `bg-light`   | Light Gray       |

### Example

```html id="4hmsvd"
<p class="bg-success text-white p-3">
    Green background
</p>
```

---

# Font Size Classes

Bootstrap provides predefined font sizes.

| Class  | Size         |
| ------ | ------------ |
| `fs-1` | Largest      |
| `fs-2` | Large        |
| `fs-3` | Medium Large |
| `fs-4` | Medium       |
| `fs-5` | Small        |
| `fs-6` | Smallest     |

### Example

```html id="g17mt5"
<p class="fs-1">Large Text</p>

<p class="fs-4">Medium Text</p>

<p class="fs-6">Small Text</p>
```

---

# Font Style Classes

| Class        | Purpose     |
| ------------ | ----------- |
| `fw-bold`    | Bold text   |
| `fw-normal`  | Normal text |
| `fw-light`   | Light text  |
| `fst-italic` | Italic text |

### Example

```html id="h2a3b2"
<p class="fw-bold">
    Bold Text
</p>

<p class="fst-italic">
    Italic Text
</p>
```

---

# Padding Classes

Padding adds **space inside** an element.

| Class          | Meaning              |
| -------------- | -------------------- |
| `p-1` to `p-5` | Padding on all sides |
| `pt-3`         | Top padding          |
| `pb-3`         | Bottom padding       |
| `ps-3`         | Left padding         |
| `pe-3`         | Right padding        |
| `px-3`         | Left & Right padding |
| `py-3`         | Top & Bottom padding |

### Example

```html id="tqk7dw"
<div class="bg-info p-4">
    This box has padding.
</div>
```

---

# Margin Classes

Margin adds **space outside** an element.

| Class          | Meaning             |
| -------------- | ------------------- |
| `m-1` to `m-5` | Margin on all sides |
| `mt-3`         | Top margin          |
| `mb-3`         | Bottom margin       |
| `ms-3`         | Left margin         |
| `me-3`         | Right margin        |
| `mx-3`         | Left & Right margin |
| `my-3`         | Top & Bottom margin |

### Example

```html id="s0gxwt"
<div class="bg-warning p-3 m-4">
    Margin around this box
</div>
```

---

# Combined Example

```html id="aymbx3"
<div class="container mt-5">

<h1 class="text-primary text-center fw-bold">
    Bootstrap Demo
</h1>

<p class="bg-light text-secondary fs-5 p-4 mt-4 rounded border">
    Bootstrap utility classes help you style webpages quickly without writing custom CSS.
</p>

<p class="bg-success text-white p-3 fw-bold fst-italic mt-3 rounded">
    Learning Bootstrap is simple and fun!
</p>

</div>
```

---

# Best Practices

* Use Bootstrap classes instead of writing CSS for common styles.
* Combine multiple utility classes to create attractive layouts.
* Use meaningful spacing with `p-*` and `m-*` classes.
* Use Bootstrap color classes consistently.
* Prefer Bootstrap utilities for simple styling and custom CSS for complex designs.

---

# Summary

* **Bootstrap** is a CSS framework that speeds up web development.
* Use `text-*` classes to change text color.
* Use `bg-*` classes to change background color.
* Use `fs-*` classes to change font size.
* Use `fw-*` and `fst-*` classes to style text.
* Use `p-*` classes for padding.
* Use `m-*` classes for margin.
* Multiple Bootstrap classes can be combined on the same element.
