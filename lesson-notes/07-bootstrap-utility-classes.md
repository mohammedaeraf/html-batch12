# Bootstrap Utility Classes – Part 2

## Learning Objectives

By the end of this lesson, you will be able to:

- Add borders to elements.
- Create rounded corners.
- Apply shadows.
- Use Bootstrap display headings.
- Control element width.
- Add borders with different colors.

---

# Bootstrap Example

```html
<!DOCTYPE html>
<html>
  <head>
    <link
      rel="stylesheet"
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/css/bootstrap.min.css"
    />
  </head>

  <body class="bg-light">
    <div class="container mt-5">
      <h1 class="display-3 text-primary text-center">Bootstrap Utilities</h1>

      <div class="border border-primary rounded shadow p-4 mt-4 bg-white">
        <h3 class="text-success">Welcome!</h3>

        <p class="fs-5">
          Bootstrap provides many ready-made utility classes that help create
          beautiful webpages without writing CSS.
        </p>
      </div>
    </div>
  </body>
</html>
```

---

# Display Headings

Bootstrap provides large heading classes.

| Class       | Size         |
| ----------- | ------------ |
| `display-1` | Largest      |
| `display-2` | Very Large   |
| `display-3` | Large        |
| `display-4` | Medium Large |
| `display-5` | Medium       |
| `display-6` | Smallest     |

### Example

```html
<h1 class="display-1">Display 1</h1>

<h1 class="display-3">Display 3</h1>

<h1 class="display-6">Display 6</h1>
```

---

# Border Classes

Add borders without writing CSS.

| Class      | Purpose         |
| ---------- | --------------- |
| `border`   | Adds a border   |
| `border-0` | Removes border  |
| `border-1` | Thin border     |
| `border-2` | Medium border   |
| `border-3` | Thick border    |
| `border-4` | Thicker border  |
| `border-5` | Thickest border |

### Example

```html
<div class="border p-3">Border Example</div>
```

---

# Border Colors

| Class            | Color  |
| ---------------- | ------ |
| `border-primary` | Blue   |
| `border-success` | Green  |
| `border-danger`  | Red    |
| `border-warning` | Yellow |
| `border-info`    | Cyan   |
| `border-dark`    | Black  |

### Example

```html
<div class="border border-danger p-3">Red Border</div>
```

---

# Rounded Corners

| Class            | Purpose                             |
| ---------------- | ----------------------------------- |
| `rounded`        | Rounded corners                     |
| `rounded-1`      | Small radius                        |
| `rounded-2`      | Medium radius                       |
| `rounded-3`      | Large radius                        |
| `rounded-4`      | Larger radius                       |
| `rounded-5`      | Largest radius                      |
| `rounded-circle` | Circle (for square elements/images) |
| `rounded-pill`   | Pill shape                          |

### Example

```html
<div class="border rounded p-3">Rounded Box</div>

<button class="btn btn-primary rounded-pill">Login</button>
```

---

# Shadow Classes

Add shadows easily.

| Class         | Purpose       |
| ------------- | ------------- |
| `shadow-none` | No shadow     |
| `shadow-sm`   | Small shadow  |
| `shadow`      | Medium shadow |
| `shadow-lg`   | Large shadow  |

### Example

```html
<div class="shadow p-4 bg-white">Shadow Example</div>
```

---

# Width Classes

| Class   | Width |
| ------- | ----- |
| `w-25`  | 25%   |
| `w-50`  | 50%   |
| `w-75`  | 75%   |
| `w-100` | 100%  |

### Example

```html
<div class="w-50 bg-info text-white p-3">50% Width</div>
```

---

# Complete Example

```html
<div class="container mt-5">
  <h1 class="display-4 text-center text-primary">Student Profile</h1>

  <div
    class="w-75 mx-auto border border-success border-3 rounded-4 shadow-lg p-4 bg-white mt-4"
  >
    <h3 class="text-success">Mohammed Ali</h3>

    <p class="fs-5">Course : Web Design</p>

    <p>Learning Bootstrap is simple and enjoyable.</p>

    <button class="btn btn-primary rounded-pill">View Profile</button>
  </div>
</div>
```

---

# Common Bootstrap Utility Classes

| Category        | Examples                        |
| --------------- | ------------------------------- |
| Text Color      | `text-primary`, `text-danger`   |
| Background      | `bg-light`, `bg-warning`        |
| Font Size       | `fs-1` to `fs-6`                |
| Font Weight     | `fw-bold`, `fw-light`           |
| Alignment       | `text-center`, `text-end`       |
| Padding         | `p-1` to `p-5`                  |
| Margin          | `m-1` to `m-5`                  |
| Border          | `border`, `border-3`            |
| Border Color    | `border-success`                |
| Rounded         | `rounded`, `rounded-pill`       |
| Shadow          | `shadow`, `shadow-lg`           |
| Width           | `w-25`, `w-50`, `w-75`, `w-100` |
| Display Heading | `display-1` to `display-6`      |

---

# Best Practices

- Combine multiple Bootstrap utility classes to style elements.
- Use `shadow` and `rounded` to create attractive cards.
- Use `display-*` for page titles.
- Prefer Bootstrap utilities over custom CSS for simple styling.
- Keep spacing consistent using margin and padding classes.

---

# Summary

- Bootstrap provides many ready-made utility classes.
- Use **`display-*`** for large headings.
- Use **`border`** and **`border-*`** classes to style borders.
- Use **`rounded-*`** classes to create rounded corners.
- Use **`shadow-*`** classes to add depth.
- Use **`w-*`** classes to control width.
- Combining utility classes allows you to build professional-looking webpages quickly without writing custom CSS.

### Suggested Classroom Activity (15–20 mins)

Ask students to create a **"Course Information Card"** using only Bootstrap classes (no custom CSS).

Requirements:

- `container`
- `display-4` heading
- `border border-primary border-3`
- `rounded-4`
- `shadow-lg`
- `bg-light`
- `p-4`
- `w-75 mx-auto`
- `text-center`
- `fw-bold`
- `btn btn-success rounded-pill`

This reinforces all the Bootstrap utility classes learned across both lessons.
