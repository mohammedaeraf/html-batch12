# Assignment – Bootstrap Tables

## Title: Employee Salary Report

### Objective

Create a professional-looking **Employee Salary Report** using **Bootstrap Tables**.

In this assignment, you will practice:

* Creating HTML tables
* Applying Bootstrap table classes
* Using table headers and table body
* Making tables responsive
* Displaying tabular data in an organized format

---

# Requirements

## 1. Add Bootstrap

Include the Bootstrap 5 CDN in your HTML file.

---

## 2. Create a Page Heading

Create the following heading:

**Employee Salary Report**

Apply suitable Bootstrap classes to make it:

* Center aligned
* Blue (`text-primary`)
* Large (`display-4`)
* Bold (`fw-bold`)
* Margin on top and bottom (`my-5`)

---

## 3. Create a Responsive Table

Wrap your table inside a Bootstrap **`table-responsive`** container.

Create a table with the following columns:

* Employee ID
* Employee Name
* Department
* Designation
* Experience (Years)
* Monthly Salary

Add **at least 6 employee records**.

---

## 4. Apply Bootstrap Table Classes

Use the following Bootstrap classes:

* `table`
* `table-striped`
* `table-bordered`
* `table-hover`

Use the **`table-dark`** class for the table header (`<thead>`).

---

## 5. Sample Data

You may use the following sample data or create your own.

| Employee ID | Name         | Department | Designation         | Experience |  Salary |
| ----------- | ------------ | ---------- | ------------------- | ---------: | ------: |
| EMP101      | Rahul Sharma | IT         | Web Developer       |          3 | ₹45,000 |
| EMP102      | Priya Nair   | HR         | HR Executive        |          5 | ₹52,000 |
| EMP103      | Amit Verma   | Finance    | Accountant          |          4 | ₹48,000 |
| EMP104      | Sneha Patel  | Marketing  | Marketing Executive |          2 | ₹40,000 |
| EMP105      | Arjun Mehta  | Sales      | Sales Manager       |          6 | ₹65,000 |
| EMP106      | Neha Kapoor  | IT         | Software Engineer   |          7 | ₹78,000 |

---

## 6. Use Bootstrap Utility Classes

Apply appropriate Bootstrap spacing classes to improve the appearance of the page.

Suggested classes:

### Typography

* `text-center`
* `text-primary`
* `display-4`
* `fw-bold`

### Table

* `table`
* `table-striped`
* `table-bordered`
* `table-hover`
* `table-dark`

### Layout

* `container`
* `table-responsive`
* `my-5`

---

# Expected Layout

```text
---------------------------------------------------------------
                 Employee Salary Report
---------------------------------------------------------------

+-----------------------------------------------------------------------------------------------+
| Employee ID | Name          | Department | Designation      | Experience | Monthly Salary    |
+-----------------------------------------------------------------------------------------------+
| EMP101      | Rahul Sharma  | IT         | Web Developer    | 3 Years    | ₹45,000           |
| EMP102      | Priya Nair    | HR         | HR Executive     | 5 Years    | ₹52,000           |
| EMP103      | Amit Verma    | Finance    | Accountant       | 4 Years    | ₹48,000           |
| EMP104      | Sneha Patel   | Marketing  | Marketing Exec.  | 2 Years    | ₹40,000           |
| EMP105      | Arjun Mehta   | Sales      | Sales Manager    | 6 Years    | ₹65,000           |
| EMP106      | Neha Kapoor   | IT         | Software Engineer| 7 Years    | ₹78,000           |
+-----------------------------------------------------------------------------------------------+
```

---

# Bonus Challenge ⭐

Complete **any two** of the following:

1. Add a **Status** column showing:

   * Active
   * On Leave
   * Probation

2. Use a different Bootstrap color for the table header such as:

   * `table-primary`
   * `table-success`
   * `table-info`

3. Add **two more employee records**.

4. Apply the `table-sm` class to create a compact version of the table and compare it with the normal table.

---

# Submission Guidelines

* Save the file as **`employee-report.html`**.
* Test the webpage in a browser before submitting.
* Use **Bootstrap classes only** for styling. Do **not** use custom CSS.

---

## Learning Outcome

By completing this assignment, you will learn how to create responsive and visually appealing **Bootstrap Tables** using table styling classes, responsive containers, and Bootstrap utility classes to present structured data effectively.
