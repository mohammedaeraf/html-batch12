# Assignment – Bootstrap Grid Layout

## Title: Online Gadget Store

### Objective

Create a responsive **Online Gadget Store** webpage using the **Bootstrap Grid System**.

In this assignment, you will practice:

* Creating Bootstrap Containers
* Using Rows and Columns
* Building responsive layouts with `col-md-*`
* Displaying Bootstrap Cards side by side
* Using Bootstrap utility classes

---

# Requirements

## 1. Add Bootstrap

Include the Bootstrap 5 CDN in your HTML file.

---

## 2. Create a Page Heading

Create the following heading:

**Online Gadget Store**

Apply suitable Bootstrap classes to make it:

* Center aligned
* Blue (`text-primary`)
* Large (`display-4`)
* Bold (`fw-bold`)
* Margin on top and bottom (`my-5`)

---

## 3. Create a Responsive Grid

Create a Bootstrap **Container**.

Inside the container:

* Create one **Row**.
* Apply a gap of **4** using the `g-4` class.
* Add **three columns** using the class:

```html
col-md-4
```

The layout should behave as follows:

* 📱 **Mobile:** One card per row
* 📱 **Tablet & Desktop:** Three cards side by side

---

## 4. Create Three Product Cards

Inside each column, create one Bootstrap Card for the following products:

* 💻 Laptop
* 📱 Smartphone
* ⌚ Smart Watch

Each card should contain:

* Product Image
* Product Name
* Short Description (3–4 lines)
* Price
* **Buy Now** button
* **View Details** button

---

## 5. Sample Product Information

### 💻 Laptop

**Description**

Powerful laptop with Intel Core i7 processor, 16GB RAM and 512GB SSD, suitable for programming, office work, and entertainment.

**Price**

₹59,999

---

### 📱 Smartphone

**Description**

Latest smartphone featuring a vibrant AMOLED display, powerful processor, excellent camera, and long-lasting battery.

**Price**

₹24,999

---

### ⌚ Smart Watch

**Description**

Stylish smartwatch with heart-rate monitoring, fitness tracking, sleep analysis, and Bluetooth calling.

**Price**

₹6,999

---

## 6. Apply Bootstrap Classes

### Layout

* `container`
* `row`
* `col-md-4`
* `g-4`

### Cards

* `card`
* `card-body`
* `card-title`
* `card-text`
* `card-img-top`

### Buttons

* `btn`
* `btn-primary`
* `btn-outline-primary`

### Utility Classes

* `shadow`
* `rounded`
* `h-100`
* `text-success`
* `me-2`
* `my-5`

---

# Expected Layout

### On Desktop / Laptop

```text
-------------------------------------------------------------
                  Online Gadget Store
-------------------------------------------------------------

-------------------------------------------------------------
|   Laptop   |   Smartphone   |   Smart Watch              |
|   Image    |     Image      |      Image                 |
|------------|----------------|----------------------------|
| Description| Description    | Description                |
| ₹59,999    | ₹24,999        | ₹6,999                    |
| Buy | View | Buy | View     | Buy | View                |
-------------------------------------------------------------
```

---

### On Mobile

```text
----------------------------
Laptop Card
----------------------------

----------------------------
Smartphone Card
----------------------------

----------------------------
Smart Watch Card
----------------------------
```

The cards should automatically stack one below another.
