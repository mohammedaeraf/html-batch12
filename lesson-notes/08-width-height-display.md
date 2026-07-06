# CSS Width, Height & Display – Quick Notes

## CSS Size Properties

CSS provides properties to control the **size of elements** on a webpage.

The most commonly used properties are:

- `width`
- `height`
- `min-height`
- `max-width`

---

# 1. Width

The **`width`** property sets the width of an element.

### Example

```css
.box {
  width: 300px;
}
```

```html
<div class="box">Width: 300px</div>
```

---

# 2. Height

The **`height`** property sets the height of an element.

### Example

```css
.box {
  height: 150px;
}
```

```html
<div class="box">Height: 150px</div>
```

---

# 3. max-width

The **`max-width`** property sets the **maximum width** an element can have.

It is commonly used to make webpages responsive.

### Example

```css
.box {
  width: 100%;
  max-width: 500px;
}
```

The box will:

- Expand up to **500px**
- Become smaller on smaller screens

---

# 4. min-height

The **`min-height`** property sets the **minimum height** of an element.

Even if there is very little content, the element will not become shorter than the specified height.

### Example

```css
.box {
  min-height: 200px;
}
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      .box {
        width: 80%;
        max-width: 500px;
        min-height: 180px;

        border: 2px solid royalblue;
        background-color: aliceblue;
        padding: 20px;
        margin: 20px auto;
      }
    </style>
  </head>

  <body>
    <div class="box">
      This box has a width of 80%, a maximum width of 500px, and a minimum
      height of 180px.
    </div>
  </body>
</html>
```

---

# Display Property

The **`display`** property controls how an HTML element appears on the webpage.

Common values:

- `block`
- `inline`
- `inline-block`

---

# 1. Block Elements

A **block element**:

- Starts on a new line.
- Takes the full available width.
- Width and height can be changed.

Examples:

- `<div>`
- `<p>`
- `<h1>`
- `<section>`

### Example

```html
<div style="background:lightblue;">First Box</div>

<div style="background:lightgreen;">Second Box</div>
```

Output:

```text
First Box
Second Box
```

---

# 2. Inline Elements

An **inline element**:

- Does **not** start on a new line.
- Takes only the required width.
- `width` and `height` generally have no effect.

Examples:

- `<span>`
- `<a>`
- `<strong>`
- `<em>`

### Example

```html
<span style="background:pink;">HTML</span>
<span style="background:lightgreen;">CSS</span>
<span style="background:lightblue;">Bootstrap</span>
```

Output:

```text
HTML CSS Bootstrap
```

(All appear on the same line.)

---

# 3. Inline-Block Elements

An **inline-block element**:

- Appears on the same line as other elements.
- Allows you to set `width` and `height`.

### Example

```html
<span
  style="
display:inline-block;
width:120px;
height:60px;
background:orange;
text-align:center;"
>
  Box 1
</span>

<span
  style="
display:inline-block;
width:120px;
height:60px;
background:skyblue;
text-align:center;"
>
  Box 2
</span>
```

The boxes stay on the same line while allowing custom width and height.

---

# Comparison

| Property             | Block | Inline | Inline-Block |
| -------------------- | ----- | ------ | ------------ |
| Starts on a new line | ✔     | ✖      | ✖            |
| Takes full width     | ✔     | ✖      | ✖            |
| Width can be set     | ✔     | ✖      | ✔            |
| Height can be set    | ✔     | ✖      | ✔            |

---

# Best Practices

- Use **block** elements for sections and containers.
- Use **inline** elements for small pieces of text.
- Use **inline-block** when elements should appear on the same line but still need a fixed width and height.
- Prefer **`max-width`** over a fixed `width` for responsive webpages.
- Use **`min-height`** to maintain a consistent layout.

---

# Summary

- **`width`** sets the width of an element.
- **`height`** sets the height of an element.
- **`max-width`** limits the maximum width.
- **`min-height`** sets the minimum height.
- **`block`** elements start on a new line and occupy the full width.
- **`inline`** elements stay on the same line and only take the required space.
- **`inline-block`** combines the advantages of both by staying on the same line while allowing custom width and height.
