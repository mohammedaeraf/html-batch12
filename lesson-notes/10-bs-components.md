# Lesson Notes – Bootstrap Components (Alerts & List Groups)

## Learning Objectives

By the end of this lesson, students will be able to:

* Use Bootstrap Alerts to display messages.
* Organize information using List Groups.
* Combine Bootstrap components to build simple webpages.

---

# 1. What are Bootstrap Components?

Bootstrap Components are **pre-designed UI (User Interface) elements** that help us create attractive websites quickly.

Examples include:

* Alerts
* Cards
* List Groups
* Buttons
* Navbar
* Accordion
* Carousel
* Modal

Today we will learn:

* Alerts
* List Groups

---

# 2. Bootstrap Alert

Alerts are used to display important messages to the user.

## Syntax

```html
<div class="alert alert-primary">
    This is an alert.
</div>
```

---

## Alert Colors

```html
<div class="alert alert-primary">Primary Alert</div>

<div class="alert alert-secondary">Secondary Alert</div>

<div class="alert alert-success">Success Alert</div>

<div class="alert alert-danger">Danger Alert</div>

<div class="alert alert-warning">Warning Alert</div>

<div class="alert alert-info">Info Alert</div>

<div class="alert alert-light">Light Alert</div>

<div class="alert alert-dark">Dark Alert</div>
```

---

## Example

```html
<div class="container mt-4">

    <div class="alert alert-success">
        ✔ Registration completed successfully.
    </div>

    <div class="alert alert-warning">
        ⚠ Please submit your assignment before Friday.
    </div>

    <div class="alert alert-danger">
        ❌ Invalid username or password.
    </div>

</div>
```

---

# 3. Bootstrap List Group

List Groups display related items in a list.

---

## Basic List Group

```html
<ul class="list-group">

<li class="list-group-item">
HTML
</li>

<li class="list-group-item">
CSS
</li>

<li class="list-group-item">
Bootstrap
</li>

<li class="list-group-item">
JavaScript
</li>

</ul>
```

---

## Active Item

```html
<ul class="list-group">

<li class="list-group-item active">
HTML
</li>

<li class="list-group-item">
CSS
</li>

<li class="list-group-item">
Bootstrap
</li>

</ul>
```

---

## Colored List Items

```html
<ul class="list-group">

<li class="list-group-item list-group-item-primary">
HTML
</li>

<li class="list-group-item list-group-item-success">
CSS
</li>

<li class="list-group-item list-group-item-warning">
Bootstrap
</li>

<li class="list-group-item list-group-item-danger">
JavaScript
</li>

</ul>
```

---

## Example – Programming Courses

```html
<div class="container mt-4">

<h2 class="mb-3">
Available Courses
</h2>

<ul class="list-group">

<li class="list-group-item active">
Programming Courses
</li>

<li class="list-group-item">
Python
</li>

<li class="list-group-item">
Java
</li>

<li class="list-group-item">
PHP
</li>

<li class="list-group-item">
React
</li>

<li class="list-group-item">
Laravel
</li>

</ul>

</div>
```

---

# Complete Demo

```html
<!DOCTYPE html>
<html>

<head>

<title>Bootstrap Components</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
rel="stylesheet">

</head>

<body>

<div class="container my-5">

<h1 class="text-center text-primary mb-5">
Bootstrap Components Demo
</h1>

<!-- Alert -->

<div class="alert alert-success">
Welcome to Bootstrap Components!
</div>

<div class="alert alert-info">
Today's lesson covers Bootstrap Alerts and List Groups.
</div>

<!-- List Group -->

<h3 class="mt-4">Programming Languages</h3>

<ul class="list-group">

<li class="list-group-item active">
Popular Languages
</li>

<li class="list-group-item">
Python
</li>

<li class="list-group-item">
Java
</li>

<li class="list-group-item">
PHP
</li>

<li class="list-group-item">
JavaScript
</li>

</ul>

</div>

</body>

</html>
```

---

# Summary

| Component           | Purpose                                 |
| ------------------- | --------------------------------------- |
| `alert`             | Displays important messages             |
| `list-group`        | Creates a styled list                   |
| `list-group-item`   | Individual list item                    |
| `active`            | Highlights the selected list item       |
| `list-group-item-*` | Applies contextual colors to list items |

