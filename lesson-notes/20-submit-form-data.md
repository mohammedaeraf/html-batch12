# Tutorial – Submitting Contact Form Data Using Formspree

## Introduction

Normally, when a user submits a Contact Us form, the form data needs to be processed by a **backend/server**.

For example:

```text
HTML Form
    ↓
Backend / Server
    ↓
Database / Email
```

However, beginner web designers may not yet know backend programming.

Services such as **Formspree** allow us to submit HTML form data to a third-party service without creating our own backend.

The basic process is:

```text
User fills Contact Form
        ↓
    Submit Form
        ↓
     Formspree
        ↓
Email / Formspree Dashboard
```

---

# Learning Objectives

By the end of this tutorial, you will be able to:

* Create a Formspree account.
* Create a Formspree project.
* Create a Contact Us form.
* Connect an HTML form to Formspree.
* Use a Formspree endpoint in the `action` attribute.
* Understand the importance of the `name` attribute.
* Submit and test form data.
* View submitted data through email and the Formspree dashboard.

---

# 1. Create a Formspree Account

Open:

**formspree.io**

Create an account using your email address.

You may be asked to verify your email address.

After registration, sign in to your Formspree account.

---

# 2. Sign In

After creating your account:

1. Open Formspree.
2. Click **Sign In**.
3. Enter your registered email address and password.
4. You will be taken to your Formspree dashboard.

---

# 3. Create a Project

From the Formspree dashboard:

1. Create a new project.
2. Give your project a suitable name.

For example:

```text
Web Design Website
```

A project helps you organize the forms associated with your website.

---

# 4. Create a Form

Inside your project, create a new form.

Give the form the name:

```text
Contact Us Form
```

After creating the form, Formspree will provide a unique **form endpoint**.

It will look similar to:

```text
https://formspree.io/f/xxxxxxxx
```

Your actual endpoint will be different.

### Important

Do **not** copy the example endpoint above.

Copy the endpoint provided by your own Formspree account.

---

# 5. Create an HTML Contact Form

Let's create a simple Contact Us form using Bootstrap.

```html
<form>

    <div class="mb-3">

        <label class="form-label">
            Name
        </label>

        <input
            type="text"
            class="form-control">

    </div>


    <div class="mb-3">

        <label class="form-label">
            Email
        </label>

        <input
            type="email"
            class="form-control">

    </div>


    <div class="mb-3">

        <label class="form-label">
            Subject
        </label>

        <input
            type="text"
            class="form-control">

    </div>


    <div class="mb-3">

        <label class="form-label">
            Message
        </label>

        <textarea
            class="form-control"
            rows="5"></textarea>

    </div>


    <button
        type="submit"
        class="btn btn-primary">

        Send Message

    </button>

</form>
```

At this stage, the form exists visually, but we haven't connected it to Formspree.

---

# 6. Add the Formspree Endpoint

The Formspree endpoint must be added to the form's `action` attribute.

For example:

```html
<form action="YOUR-FORMSPREE-ENDPOINT">
```

Replace `YOUR-FORMSPREE-ENDPOINT` with the endpoint provided by Formspree.

For example:

```html
<form action="https://formspree.io/f/xxxxxxxx">
```

### Important

Your endpoint will be unique to your Formspree form.

---

# 7. Use the POST Method

The form should also use the `POST` method.

```html
<form
    action="https://formspree.io/f/xxxxxxxx"
    method="POST">
```

The important attributes are:

```text
action → Where the form data should be sent

method → How the data should be sent
```

For submitting form data, we generally use:

```html
method="POST"
```

---

# 8. Give Every Field a `name`

This is one of the **most important steps**.

Every form field that you want to submit must have a `name` attribute.

For example:

```html
<input
    type="text"
    name="name"
    class="form-control">
```

Email:

```html
<input
    type="email"
    name="email"
    class="form-control">
```

Subject:

```html
<input
    type="text"
    name="subject"
    class="form-control">
```

Message:

```html
<textarea
    name="message"
    class="form-control">
</textarea>
```

---

# 9. Why is `name` Important?

The `name` attribute identifies the data being submitted.

For example:

```html
<input
    type="text"
    name="name">
```

If the user enters:

```text
Ahmed
```

the submitted data will contain something similar to:

```text
name = Ahmed
```

Similarly:

```html
<input
    type="email"
    name="email">
```

might produce:

```text
email = ahmed@example.com
```

### Remember

An `id` is mainly useful for identifying an element within the webpage.

A `name` identifies the **form data being submitted**.

Therefore, for form submission:

