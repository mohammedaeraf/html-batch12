# Lesson Notes – Google Fonts

## Learning Objectives

By the end of this lesson, you will be able to:

- Understand what Google Fonts are.
- Add Google Fonts to a webpage.
- Apply a Google Font using CSS.
- Improve the appearance of your website with modern typography.

---

# 1. What are Google Fonts?

**Google Fonts** is a free library of high-quality fonts provided by Google.

It allows you to use beautiful fonts in your websites without installing them on your computer.

Some popular Google Fonts include:

- Poppins
- Roboto
- Open Sans
- Montserrat
- Lato
- Nunito

---

# 2. Why Use Google Fonts?

Google Fonts make your website look:

- ✅ Modern
- ✅ Professional
- ✅ Attractive
- ✅ Easy to read

---

# 3. Step 1 – Visit Google Fonts

Open the following website:

**[https://fonts.google.com](https://fonts.google.com)**

Search for your preferred font.

Example:

**Poppins**

---

# 4. Step 2 – Copy the Font Link

After selecting a font, Google provides a `<link>` tag.

Example:

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />

<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />

<link
  href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
  rel="stylesheet"
/>
```

Paste these lines inside the `<head>` section of your HTML document.

---

# 5. Step 3 – Apply the Font

Use the `font-family` property in CSS.

```css
body {
  font-family: "Poppins", sans-serif;
}
```

Now the entire webpage will use the **Poppins** font.

---

# 6. Complete Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>Google Fonts Demo</title>

    <link rel="preconnect" href="https://fonts.googleapis.com" />

    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />

    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
      rel="stylesheet"
    />

    <style>
      body {
        font-family: "Poppins", sans-serif;
      }
    </style>
  </head>

  <body>
    <h1>Welcome to Google Fonts</h1>

    <p>This webpage uses the Poppins font from Google Fonts.</p>
  </body>
</html>
```

---

# 7. Applying Fonts to Specific Elements

Instead of the entire webpage, you can apply the font to selected elements.

```css
h1 {
  font-family: "Poppins", sans-serif;
}

p {
  font-family: "Roboto", sans-serif;
}
```

---

# 8. Popular Google Fonts

| Font       | Best Used For        |
| ---------- | -------------------- |
| Poppins    | Modern websites      |
| Roboto     | Business websites    |
| Open Sans  | Blogs and articles   |
| Montserrat | Headings             |
| Lato       | Corporate websites   |
| Nunito     | Educational websites |

---

# Summary

| Step | Action                             |
| ---- | ---------------------------------- |
| 1    | Visit **fonts.google.com**         |
| 2    | Select a font                      |
| 3    | Copy the `<link>` tag              |
| 4    | Paste it inside `<head>`           |
| 5    | Apply the font using `font-family` |

---

# Practice Exercise

Create a simple webpage titled **"My Favourite Font"**.

Requirements:

1. Add the **Poppins** font from Google Fonts.

2. Create a heading:

   **Welcome to My Website**

3. Add a short paragraph about yourself.

4. Apply the **Poppins** font to the entire webpage.

5. Add a light background color and center-align the heading.

**Expected Result:**

- The webpage should display the **Poppins** font.
- The heading should be centered.
- The text should appear clean, modern, and easy to read.
