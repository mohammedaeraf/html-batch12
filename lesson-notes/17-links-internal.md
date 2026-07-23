# Lesson Notes – Internal Links in HTML

## Learning Objectives

By the end of this lesson, you will be able to:

* Understand what internal links are.
* Create links that navigate to different sections of the same webpage.
* Use the `id` attribute to identify page sections.
* Use Bootstrap classes to create an attractive navigation menu.

---

# 1. What are Internal Links?

An **internal link** is a hyperlink that takes the user to another section **within the same webpage**.

Internal links are commonly used in:

* Navigation menus
* One-page websites
* Landing pages
* FAQ pages
* Documentation websites
* "Back to Top" links

---

# 2. How Do Internal Links Work?

Internal links use the following two elements:

### Step 1 – Create an `id`

Assign a unique `id` to the section you want to navigate to.

```html
<div id="about">

    <h2>About</h2>

</div>
```

---

### Step 2 – Create a Link

Use the `href` attribute with the `#` symbol followed by the `id`.

```html
<a href="#about">
    About
</a>
```

When the user clicks the link, the browser automatically scrolls to the section whose `id` matches the value after `#`.

---

# 3. Bootstrap Navigation Menu

Create a simple navigation menu using Bootstrap buttons.

```html
<div class="text-center mb-5">

    <a href="#home" class="btn btn-primary me-2">
        Home
    </a>

    <a href="#about" class="btn btn-success me-2">
        About
    </a>

    <a href="#services" class="btn btn-warning me-2">
        Services
    </a>

    <a href="#contact" class="btn btn-danger">
        Contact
    </a>

</div>
```

---

# 4. Creating Page Sections

Each section should have a unique `id`.

Example:

```html
<div id="home" class="p-4 mb-5 bg-primary-subtle rounded shadow">

    <h2 class="text-primary">
        Home
    </h2>

    <p>
        Welcome to our website.
    </p>

</div>
```

Similarly, create sections for:

* About
* Services
* Contact

---

# 5. Back to Top Link

A common use of internal links is a **Back to Top** button.

```html
<a href="#home" class="btn btn-dark">
    ↑ Back to Top
</a>
```

When clicked, the page scrolls back to the **Home** section.

---

# 6. Complete Example

```html
<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<title>Bootstrap Internal Links</title>

<link
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
rel="stylesheet">

</head>

<body>

<div class="container my-5">

<h1 class="text-center text-primary display-4 fw-bold mb-5">
My Website
</h1>

<div class="text-center mb-5">

<a href="#home" class="btn btn-primary me-2">Home</a>

<a href="#about" class="btn btn-success me-2">About</a>

<a href="#services" class="btn btn-warning me-2">Services</a>

<a href="#contact" class="btn btn-danger">Contact</a>

</div>

<div id="home" class="p-4 mb-5 bg-primary-subtle rounded shadow">

<h2 class="text-primary">Home</h2>

<p>
Welcome to our website.
</p>

</div>

<div id="about" class="p-4 mb-5 bg-success-subtle rounded shadow">

<h2 class="text-success">About</h2>

<p>
We provide professional IT training.
</p>

</div>

<div id="services" class="p-4 mb-5 bg-warning-subtle rounded shadow">

<h2 class="text-warning">Services</h2>

<p>
Web Design, Python, React and AWS courses.
</p>

</div>

<div id="contact" class="p-4 mb-5 bg-danger-subtle rounded shadow">

<h2 class="text-danger">Contact</h2>

<p>
Email: info@example.com
</p>

</div>

<div class="text-center">

<a href="#home" class="btn btn-dark">
↑ Back to Top
</a>

</div>

</div>

</body>

</html>
```

---

# Bootstrap Classes Used

| Class                                                                             | Purpose                         |
| --------------------------------------------------------------------------------- | ------------------------------- |
| `container`                                                                       | Centers and aligns page content |
| `btn`                                                                             | Creates a Bootstrap button      |
| `btn-primary`, `btn-success`, `btn-warning`, `btn-danger`, `btn-dark`             | Button colors                   |
| `display-4`                                                                       | Large heading                   |
| `fw-bold`                                                                         | Bold text                       |
| `text-center`                                                                     | Center-aligns text              |
| `text-primary`, `text-success`, `text-warning`, `text-danger`                     | Text colors                     |
| `bg-primary-subtle`, `bg-success-subtle`, `bg-warning-subtle`, `bg-danger-subtle` | Light background colors         |
| `p-4`                                                                             | Adds padding                    |
| `mb-5`, `my-5`, `me-2`                                                            | Adds spacing                    |
| `rounded`                                                                         | Rounds the corners              |
| `shadow`                                                                          | Adds a shadow effect            |

---

# Summary

* Internal links navigate to another section of the **same webpage**.
* The destination section must have a unique `id`.
* The link uses `href="#id"` to point to that section.
* Bootstrap buttons can be used to create attractive navigation links.
* Internal links improve navigation on long webpages.

---

# Practice Exercise

Create a webpage titled **"My Personal Website"**.

Requirements:

1. Create a Bootstrap navigation menu with the following buttons:

   * Home
   * About Me
   * Skills
   * Contact

2. Create four sections with matching `id` attributes.

3. Apply Bootstrap classes to each section:

   * Different subtle background color
   * Padding (`p-4`)
   * Rounded corners (`rounded`)
   * Shadow (`shadow`)
   * Bottom margin (`mb-5`)

4. Add a **Back to Top** button at the bottom of the page that links to the **Home** section.

### Learning Outcome

By completing this exercise, you will understand how to create internal links using the `id` attribute and `href="#id"` while building a clean, Bootstrap-styled single-page website.
