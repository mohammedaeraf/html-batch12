# Introduction to HTML & CSS

## What is HTML?

**HTML (HyperText Markup Language)** is the standard language used to create the **structure** of a web page.

HTML is made up of **elements (tags)** such as headings, paragraphs, images, links, tables, and lists.

### Common HTML Tags

| Tag       | Purpose                      |
| --------- | ---------------------------- |
| `<html>`  | Root element of the webpage  |
| `<head>`  | Contains page information    |
| `<title>` | Sets the page title          |
| `<style>` | Contains CSS styles          |
| `<body>`  | Contains the visible content |
| `<h1>`    | Main heading                 |
| `<p>`     | Paragraph                    |

---

## What is CSS?

**CSS (Cascading Style Sheets)** is used to **style** the HTML content.

With CSS, you can change:

* Text color
* Font
* Size
* Alignment
* Background
* Borders
* Spacing

> **HTML creates the structure. CSS makes it attractive.**

---

# Example

```html
<!DOCTYPE html>
<html>

<head>

    <title>My First Web Page</title>

    <style>

        h1{
            color: darkblue;
            text-align: center;
            font-family: Arial, sans-serif;
        }

        p{
            color: #555;
            font-family: Verdana, sans-serif;
            font-size: 18px;
        }

    </style>

</head>

<body>

    <h1>Welcome to Web Design!</h1>

    <p>HTML creates the structure of a webpage.</p>

    <p>CSS is used to style the webpage.</p>

    <p>Learning HTML and CSS is the first step towards becoming a Web Developer.</p>

</body>

</html>
```

---

# Explanation

### HTML

* `<head>` contains information about the webpage.
* `<title>` displays the page title in the browser tab.
* `<body>` contains everything visible on the webpage.
* `<h1>` displays a large heading.
* `<p>` displays paragraphs.

### CSS

```css
h1{
    color: darkblue;
    text-align: center;
}
```

* Changes the heading color to dark blue.
* Centers the heading.

```css
p{
    color: #555;
    font-family: Verdana;
}
```

* Changes the paragraph text color.
* Uses the Verdana font.

---

# HTML vs CSS

| HTML                  | CSS                           |
| --------------------- | ----------------------------- |
| Creates the structure | Styles the webpage            |
| Uses tags             | Uses selectors and properties |
| Adds content          | Changes appearance            |

---

# Real-Life Analogy

Think of building a house:

* **HTML** = Bricks, walls, doors, and windows (the structure)
* **CSS** = Paint, furniture, curtains, and decorations (the appearance)

Without HTML, there is nothing to display.

Without CSS, the webpage works but looks plain.

---

# Summary

* **HTML** is used to create the structure of a webpage.
* **CSS** is used to style and beautify the webpage.
* HTML and CSS work together to create modern websites.
* Learning HTML and CSS is the foundation of web development.
