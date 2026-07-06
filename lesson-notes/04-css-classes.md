# CSS Classes – Quick Notes

## What is a CSS Class?

A **CSS class** is a reusable style that can be applied to one or more HTML elements.

Instead of writing the same CSS repeatedly, define it once as a class and reuse it wherever needed.

---

# Defining a Class

A CSS class starts with a **dot (`.`)**.

### Syntax

```css id="o8mjlwm"
.class-name{
    property: value;
}
```

### Example

```css id="dlyovq"
.text-red{
    color: red;
}

.text-bold{
    font-weight: bold;
}
```

---

# Using a Class

Use the **`class`** attribute to apply a class to an HTML element.

```html id="khz0l7"
<p class="text-red">
    This text is red.
</p>
```

---

# Applying Multiple Classes

You can apply **more than one class** to the same element by separating the class names with spaces.

```html id="dgg86l"
<h1 class="text-blue align-center">
    Welcome to CSS
</h1>

<p class="text-red text-bold">
    Learning CSS Classes is easy.
</p>
```

---

# Example

```html id="hjm7n6"
<!DOCTYPE html>
<html>

<head>

<style>

.text-blue{
    color: royalblue;
}

.text-red{
    color: crimson;
}

.text-bold{
    font-weight: bold;
}

.text-center{
    text-align: center;
}

.highlight{
    background-color: #fff3cd;
    border: 1px solid orange;
    padding: 12px;
    border-radius: 6px;
}

</style>

</head>

<body>

<h1 class="text-blue text-center">
    CSS Classes Demo
</h1>

<p class="text-red text-bold highlight">
    CSS classes allow you to reuse the same styles on multiple elements.
</p>

</body>

</html>
```

---

# Common CSS Classes

```css id="m5uxvx"
.text-red{
    color: red;
}

.text-blue{
    color: blue;
}

.text-center{
    text-align: center;
}

.text-bold{
    font-weight: bold;
}

.text-italic{
    font-style: italic;
}

.box{
    border: 1px solid gray;
    padding: 10px;
    border-radius: 5px;
}
```

---

# Why Use CSS Classes?

* Reuse the same styles many times.
* Keep HTML clean and readable.
* Reduce duplicate CSS code.
* Make webpages easier to maintain.
* Professional websites rely heavily on CSS classes.

---

# Best Practices

* Use meaningful class names such as `.title`, `.button`, or `.highlight`.
* Apply multiple classes when needed instead of creating many similar classes.
* Keep class names short and descriptive.
* Use lowercase letters and hyphens (`-`) in class names.

---

# Summary

* A **CSS class** is a reusable style.
* Classes are defined using a **dot (`.`)**.
* Apply a class using the **`class`** attribute.
* Multiple classes can be applied to the same HTML element.
* CSS classes make web pages cleaner, reusable, and easier to maintain.
