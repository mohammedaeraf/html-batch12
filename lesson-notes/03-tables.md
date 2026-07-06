# HTML Tables – Quick Notes

## What is a Table?

A **table** is used to display information in **rows** and **columns**.

**Examples:**

- Student Marks
- Employee Details
- Product List
- Timetable

---

# Basic Table Tags

| Tag       | Purpose                     |
| --------- | --------------------------- |
| `<table>` | Creates a table             |
| `<thead>` | Contains the table headings |
| `<tbody>` | Contains the table data     |
| `<tr>`    | Creates a row               |
| `<th>`    | Creates a heading cell      |
| `<td>`    | Creates a data cell         |

---

# Basic Table Example

```html
<table>
  <thead>
    <tr>
      <th>ID</th>
      <th>Name</th>
      <th>Course</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>101</td>
      <td>Rahul</td>
      <td>HTML</td>
    </tr>

    <tr>
      <td>102</td>
      <td>Aisha</td>
      <td>CSS</td>
    </tr>
  </tbody>
</table>
```

---

# CSS Styling

```css
table {
  width: 60%;
  border-collapse: collapse;
}

th,
td {
  border: 1px solid gray;
  padding: 10px;
  text-align: center;
}

thead {
  background-color: royalblue;
  color: white;
}

tbody tr:nth-child(even) {
  background-color: #f2f2f2;
}

tbody tr:hover {
  background-color: lightyellow;
}
```

---

# Merging Cells

### Merge Columns

```html
<th colspan="3">Student Details</th>
```

### Merge Rows

```html
<td rowspan="2">Rahul</td>
```

---

# Why Use `<thead>` and `<tbody>`?

- Makes tables well organized.
- Easier to style using CSS.
- Improves readability.
- Used in modern web development.

---

# Best Practices

- Use `<th>` for headings.
- Use CSS instead of the HTML `border` attribute.
- Use `border-collapse: collapse;` for a cleaner look.
- Add `padding` for better spacing.
- Use alternate row colors (`nth-child`) for readability.
- Add a hover effect to improve user experience.

---

# Summary

- A table displays data in rows and columns.
- Use `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, and `<td>` to build tables.
- Style tables with CSS to make them attractive and easy to read.
- Modern websites use semantic table elements like `<thead>` and `<tbody>`.
