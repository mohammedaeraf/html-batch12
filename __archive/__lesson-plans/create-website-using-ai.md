For **Grade 7–10 students**, I’d make the final session feel like a **mini-project rather than an AI lecture**. The students should experience the complete journey:

**Idea → Prompt ChatGPT → Get Website → Open in Browser → Modify with GitHub Copilot → Publish**

## Recommended Theme: 🍕 Pizza Café Website

I recommend a **Pizza Café** rather than a portfolio or business website because it is:

* Fun and relatable for school students
* Visually attractive
* Easy to understand
* Rich enough to demonstrate several Bootstrap components
* Easy to modify with AI
* Possible to complete in one session

### Suggested Website

**"Pizza Palace" – A Modern Pizza Café**

Sections:

1. **Navbar**
2. **Hero Section**
3. **Popular Pizzas** – 3 Bootstrap Cards
4. **Why Choose Us** – 3 simple features
5. **Special Offer** – Bootstrap Alert
6. **Contact Us**
7. **Footer**

This also revises many concepts they've already learned: **Navbar, Container, Grid, Cards, Buttons, Images, Icons, Google Fonts, Alerts and responsive design.**

---

# Final Session Plan

### Duration: 90–120 minutes

| Time   | Activity                               |
| ------ | -------------------------------------- |
| 10 min | Introduction to AI-assisted Web Design |
| 15 min | Generate website using ChatGPT         |
| 15 min | Run and inspect the website            |
| 10 min | Ask ChatGPT to improve the website     |
| 15 min | Introduce GitHub Copilot               |
| 20 min | Modify website using Copilot           |
| 10 min | Save/commit/push changes               |
| 10 min | Student challenge                      |
| 5 min  | Final discussion                       |

---

# Part 1 – Introduce AI-Assisted Web Design

Start with a simple question:

> **"Can AI create a website for us?"**

Explain:

```text
Traditional Approach

Idea
 ↓
Write HTML
 ↓
Write CSS
 ↓
Write Bootstrap
 ↓
Test
 ↓
Fix Errors
```

With GenAI:

```text
Idea
 ↓
Describe what we want
 ↓
AI generates code
 ↓
We test it
 ↓
We modify it
```

But emphasize:

> **AI creates the code. We are still the designers.**

Students should learn to **describe, test, evaluate and modify** the result rather than blindly copying AI-generated code.

---

# Part 2 – Generate the Website Using ChatGPT

Tell students to open ChatGPT.

Give them this prompt.

## Prompt 1 – Create the Website

```text
Create a complete responsive website called "Pizza Palace", a modern pizza café.

Target audience: teenagers and families.

Use:
- HTML5
- Bootstrap 5
- Bootstrap Icons
- Google Fonts

Important requirements:
- Maximise the use of Bootstrap 5 classes.
- Keep custom CSS to an absolute minimum.
- Do not use external CSS frameworks other than Bootstrap.
- Use Bootstrap containers, rows, columns, cards, buttons, alerts and navbar classes wherever possible.
- Make the website responsive for mobile, tablet and desktop.
- Use Bootstrap grid classes such as col-lg-4 col-md-6 col-12.
- Use attractive images from Unsplash.
- Use Bootstrap Icons wherever appropriate.

Create these sections:

1. Responsive Navbar
   - Pizza Palace logo/name
   - Home
   - Menu
   - About
   - Contact

2. Hero section
   - Large heading: "Fresh Pizza. Happy Moments."
   - Short description
   - "View Menu" button
   - Attractive pizza image

3. Popular Pizzas
   - Three Bootstrap cards
   - Margherita
   - BBQ Chicken
   - Veggie Supreme
   - Each card should have an image, title, description, price and button.
   - Cards should have equal height.

4. Why Choose Us
   - Three simple features using Bootstrap Icons:
     Fresh Ingredients
     Fast Delivery
     Great Taste

5. Special Offer
   - Use a Bootstrap alert.
   - Display: "Get 20% OFF on your first order!"

6. Contact section
   - Name
   - Email
   - Message
   - Submit button

7. Footer
   - Copyright message
   - Social media icons

Use semantic HTML elements such as header, nav, main, section and footer.

Use Bootstrap utility classes extensively for spacing, alignment, colors, typography, shadows and responsiveness.

Keep the code beginner-friendly and well commented.

Return the complete HTML file in one code block.
```

---

# Part 3 – Students Run the Website

Ask students to:

1. Copy the generated HTML.
2. Open VS Code.
3. Create:

```text
pizza-palace
    └── index.html
```

4. Paste the code.
5. Save.
6. Open the page in the browser.

Then ask:

> **"Does the website look exactly the way you imagined?"**

This is an important teaching moment.

Explain that **the first AI-generated result doesn't have to be perfect.**

---

# Part 4 – Improve the Website Using ChatGPT

Now demonstrate how students can give AI **incremental instructions**.

Instead of generating the whole website again, ask ChatGPT:

## Prompt 2 – Improve the Hero

