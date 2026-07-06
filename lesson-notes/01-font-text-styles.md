# CSS Font & Text Styling – Quick Notes

## What is Font & Text Styling?

CSS is used to change the **appearance of text** on a webpage, such as:

* Font family
* Font size
* Font weight
* Font style
* Text color
* Text alignment
* Spacing
* Shadow

---

# Common CSS Properties

| Property          | Purpose                                   |
| ----------------- | ----------------------------------------- |
| `font-family`     | Changes the font                          |
| `font-size`       | Changes text size                         |
| `font-weight`     | Makes text bold or light                  |
| `font-style`      | Makes text italic                         |
| `color`           | Changes text color                        |
| `text-align`      | Aligns text (left, center, right)         |
| `text-decoration` | Adds underline, overline, or line-through |
| `text-shadow`     | Adds a shadow behind text                 |
| `line-height`     | Controls space between lines              |
| `letter-spacing`  | Controls space between letters            |
| `word-spacing`    | Controls space between words              |

---

# Example

```html
<!DOCTYPE html>
<html>
<head>

<style>

body{
    font-family: Verdana, Arial, sans-serif;
    background-color: #f8f9fa;
}

h1{
    color: darkblue;
    text-align: center;
    text-shadow: 2px 2px 4px lightgray;
}

p{
    font-size: 18px;
    font-weight: bold;
    font-style: italic;
    color: #444;
    text-decoration: underline;

    line-height: 30px;
    letter-spacing: 2px;
    word-spacing: 6px;

    background-color: #fff8dc;
    border: 1px solid #999;
    padding: 15px;
    border-radius: 8px;
}

</style>

</head>

<body>

<h1>CSS Font Styling</h1>

<p>
CSS makes webpages attractive by changing the font, color,
alignment, spacing, and other text properties.
</p>

</body>
</html>
```

---

# Explanation

* **font-family** → Changes the font style.
* **font-size** → Changes the size of the text.
* **font-weight** → Makes text bold.
* **font-style** → Makes text italic.
* **color** → Changes the text color.
* **text-align** → Aligns text horizontally.
* **text-decoration** → Adds underline or other decorations.
* **text-shadow** → Adds a shadow behind the text.
* **line-height** → Increases spacing between lines.
* **letter-spacing** → Increases spacing between letters.
* **word-spacing** → Increases spacing between words.

---

# Best Practices

* Use readable fonts such as **Arial**, **Verdana**, or **Tahoma**.
* Use dark text on a light background for better readability.
* Avoid excessive spacing and text shadows.
* Use bold and italic only when necessary.
* Keep font sizes consistent throughout the webpage.

---

# Summary

* CSS provides many properties to style text.
* Font properties improve readability.
* Text properties improve appearance and layout.
* Well-formatted text makes webpages more attractive and professional.