```html
name="email"
```

is important.

---

# 10. Complete Contact Us Form

Here is a complete example using Bootstrap and Formspree.

Replace the endpoint with your own endpoint.

```html
<form
    action="https://formspree.io/f/xxxxxxxx"
    method="POST">

    <div class="mb-3">

        <label class="form-label">
            Name
        </label>

        <input
            type="text"
            name="name"
            class="form-control"
            required>

    </div>


    <div class="mb-3">

        <label class="form-label">
            Email
        </label>

        <input
            type="email"
            name="email"
            class="form-control"
            required>

    </div>


    <div class="mb-3">

        <label class="form-label">
            Subject
        </label>

        <input
            type="text"
            name="subject"
            class="form-control"
            required>

    </div>


    <div class="mb-3">

        <label class="form-label">
            Message
        </label>

        <textarea
            name="message"
            class="form-control"
            rows="5"
            required></textarea>

    </div>


    <button
        type="submit"
        class="btn btn-primary">

        Send Message

    </button>

</form>
```

---

# 11. Test the Form

Now test your form.

### Step 1

Open your webpage in the browser.

### Step 2

Enter some sample information.

For example:

```text
Name: Ahmed Khan

Email: ahmed@example.com

Subject: Course Enquiry

Message: I would like to know more about the Web Design course.
```

### Step 3

Click:

**Send Message**

The form data will be submitted to Formspree.

---

# 12. Check Your Email

After submitting the form, check the email account associated with your Formspree account.

You should receive an email containing the submitted information.

For example:

```text
Name: Ahmed Khan

Email: ahmed@example.com

Subject: Course Enquiry

Message:
I would like to know more about the Web Design course.
```

---

# 13. Check the Formspree Dashboard

You can also log in to Formspree and open your **Contact Us Form**.

You should be able to see the submissions received through the form.

This gives you two ways to monitor submissions:

```text
                Formspree
                   |
          -------------------
          |                 |
        Email           Dashboard
```

---

# 14. Complete Process

The complete workflow is:

```text
1. Register on Formspree
             ↓
2. Sign In
             ↓
3. Create Project
             ↓
4. Create Contact Us Form
             ↓
5. Copy Form Endpoint
             ↓
6. Add Endpoint to <form action="">
             ↓
7. Add method="POST"
             ↓
8. Add name to every form field
             ↓
9. Test the form
             ↓
10. Check Email
             ↓
11. Check Formspree Dashboard
```

---

# Important Concepts

## `action`

Specifies where the form data should be submitted.

```html
<form action="https://formspree.io/f/xxxxxxxx">
```

---

## `method`

Specifies how the form data is submitted.

```html
<form method="POST">
```

---

## `name`

Identifies the submitted form field.

```html
<input name="email">
```

---

## `required`

Makes a field mandatory.

```html
<input
    type="text"
    name="name"
    required>
```

---

# Common Mistakes

### Mistake 1 – Missing `action`

Incorrect:

```html
<form>
```

Correct:

```html
<form
    action="YOUR-FORMSPREE-ENDPOINT"
    method="POST">
```

---

### Mistake 2 – Missing `name`

Incorrect:

```html
<input
    type="email"
    class="form-control">
```

Correct:

```html
<input
    type="email"
    name="email"
    class="form-control">
```

---

### Mistake 3 – Using the wrong endpoint

Make sure you copy the endpoint from **your own Formspree form**.

---

### Mistake 4 – Forgetting `method="POST"`

Use:

```html
method="POST"
```

when submitting the form.

---

# Practice Exercise

Create a **Contact Us** section for a fictional company called:

**PixelBoost Digital Agency**

Create a form containing:

* Full Name
* Email
* Phone
* Subject
* Message

Requirements:

1. Use Bootstrap form classes.
2. Connect the form to your Formspree account.
3. Add your Formspree endpoint to the `action` attribute.
4. Use `method="POST"`.
5. Give every field a suitable `name`.
6. Make all fields required except Phone.
7. Add a **Send Message** button.
8. Submit a test enquiry.
9. Verify that the submission is received by email.
10. Verify that the submission appears in the Formspree dashboard.

---

# Key Takeaway

Formspree allows a **static HTML website** to submit form data without creating your own backend.

The three most important things to remember are:

```html
<form
    action="YOUR-FORMSPREE-ENDPOINT"
    method="POST">
```

and:

```html
<input name="name">
<input name="email">
<textarea name="message"></textarea>
```

**`action` → Where the data goes**

**`method` → How the data is sent**

**`name` → What the submitted data is called**
