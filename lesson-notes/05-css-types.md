# Lesson Notes – Types of CSS

## What is CSS?

**CSS (Cascading Style Sheets)** is used to style and design web pages. It controls the appearance of HTML elements, such as:

* Text color
* Background color
* Font style and size
* Borders
* Spacing
* Alignment
* Layout

**HTML** creates the structure of a webpage, while **CSS** makes it attractive.

---

# Types of CSS

There are **three types of CSS**:

1. Inline CSS
2. Internal CSS
3. External CSS

---

# 1. Inline CSS

### Definition

Inline CSS is written directly inside an HTML element using the **style** attribute.

### Syntax

```html
<tag style="property: value;">
```

### Example

```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color: blue;">Welcome to CSS</h1>

<p style="color: red;">This is a paragraph.</p>

</body>
</html>
```

### Advantages

* Easy to use
* Good for testing small changes
* Styles only one element

### Disadvantages

* Difficult to maintain
* Repeats the same code
* Not suitable for large websites

---

# 2. Internal CSS

### Definition

Internal CSS is written inside the `<style>` tag, usually within the `<head>` section of an HTML document.

### Example

```html
<!DOCTYPE html>
<html>

<head>

<style>

h1{
    color: blue;
}

p{
    color: red;
}

button{
    background-color: green;
    color: white;
}

</style>

</head>

<body>

<h1>Learning CSS</h1>

<p>Internal CSS Example</p>

<button>Submit</button>

</body>
</html>
```

### Advantages

* Keeps HTML cleaner
* One style can be applied to multiple elements
* Good for single-page websites

### Disadvantages

* Cannot be shared across multiple web pages
* Repetition if many pages use the same styles

---

# 3. External CSS

### Definition

External CSS stores all styles in a separate **.css** file. The HTML page links to this file.

### HTML File (index.html)

```html
<!DOCTYPE html>
<html>

<head>
    <link rel="stylesheet" href="style.css">
</head>

<body>

<h1>Future Leaders Academy</h1>

<p>Learning External CSS</p>

<button>Enroll Now</button>

</body>
</html>
```

### CSS File (style.css)

```css
body{
    background-color: #f5f5f5;
    font-family: Arial;
}

h1{
    color: darkblue;
}

p{
    color: #555;
}

button{
    background-color: green;
    color: white;
    padding: 10px 20px;
}
```

### Advantages

* Best for professional websites
* Reusable across multiple pages
* Easy to maintain
* Keeps HTML clean and organized

### Disadvantages

* Requires an additional CSS file

---

# Comparison of CSS Types

| Feature          | Inline CSS          | Internal CSS         | External CSS         |
| ---------------- | ------------------- | -------------------- | -------------------- |
| Location         | Inside HTML element | Inside `<style>` tag | Separate `.css` file |
| Reusable         | No                  | Limited              | Yes                  |
| Easy to Maintain | No                  | Moderate             | Yes                  |
| Best For         | Quick styling       | Single-page websites | Multi-page websites  |

---

# CSS Priority

If the same style is defined in all three places, the browser follows this priority:

1. Inline CSS (Highest)
2. Internal CSS
3. External CSS (Lowest)

Example:

```css
/* style.css */
h1{
    color: green;
}
```

```html
<style>
h1{
    color: blue;
}
</style>

<h1 style="color:red;">Hello CSS</h1>
```

**Output:** The heading appears **red** because Inline CSS has the highest priority.

---

# Best Practices

* Use **Inline CSS** only for quick testing or small changes.
* Use **Internal CSS** for small, single-page websites.
* Use **External CSS** for professional websites because it is reusable and easier to maintain.

---

# Key Terms

* **CSS** – Cascading Style Sheets
* **Selector** – Specifies which HTML element to style (e.g., `h1`, `p`)
* **Property** – The style to change (e.g., `color`)
* **Value** – The setting for the property (e.g., `blue`)

Example:

```css
h1{
    color: blue;
}
```

* `h1` → Selector
* `color` → Property
* `blue` → Value

---

# Summary

* CSS styles the appearance of web pages.
* There are three types of CSS: Inline, Internal, and External.
* External CSS is the preferred method for building professional websites.
* CSS helps create consistent, attractive, and easy-to-maintain web pages.
