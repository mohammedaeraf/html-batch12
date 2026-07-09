# Lesson Notes – Bootstrap Images

## Objective

In this lesson, you will learn how to:

- Add images to a webpage.
- Make images responsive using Bootstrap.
- Apply borders, rounded corners, and shadows.
- Create attractive image sections.

---

# 1. Adding an Image

Use the `<img>` tag to display an image.

### Syntax

```html
<img src="image.jpg" alt="Description" />
```

### Example

```html
<img src="goa.jpg" alt="Goa Beach" />
```

### Attributes

| Attribute | Description                                              |
| --------- | -------------------------------------------------------- |
| `src`     | Specifies the image path or URL.                         |
| `alt`     | Displays alternative text if the image cannot be loaded. |

---

# 2. Responsive Images

Bootstrap provides the `img-fluid` class to make images responsive.

### Syntax

```html
<img src="image.jpg" class="img-fluid" alt="Image" />
```

### Example

```html
<img src="goa.jpg" class="img-fluid" alt="Goa Beach" />
```

### What it does

- Automatically adjusts image width.
- Prevents image overflow.
- Maintains aspect ratio.

---

# 3. Rounded Corners

Use Bootstrap rounded classes.

### Rounded

```html
<img src="goa.jpg" class="img-fluid rounded" />
```

### Larger Rounded Corners

```html
<img src="goa.jpg" class="img-fluid rounded-4" />
```

### Fully Circular Image

```html
<img src="person.jpg" class="img-fluid rounded-circle" />
```

---

# 4. Image Thumbnail

Adds a border and padding around the image.

```html
<img src="goa.jpg" class="img-thumbnail" />
```

---

# 5. Adding Borders

### Basic Border

```html
<img src="goa.jpg" class="img-fluid border" />
```

---

### Colored Border

```html
<img src="goa.jpg" class="img-fluid border border-primary" />
```

---

### Thick Border

```html
<img src="goa.jpg" class="img-fluid border border-3 border-success" />
```

---

# 6. Adding Shadows

### Medium Shadow

```html
<img src="goa.jpg" class="img-fluid shadow" />
```

---

### Large Shadow

```html
<img src="goa.jpg" class="img-fluid shadow-lg" />
```

---

# 7. Combining Multiple Classes

Bootstrap classes can be combined.

Example:

```html
<img
  src="goa.jpg"
  class="img-fluid rounded border border-3 border-info shadow-lg"
/>
```

This image will have:

- Responsive width
- Rounded corners
- Thick blue border
- Large shadow

---

# 8. Local Image

Store the image inside your project folder.

```
Project
│
├── index.html
│
└── images
      ├── goa.jpg
      └── munnar.jpg
```

Use

```html
<img src="images/goa.jpg" class="img-fluid" alt="Goa" />
```

---

# 9. Online Image

You can also use an image URL.

```html
<img
  src="https://images.unsplash.com/photo-example"
  class="img-fluid"
  alt="Beach"
/>
```

---

# Bootstrap Image Classes

| Class                    | Description                 |
| ------------------------ | --------------------------- |
| `img-fluid`              | Makes image responsive      |
| `rounded`                | Rounded corners             |
| `rounded-1`              | Small rounded corners       |
| `rounded-2`              | Medium rounded corners      |
| `rounded-3`              | Large rounded corners       |
| `rounded-4`              | Extra large rounded corners |
| `rounded-5`              | Maximum rounded corners     |
| `rounded-circle`         | Circular image              |
| `img-thumbnail`          | Thumbnail effect            |
| `border`                 | Adds border                 |
| `border-1` to `border-5` | Border thickness            |
| `border-primary`         | Blue border                 |
| `border-success`         | Green border                |
| `border-danger`          | Red border                  |
| `border-warning`         | Yellow border               |
| `border-info`            | Cyan border                 |
| `shadow`                 | Medium shadow               |
| `shadow-sm`              | Small shadow                |
| `shadow-lg`              | Large shadow                |

---

# Complete Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Bootstrap Images</title>

    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
      rel="stylesheet"
    />
  </head>
  <body>
    <div class="container my-5">
      <h1 class="text-center text-primary display-4 fw-bold mb-5">
        Beautiful Tourist Destinations
      </h1>

      <!-- Goa -->
      <div class="border rounded shadow p-4 mb-5">
        <h2 class="text-success">Goa</h2>

        <img
          src="images/goa.jpg"
          class="img-fluid rounded shadow mb-3"
          alt="Goa Beach"
        />

        <p>
          Goa is famous for its beautiful beaches, water sports, seafood, and
          Portuguese heritage.
        </p>
      </div>

      <!-- Munnar -->
      <div class="border border-info rounded-4 shadow-lg p-4">
        <h2 class="text-info">Munnar</h2>

        <img
          src="images/munnar.jpg"
          class="img-fluid rounded-4 border border-3 border-info shadow-lg mb-3"
          alt="Munnar Hills"
        />

        <p>
          Munnar is known for its lush tea plantations, cool climate, and scenic
          mountain views.
        </p>
      </div>
    </div>
  </body>
</html>
```

---

# Summary

- Use the `<img>` tag to display images.
- `img-fluid` makes images responsive.
- `rounded` and `rounded-circle` create curved edges.
- `img-thumbnail` gives a thumbnail appearance.
- `border` classes add colored and thick borders.
- `shadow` classes add depth and improve visual appearance.
- Combine multiple Bootstrap classes to create modern, attractive image layouts.