```text
Improve only the Hero section of the Pizza Palace website.

Make it more visually attractive using Bootstrap 5 classes.

Requirements:
- Use Bootstrap classes as much as possible.
- Do not add custom CSS unless absolutely necessary.
- Make the heading large and bold.
- Add a short attractive tagline.
- Add two buttons: "View Menu" and "Order Now".
- Improve spacing and alignment.
- Keep it responsive.

Return only the modified Hero section.
```

This teaches an important AI skill:

> **Give AI a specific task instead of asking it to rebuild everything.**

---

# Part 5 – Another Simple Modification

Ask students to try their own prompt.

Give them examples:

### Change the colors

```text
Change the Pizza Palace color theme to a warm red, orange and cream theme using Bootstrap classes as much as possible. Minimise custom CSS.
```

### Add another pizza

```text
Add a fourth pizza called Cheese Burst Pizza to the Popular Pizzas section. Use the same Bootstrap card structure and grid layout.
```

### Add an offer

```text
Change the Special Offer section into a Bootstrap warning alert with a suitable Bootstrap Icon.
```

### Add icons

```text
Add suitable Bootstrap Icons to the navigation links, buttons and Why Choose Us section.
```

---

# Part 6 – Introduce GitHub Copilot

Now make the distinction very simple.

### ChatGPT

> **Create / explain / suggest code**

### GitHub Copilot

> **Help me write or modify code while I'm working in VS Code.**

Show students that they can select existing code and ask Copilot to modify it.

---

# Part 7 – GitHub Copilot Demo

Open the Pizza Palace project in VS Code.

Select the **Popular Pizzas** section.

Ask Copilot:

```text
Modify this section.

Add one more Bootstrap card for "Cheese Burst Pizza".

Use the same structure as the existing cards.

Use Bootstrap 5 classes wherever possible.
Do not introduce custom CSS.
Keep all cards equal height and responsive.
```

Copilot should modify the existing code.

Students can immediately see the difference between:

```text
ChatGPT
↓
Generate website
```

and:

```text
Copilot
↓
Modify existing code
```

---

# Part 8 – Let Copilot Improve Something

Give students a small challenge.

### Challenge

Ask Copilot:

```text
Improve the Popular Pizzas cards.

Requirements:
- Use Bootstrap 5 classes.
- Add a Bootstrap shadow.
- Make the cards equal height.
- Add a suitable Bootstrap Icon to each button.
- Improve spacing using Bootstrap utility classes.
- Do not create custom CSS.
```

Students can see the changes immediately.

---

# Part 9 – Teach Students to Ask AI Properly

This is perhaps the **most valuable lesson of the entire session**.

Show them the difference.

### ❌ Weak Prompt

```text
Make my website better.
```

### ✅ Better Prompt

```text
Improve the Pizza cards.

Use Bootstrap 5 classes.
Make them equal height.
Improve spacing.
Add Bootstrap Icons.
Keep custom CSS to a minimum.
Do not change the content.
```

Explain:

> **The more clearly you describe the desired result, the more useful the AI response is likely to be.**

---

# Part 10 – Final Student Challenge

Give students **20 minutes** to customize their Pizza Palace website.

They can ask ChatGPT or Copilot to do **any three** of the following:

### Challenge Options

* 🍕 Add a new pizza
* 🎨 Change the color theme
* 🖼️ Change the hero image
* ⭐ Add customer reviews
* 💰 Add a "Today's Special" card
* 📱 Improve mobile layout
* 🔔 Add an alert
* 🧭 Add a navigation link
* 📞 Add contact information
* 🧑‍🍳 Add an "Our Chef" section
* 🛒 Change "Order Now" buttons
* ⭐ Add star ratings

But give them one important rule:

> **Do not ask AI to recreate the entire website. Ask it to modify one section at a time.**

---

# Part 11 – Save the Project to GitHub

This is a great way to connect today's session with the Git/GitHub lesson you taught previously.

Students can use VS Code:

```text
Source Control
      ↓
Stage Changes
      ↓
Commit
      ↓
Push
```

Commit message:

```text
Updated Pizza Palace website using AI
```

Then their final project is available in their GitHub repository.

---

# Optional Final Step – GitHub Pages

If you have enough time, this makes a **fantastic ending to the course**.

Students can publish their Pizza Palace website using GitHub Pages.

The complete journey becomes:

```text
Idea
  ↓
ChatGPT
  ↓
HTML + Bootstrap
  ↓
VS Code
  ↓
GitHub Copilot
  ↓
Modify Website
  ↓
Git
  ↓
GitHub
  ↓
GitHub Pages
  ↓
🌐 LIVE WEBSITE
```

That's a very satisfying final project for Grade 7–10 students.

---

# 🎯 Final Message to Students

I'd end the session with something like:

> **"You don't need to know everything before you start creating. Today you've learned how to use AI as a tool to help you build, understand and improve websites. But remember—AI is your assistant, not your replacement. Your creativity, ideas and ability to make good design decisions are what make the website yours."**

And perhaps give them a final challenge:

> **"This week, create a completely different website using ChatGPT. You decide the theme—Restaurant, School, Sports Club, Gaming Website, Travel Website or anything you like. Then use GitHub Copilot to make at least three improvements."**

That keeps the final session **fun, practical and memorable**, without turning it into an overwhelming "AI coding" class.
