# Lesson Notes – HTML Semantic Elements

## Learning Objectives

By the end of this lesson, you will be able to:

- Understand what semantic elements are.
- Identify the most commonly used HTML semantic elements.
- Build a well-structured webpage using semantic tags.
- Understand the advantages of semantic HTML.

---

# 1. What are Semantic Elements?

A **semantic element** clearly describes its purpose to both the **browser** and the **developer**.

For example:

- `<header>` represents the header of a webpage.
- `<nav>` represents the navigation menu.
- `<footer>` represents the footer.

Unlike `<div>`, semantic elements tell us **what the content is**, not just how it is grouped.

---

# 2. Why Use Semantic Elements?

Semantic elements help to:

- Improve code readability.
- Organize webpage content.
- Improve Search Engine Optimization (SEO).
- Make webpages more accessible.
- Help developers understand the page structure.

---

# 3. Common Semantic Elements

| Element     | Purpose                                                                |
| ----------- | ---------------------------------------------------------------------- |
| `<header>`  | Displays the webpage or section header                                 |
| `<nav>`     | Contains navigation links                                              |
| `<main>`    | Contains the main content of the webpage                               |
| `<section>` | Groups related content                                                 |
| `<article>` | Represents independent content such as a blog, news article, or course |
| `<aside>`   | Displays related information, announcements, or advertisements         |
| `<footer>`  | Displays footer information such as copyright or contact details       |

---

# 4. Webpage Structure

A typical webpage using semantic elements looks like this:

```text id="b1xkws"
<header>

<nav>

<main>

    <section>

        <article>

        </article>

    </section>

    <aside>

    </aside>

</main>

<footer>
```

---

# 5. The `<header>` Element

The `<header>` element contains the introductory content of a webpage.

Example:

```html id="cztxzy"
<header>
  <h1>Future Leaders Academy</h1>

  <p>Learn • Build • Succeed</p>
</header>
```

Typical contents:

- Website title
- Logo
- Tagline

---

# 6. The `<nav>` Element

The `<nav>` element contains the website navigation.

Example:

```html id="djqv6d"
<nav>
  <a href="#">Home</a>

  <a href="#">Courses</a>

  <a href="#">About</a>

  <a href="#">Contact</a>
</nav>
```

Users click these links to navigate between pages or sections.

---

# 7. The `<main>` Element

The `<main>` element contains the primary content of the webpage.

Example:

```html id="r53czq"
<main>Website Content</main>
```

Every webpage should normally have only **one** `<main>` element.

---

# 8. The `<section>` Element

A `<section>` groups related content together.

Example:

```html id="ub0aj4"
<section>
  <h2>Popular Courses</h2>
</section>
```

Examples of sections:

- About Us
- Services
- Courses
- Contact
- Gallery

---

# 9. The `<article>` Element

An `<article>` represents independent content.

Example:

```html id="4myu8e"
<article>
  <h3>Python Programming</h3>

  <p>Learn Python from beginner to advanced level.</p>
</article>
```

Examples:

- Blog post
- News article
- Product card
- Course card

---

# 10. The `<aside>` Element

The `<aside>` element contains related information.

Example:

```html id="jlwmja"
<aside>Admissions Open!</aside>
```

Examples:

- Announcements
- Advertisements
- Upcoming Events
- Tips
- Related Links

---

# 11. The `<footer>` Element

The `<footer>` displays information at the bottom of the webpage.

Example:

```html id="gk3s9k"
<footer>© 2026 Future Leaders Academy</footer>
```

Typical contents:

- Copyright
- Contact Information
- Social Media Links
- Privacy Policy

---

# 12. Complete Example

```html id="39s22x"
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>Semantic Elements</title>

    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
  </head>

  <body>
    <header class="bg-primary text-white text-center p-4">
      <h1>Future Leaders Academy</h1>

      <p>Learn • Build • Succeed</p>
    </header>

    <nav class="bg-dark text-center p-3">
      <a href="#" class="btn btn-outline-light me-2">Home</a>

      <a href="#" class="btn btn-outline-light me-2">Courses</a>

      <a href="#" class="btn btn-outline-light me-2">About</a>

      <a href="#" class="btn btn-outline-light">Contact</a>
    </nav>

    <main class="container my-5">
      <section>
        <h2 class="text-primary mb-4">Popular Courses</h2>

        <div class="row g-4">
          <article class="col-md-4">
            <div class="card shadow">
              <div class="card-body">
                <h4>HTML & CSS</h4>

                <p>Learn modern web design using HTML and CSS.</p>
              </div>
            </div>
          </article>

          <article class="col-md-4">
            <div class="card shadow">
              <div class="card-body">
                <h4>Python</h4>

                <p>Learn Python programming with practical examples.</p>
              </div>
            </div>
          </article>

          <article class="col-md-4">
            <div class="card shadow">
              <div class="card-body">
                <h4>AWS Fundamentals</h4>

                <p>Understand cloud computing using AWS.</p>
              </div>
            </div>
          </article>
        </div>
      </section>

      <aside class="alert alert-info mt-5">
        <h4>Upcoming Batch</h4>

        <p>Admissions are now open for the next Web Design batch.</p>
      </aside>
    </main>

    <footer class="bg-dark text-white text-center p-4">
      <p>© 2026 Future Leaders Academy. All Rights Reserved.</p>
    </footer>
  </body>
</html>
```

---

# Semantic Elements Used in This Example

| Semantic Element | Used For                    |
| ---------------- | --------------------------- |
| `<header>`       | Academy title and tagline   |
| `<nav>`          | Navigation buttons          |
| `<main>`         | Main webpage content        |
| `<section>`      | Popular Courses section     |
| `<article>`      | Individual course cards     |
| `<aside>`        | Upcoming batch announcement |
| `<footer>`       | Copyright information       |

---

# Summary

| Element     | Purpose                |
| ----------- | ---------------------- |
| `<header>`  | Header of the webpage  |
| `<nav>`     | Navigation menu        |
| `<main>`    | Main webpage content   |
| `<section>` | Groups related content |
| `<article>` | Independent content    |
| `<aside>`   | Related information    |
| `<footer>`  | Footer information     |

---

# Practice Exercise

Create a webpage titled **"My Learning Portal"** using HTML Semantic Elements.

Requirements:

1. Create a **`<header>`** with the website title and a short tagline.

2. Create a **`<nav>`** containing four navigation buttons:
   - Home
   - Courses
   - About
   - Contact

3. Create a **`<main>`** section.

4. Inside `<main>`, create a **`<section>`** titled **Popular Courses**.

5. Add **three `<article>` elements**, each containing:
   - Course Name
   - Short Description
   - Bootstrap Card

6. Add an **`<aside>`** displaying:

> Admissions Open for New Batches!

7. Add a **`<footer>`** containing a copyright message.

Use Bootstrap classes to make the webpage attractive and responsive.

---

## Learning Outcome

By completing this exercise, you will learn how to organize a webpage using HTML semantic elements while reinforcing your knowledge of Bootstrap Containers, Grid Layout, Cards, Buttons, and Utility Classes to create a clean, accessible, and well-structured website.
