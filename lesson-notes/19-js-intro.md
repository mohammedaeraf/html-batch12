# Lesson Notes – JavaScript Introduction

## Learning Objectives

By the end of this lesson, you will be able to:

* Understand what JavaScript is.
* Explain the role of JavaScript in web development.
* Add JavaScript to an HTML webpage.
* Create simple JavaScript functions.
* Respond to button click events.
* Show and hide webpage content using JavaScript.

---

# 1. What is JavaScript?

**JavaScript** is a programming language used to make webpages **interactive**.

While HTML creates the structure and CSS styles the webpage, JavaScript adds functionality and behavior.

For example, JavaScript can:

* Show or hide content
* Display messages
* Validate forms
* Change text or images
* Create animations
* Build interactive web applications

---

# 2. HTML, CSS and JavaScript

Think of a webpage like a house.

| Technology | Purpose                                       |
| ---------- | --------------------------------------------- |
| HTML       | Builds the structure (walls, doors, windows)  |
| CSS        | Makes it attractive (colors, fonts, design)   |
| JavaScript | Makes it interactive (lights, doors, buttons) |

---

# 3. Adding JavaScript to a Webpage

JavaScript is usually written inside the `<script>` tag.

Example:

```html
<script>

    // JavaScript code goes here

</script>
```

The `<script>` tag is commonly placed just before the closing `</body>` tag.

---

# 4. JavaScript Functions

A **function** is a block of code that performs a specific task.

Syntax:

```javascript
function functionName()
{

    // Code

}
```

Example:

```javascript
function showMessage()
{

    alert("Welcome to JavaScript!");

}
```

---

# 5. Calling a Function

A function runs only when it is called.

Example:

```html
<button onclick="showMessage()">
    Click Me
</button>
```

When the button is clicked, the function executes.

---

# 6. The `onclick` Event

The `onclick` event occurs when the user clicks an element.

Example:

```html
<button onclick="showDetails()">

    Show Details

</button>
```

When the button is clicked, the `showDetails()` function is executed.

---

# 7. Selecting an HTML Element

JavaScript can access HTML elements using their **id**.

Example:

```javascript
document.getElementById("courseDetails")
```

This selects the element whose `id` is `courseDetails`.

---

# 8. Showing and Hiding Elements (Vanilla JavaScript)

JavaScript can show or hide an element by changing its `display` property.

Hide an element:

```javascript
document.getElementById("courseDetails").style.display = "none";
```

Show an element:

```javascript
document.getElementById("courseDetails").style.display = "block";
```

---

# 9. Demo – Show and Hide Course Details

```html
<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width, initial-scale=1.0">

<title>JavaScript Introduction</title>

<link
href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css"
rel="stylesheet">

</head>

<body>

<div class="container my-5">

<h1 class="text-center text-primary mb-4">

JavaScript Introduction

</h1>

<div class="card shadow">

<div class="card-body">

<h3>Web Design Course</h3>

<p>

Click the buttons below to show or hide the course details.

</p>

<button
class="btn btn-success me-2"
onclick="showDetails()">

Show Details

</button>

<button
class="btn btn-danger"
onclick="hideDetails()">

Hide Details

</button>

<div
id="courseDetails"
class="alert alert-info mt-4"
style="display:none;">

<h5>Course Information</h5>

<ul>

<li>HTML5</li>

<li>CSS3</li>

<li>Bootstrap</li>

<li>JavaScript</li>

</ul>

</div>

</div>

</div>

</div>

<script>

function showDetails()
{

    document.getElementById("courseDetails").style.display = "block";

}

function hideDetails()
{

    document.getElementById("courseDetails").style.display = "none";

}

</script>

</body>

</html>
```

---

# 10. Understanding the Demo

### Step 1

The `<div>` is initially hidden.

```html
style="display:none;"
```

---

### Step 2

The user clicks **Show Details**.

```html
<button onclick="showDetails()">
```

---

### Step 3

The `showDetails()` function runs.

```javascript
function showDetails()
{

    document.getElementById("courseDetails").style.display = "block";

}
```

The course details become visible.

---

### Step 4

The user clicks **Hide Details**.

```html
<button onclick="hideDetails()">
```

---

### Step 5

The `hideDetails()` function runs.

```javascript
function hideDetails()
{

    document.getElementById("courseDetails").style.display = "none";

}
```

The course details disappear.

---

# 11. Using Bootstrap's `d-none` Class (Alternative Method)

Bootstrap provides the utility class `d-none` to hide an element.

HTML:

```html
<div
id="courseDetails"
class="alert alert-info mt-4 d-none">
```

JavaScript:

```javascript
function showDetails()
{

    document.getElementById("courseDetails")
            .classList.remove("d-none");

}

function hideDetails()
{

    document.getElementById("courseDetails")
            .classList.add("d-none");

}
```

This approach is commonly used in Bootstrap-based projects.

---

# 12. Vanilla JavaScript vs Bootstrap Method

| Vanilla JavaScript                   | Bootstrap Method                      |
| ------------------------------------ | ------------------------------------- |
| `style.display = "none"`             | `classList.add("d-none")`             |
| `style.display = "block"`            | `classList.remove("d-none")`          |
| Directly changes the element's style | Adds or removes a Bootstrap CSS class |
| Easy for beginners                   | Common in Bootstrap projects          |

---

# Summary

In this lesson, you learned:

* What JavaScript is
* The role of JavaScript in web development
* How to add JavaScript using the `<script>` tag
* How to create and call functions
* How to use the `onclick` event
* How to select HTML elements using `getElementById()`
* How to show and hide content using JavaScript
* The difference between the `style.display` method and Bootstrap's `d-none` class

---

# Practice Exercise

Create a webpage titled **"Student Information"**.

Requirements:

1. Add a heading titled **Student Information**.
2. Create a Bootstrap card.
3. Inside the card, display a short paragraph explaining that student details can be shown or hidden.
4. Add two buttons:

   * Show Information
   * Hide Information
5. Add a hidden Bootstrap alert containing:

   * Student Name
   * Course
   * Batch
   * Duration
6. Use JavaScript functions named:

   * `showInfo()`
   * `hideInfo()`
7. Show and hide the alert using:

```javascript
style.display = "block";
```

and

```javascript
style.display = "none";
```

---

## Learning Outcome

By completing this exercise, you will understand the basic workflow of JavaScript—responding to user actions, selecting HTML elements, creating functions, and changing webpage content dynamically. These concepts form the foundation for learning variables, conditions, loops, DOM manipulation, and interactive web development.
