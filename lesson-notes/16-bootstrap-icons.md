# Lesson Notes – Bootstrap Icons

## Learning Objectives

By the end of this lesson, you will be able to:

* Understand what Bootstrap Icons are.
* Add Bootstrap Icons to a webpage.
* Display icons using Bootstrap classes.
* Change the size and color of icons.
* Use icons inside headings, buttons, and alerts.

---

# 1. What are Bootstrap Icons?

**Bootstrap Icons** are a collection of free, high-quality icons created by the Bootstrap team.

They can be used to make websites more attractive and user-friendly.

Examples include:

* 🏠 Home
* 🔍 Search
* ❤️ Heart
* 📧 Email
* 🛒 Shopping Cart
* 📍 Location
* ✈ Airplane

---

# 2. Why Use Bootstrap Icons?

Bootstrap Icons help to:

* Improve the appearance of webpages.
* Make buttons more meaningful.
* Enhance navigation.
* Display information visually.

---

# 3. Step 1 – Add Bootstrap Icons

Add the Bootstrap Icons CDN inside the `<head>` section.

```html id="ywjlwm"
<link
rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.13.1/font/bootstrap-icons.min.css">
```

Now you can use any Bootstrap Icon in your webpage.

---

# 4. Step 2 – Add an Icon

Icons are added using the `<i>` tag.

### Syntax

```html id="2s0oaq"
<i class="bi bi-house-fill"></i>
```

---

### Example

```html id="rqarfm"
<h2>

<i class="bi bi-house-fill"></i>

Home

</h2>
```

---

# 5. Popular Bootstrap Icons

| Icon         | Class                  |
| ------------ | ---------------------- |
| 🏠 Home      | `bi bi-house-fill`     |
| 🔍 Search    | `bi bi-search`         |
| ❤️ Heart     | `bi bi-heart-fill`     |
| ⭐ Star       | `bi bi-star-fill`      |
| 📧 Envelope  | `bi bi-envelope-fill`  |
| 📞 Telephone | `bi bi-telephone-fill` |
| 🛒 Cart      | `bi bi-cart-fill`      |
| 👤 Person    | `bi bi-person-fill`    |
| 📍 Location  | `bi bi-geo-alt-fill`   |
| ✈ Airplane   | `bi bi-airplane-fill`  |
| 🏨 Building  | `bi bi-building`       |
| 🌳 Tree      | `bi bi-tree-fill`      |
| ☀ Sun        | `bi bi-sun-fill`       |
| 🏖 Umbrella  | `bi bi-umbrella-fill`  |

---

# 6. Changing Icon Size

Bootstrap provides font-size utility classes.

```html id="63rdc8"
<i class="bi bi-heart-fill fs-1"></i>
```

Other size classes:

* `fs-1`
* `fs-2`
* `fs-3`
* `fs-4`
* `fs-5`
* `fs-6`

---

# 7. Changing Icon Color

Use Bootstrap text color classes.

```html id="tsbipq"
<i class="bi bi-heart-fill text-danger"></i>
```

Examples:

```html id="ebnb4y"
<i class="bi bi-star-fill text-warning"></i>

<i class="bi bi-house-fill text-primary"></i>

<i class="bi bi-tree-fill text-success"></i>

<i class="bi bi-cart-fill text-info"></i>
```

---

# 8. Icons in Buttons

Icons make buttons easier to understand.

```html id="dgu0ji"
<button class="btn btn-primary">

<i class="bi bi-cart-fill"></i>

Buy Now

</button>
```

---

```html id="pww6yh"
<button class="btn btn-success">

<i class="bi bi-download"></i>

Download

</button>
```

---

# 9. Icons in Alerts

```html id="6snm0g"
<div class="alert alert-warning">

<i class="bi bi-exclamation-triangle-fill"></i>

Please submit your assignment today.

</div>
```

---

# 10. Icons in Headings

```html id="r60vrs"
<h1 class="text-primary">

<i class="bi bi-airplane-fill"></i>

Explore Amazing Destinations

</h1>
```

---

# 11. Icons in Cards

```html id="d9d70n"
<div class="card">

<div class="card-body">

<h4>

<i class="bi bi-geo-alt-fill text-danger"></i>

Goa

</h4>

<p>
One of India's most popular tourist destinations.
</p>

</div>

</div>
```

---

# Complete Example

```html id="b0qoy7"
<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<title>Bootstrap Icons Demo</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
rel="stylesheet">

<link
rel="stylesheet"
href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.13.1/font/bootstrap-icons.min.css">

</head>

<body>

<div class="container my-5">

<h1 class="text-center text-primary mb-4">

<i class="bi bi-airplane-fill"></i>

Explore Amazing Destinations

</h1>

<div class="alert alert-warning">

<i class="bi bi-megaphone-fill"></i>

Get 15% OFF on all holiday packages this month!

</div>

<button class="btn btn-primary me-3">

<i class="bi bi-compass-fill"></i>

Explore

</button>

<button class="btn btn-success">

<i class="bi bi-calendar-check"></i>

Book Now

</button>

</div>

</body>

</html>
```

---

# Common Bootstrap Icon Classes

| Icon         | Class                  |
| ------------ | ---------------------- |
| Home         | `bi bi-house-fill`     |
| Person       | `bi bi-person-fill`    |
| Search       | `bi bi-search`         |
| Heart        | `bi bi-heart-fill`     |
| Star         | `bi bi-star-fill`      |
| Cart         | `bi bi-cart-fill`      |
| Airplane     | `bi bi-airplane-fill`  |
| Geo Location | `bi bi-geo-alt-fill`   |
| Telephone    | `bi bi-telephone-fill` |
| Envelope     | `bi bi-envelope-fill`  |
| Download     | `bi bi-download`       |
| Calendar     | `bi bi-calendar-check` |
| Megaphone    | `bi bi-megaphone-fill` |
| Tree         | `bi bi-tree-fill`      |

---

# Summary

| Step | Action                                            |
| ---- | ------------------------------------------------- |
| 1    | Add the Bootstrap Icons CDN                       |
| 2    | Use the `<i>` tag                                 |
| 3    | Specify the icon class (`bi bi-...`)              |
| 4    | Change the size using `fs-*`                      |
| 5    | Change the color using `text-*`                   |
| 6    | Use icons in headings, buttons, cards, and alerts |

---

# Practice Exercise

Create a webpage titled **"My Travel Website"**.

Requirements:

1. Add the Bootstrap Icons CDN.

2. Create a heading:

   **Explore India**

   Add an **airplane icon** before the heading.

3. Create a **success alert** with a **megaphone icon** announcing:

   > 🎉 Special Offer: Flat 20% OFF on all tour packages!

4. Add two buttons:

* **Explore** with a **compass icon**
* **Book Now** with a **calendar-check icon**

5. Create a simple card for **Goa** that includes a **location icon** before the destination name.

---

## Useful Resources

* [Bootstrap Icons Library](https://icons.getbootstrap.com/m) — Browse and search thousands of free Bootstrap Icons.

