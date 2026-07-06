# HTML Lists – Quick Notes

## What is a List?

A **list** is used to display related items in an organized way.

**Examples:**

* Shopping List
* Course Topics
* Steps to Complete a Task
* Website Navigation Menu

---

# Types of HTML Lists

There are **three types of lists**:

1. Unordered List (`<ul>`)
2. Ordered List (`<ol>`)
3. Description List (`<dl>`)

---

# 1. Unordered List

An **unordered list** displays items with **bullets**.

### Syntax

```html id="btxcwt"
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### Output

* HTML
* CSS
* JavaScript

---

# 2. Ordered List

An **ordered list** displays items with **numbers or letters**.

### Syntax

```html id="ry03zw"
<ol>
    <li>Wake up</li>
    <li>Study HTML</li>
    <li>Complete Assignment</li>
</ol>
```

### Output

1. Wake up
2. Study HTML
3. Complete Assignment

---

# Ordered List Types

| Type | Example    |
| ---- | ---------- |
| `1`  | 1, 2, 3    |
| `A`  | A, B, C    |
| `a`  | a, b, c    |
| `I`  | I, II, III |
| `i`  | i, ii, iii |

### Example

```html id="b8gw7h"
<ol type="A">
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

---

# 3. Description List

A **description list** is used for terms and their descriptions.

### Syntax

```html id="h2lnm6"
<dl>
    <dt>HTML</dt>
    <dd>Creates the structure of a webpage.</dd>

    <dt>CSS</dt>
    <dd>Styles the webpage.</dd>
</dl>
```

---

# Nested Lists

A list can contain another list.

```html id="8r8clv"
<ul>
    <li>Frontend
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
    </li>

    <li>Backend</li>
</ul>
```

---

# Styling Lists with CSS

```css id="xw0lb7"
ul{
    list-style-type: square;
}

ol{
    color: darkblue;
}

li{
    padding: 5px;
}
```

---

# Common `list-style-type` Values

### Unordered Lists

* `disc` (default)
* `circle`
* `square`
* `none`

```css id="1rjlwm"
ul{
    list-style-type: square;
}
```

### Ordered Lists

```css id="s57tsh"
ol{
    list-style-type: upper-roman;
}
```

Possible values:

* decimal
* upper-alpha
* lower-alpha
* upper-roman
* lower-roman

---

# Best Practices

* Use **`<ul>`** when the order of items does not matter.
* Use **`<ol>`** when the order is important.
* Use **`<dl>`** for terms and definitions.
* Keep list items short and meaningful.
* Use CSS to customize the appearance of lists.

---

# Summary

* HTML provides **three types of lists**.
* `<ul>` creates a bulleted list.
* `<ol>` creates a numbered or lettered list.
* `<li>` represents a list item.
* CSS can change bullet styles, numbering styles, spacing, and colors.
