# Assignment – Bootstrap Grid Layout

## Title: Explore Amazing Destinations

### Objective

Create a responsive **Travel Destinations** webpage using the **Bootstrap Grid System**.

In this assignment, you will practice:

- Creating Bootstrap Containers
- Using Rows and Columns
- Building responsive layouts with `col-md-*`
- Displaying Bootstrap Cards side by side
- Using Bootstrap utility classes

---

# Requirements

## 1. Add Bootstrap

Include the Bootstrap 5 CDN in your HTML file.

---

## 2. Create a Page Heading

Create the following heading:

**Explore Amazing Destinations**

Apply suitable Bootstrap classes to make it:

- Center aligned
- Blue (`text-primary`)
- Large (`display-4`)
- Bold (`fw-bold`)
- Margin on top and bottom (`my-5`)

---

## 3. Create a Responsive Grid

Create a Bootstrap **Container**.

Inside the container:

- Create one **Row**.
- Apply a gap of **4** using the `g-4` class.
- Add **three columns** using the class:

```html
col-md-4
```

The layout should behave as follows:

- 📱 **Mobile:** One card per row
- 💻 **Tablet & Desktop:** Three cards displayed side by side

---

## 4. Create Three Destination Cards

Inside each column, create one Bootstrap Card for the following tourist destinations:

- 🏝 Goa
- 🌄 Munnar
- 🏔 Ooty

Each card should contain:

- Destination Image
- Destination Name
- Short Description (3–4 lines)
- Starting Package Price
- **Explore** button
- **Book Now** button

---

## 5. Sample Destination Information

### 🏝 Goa

**Description**

Goa is famous for its beautiful beaches, Portuguese heritage, water sports, vibrant nightlife, and delicious seafood. It is one of India's most popular holiday destinations.

**Starting Package**

₹14,999

---

### 🌄 Munnar

**Description**

Munnar is a picturesque hill station in Kerala known for its lush tea plantations, misty mountains, waterfalls, and pleasant climate throughout the year.

**Starting Package**

₹11,999

---

### 🏔 Ooty

**Description**

Ooty is a charming hill station surrounded by green valleys, botanical gardens, scenic lakes, and cool weather, making it an ideal family getaway.

**Starting Package**

₹12,499

---

## 6. Apply Bootstrap Classes

### Layout

- `container`
- `row`
- `col-md-4`
- `g-4`

### Cards

- `card`
- `card-body`
- `card-title`
- `card-text`
- `card-img-top`

### Buttons

- `btn`
- `btn-primary`
- `btn-outline-primary`

### Utility Classes

- `shadow`
- `rounded`
- `h-100`
- `text-success`
- `me-2`
- `my-5`

---

# Expected Layout

### On Desktop / Laptop

```text
----------------------------------------------------------------------
                    Explore Amazing Destinations
----------------------------------------------------------------------

----------------------------------------------------------------------
|     Goa      |     Munnar      |        Ooty                      |
|    Image     |      Image      |        Image                     |
|--------------|-----------------|----------------------------------|
| Description  | Description     | Description                      |
| ₹14,999      | ₹11,999         | ₹12,499                          |
| Explore Book | Explore Book    | Explore Book                     |
----------------------------------------------------------------------
```

---

### On Mobile

```text
----------------------------
Goa Card
----------------------------

----------------------------
Munnar Card
----------------------------

----------------------------
Ooty Card
----------------------------
```

The cards should automatically stack one below another.
