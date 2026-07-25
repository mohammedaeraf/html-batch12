# Mini Project – Bootstrap Single Page Website

## Title: Future Leaders Academy

### Objective

Design a professional **single-page website** for **Future Leaders Academy** using HTML, Bootstrap, Google Fonts, Bootstrap Icons, Images, Cards, Grid Layout, and Internal Links.

This mini project combines all the Bootstrap concepts learned so far.

---

# Concepts Covered

* HTML Internal Links
* Bootstrap Containers
* Bootstrap Grid Layout
* Bootstrap Cards
* Bootstrap Buttons
* Bootstrap Alerts
* Bootstrap Utility Classes
* Bootstrap Images
* Bootstrap Icons
* Google Fonts
* Responsive Design

---

# Project Requirements

## 1. Add Required Libraries

Include the following in the `<head>` section:

* Bootstrap 5 CDN
* Google Font (**Poppins**)
* Bootstrap Icons CDN

Apply the **Poppins** font to the entire webpage.

---

## 2. Create the Page Header

Display the heading:

**Future Leaders Academy**

Add an **education icon** before the heading.

Below the heading, add the following subtitle:

> Learn. Build. Succeed.

Center-align both the heading and subtitle.

---

## 3. Navigation Menu

Create a Bootstrap navigation menu using buttons.

The menu should contain:

* Home
* Courses
* About
* Contact

Each button should navigate to its corresponding section using **internal links**.

---

## 4. Home Section

Create a section with:

* Heading: **Welcome to Future Leaders Academy**
* Short introductory paragraph
* A Bootstrap **Success Alert** displaying:

> 🎉 Admissions Open for New Batches!

Use Bootstrap classes:

* `bg-primary-subtle`
* `rounded`
* `shadow`
* `p-4`

---

## 5. Courses Section

Create a responsive Bootstrap Grid.

Use:

```html
col-12 col-md-6 col-lg-4
```

Create **three Bootstrap Cards**.

### Course 1

**Web Design**

Include:

* Course Image
* Course Name
* Short Description
* **Learn More** button

---

### Course 2

**Python Programming**

Include:

* Course Image
* Course Name
* Short Description
* **Learn More** button

---

### Course 3

**AWS Fundamentals**

Include:

* Course Image
* Course Name
* Short Description
* **Learn More** button

Each card should include:

* Course Image
* Bootstrap Icon
* Course Title
* Description
* Button
* Shadow
* Rounded Corners
* Equal Height

---

## 6. About Section

Create a card containing:

* Academy image
* Heading
* About the academy
* Years of experience
* Number of students trained

Add suitable Bootstrap Icons.

---

## 7. Contact Section

Display:

* Address
* Phone Number
* Email Address
* Website

Add suitable icons before each item.

Example:

* 📍 Location
* ☎ Phone
* ✉ Email
* 🌐 Website

---

## 8. Back to Top Button

At the bottom of the page, create a button:

**↑ Back to Top**

Clicking the button should navigate to the **Home** section.

---

# Bootstrap Classes to Use

### Layout

* `container`
* `row`
* `col-12`
* `col-md-6`
* `col-lg-4`
* `g-4`

### Cards

* `card`
* `card-body`
* `card-title`
* `card-text`
* `card-img-top`
* `h-100`

### Buttons

* `btn`
* `btn-primary`
* `btn-success`
* `btn-outline-primary`

### Typography

* `display-4`
* `fw-bold`
* `text-center`
* `text-primary`
* `text-success`

### Utility Classes

* `my-5`
* `mb-4`
* `p-4`
* `rounded`
* `shadow`
* `me-2`

---

# Expected Layout

```text
---------------------------------------------------------
      🎓 Future Leaders Academy
         Learn. Build. Succeed.
---------------------------------------------------------

[ Home ] [ Courses ] [ About ] [ Contact ]

---------------------------------------------------------
🎉 Admissions Open for New Batches!
---------------------------------------------------------

---------------------------------------------------------
| Web Design | Python | AWS Fundamentals |
|   Image    |  Image |      Image       |
|------------|--------|------------------|
| Description|Description|Description    |
| Learn More |Learn More |Learn More     |
---------------------------------------------------------

---------------------------------------------------------
About Future Leaders Academy
Image
Short description about the academy.
---------------------------------------------------------

---------------------------------------------------------
📍 Address

☎ Phone

✉ Email

🌐 Website
---------------------------------------------------------

              [ ↑ Back to Top ]
```

---

# Submission Guidelines

* Save the file as **`future-leaders-academy.html`**.
* Ensure that all navigation buttons work correctly.
* Use the **Poppins** Google Font throughout the webpage.
* Display Bootstrap Icons appropriately.
* Ensure all course cards are responsive and aligned properly.
* Test the webpage on mobile and desktop screens.
* Use Bootstrap classes wherever possible. Avoid unnecessary custom CSS.

---

## Learning Outcome

By completing this mini project, you will integrate all the concepts learned so far into a single responsive webpage. You will gain practical experience in creating a professional-looking website using **Bootstrap Grid Layout, Cards, Images, Google Fonts, Bootstrap Icons, Internal Links, Alerts, Buttons, and Utility Classes**, preparing you for building complete responsive websites.
