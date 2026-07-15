# Bootstrap Responsive Breakpoints

Bootstrap defines **responsive breakpoints** based on the **screen width** (viewport width). These breakpoints help your layout adapt to different devices.

| Breakpoint        | Class Prefix | Screen Width | Typical Devices                   |
| ----------------- | ------------ | ------------ | --------------------------------- |
| Extra Small       | _(none)_     | **< 576px**  | Small smartphones                 |
| Small             | `sm`         | **≥ 576px**  | Large smartphones                 |
| Medium            | `md`         | **≥ 768px**  | Tablets (portrait), small laptops |
| Large             | `lg`         | **≥ 992px**  | Laptops and desktops              |
| Extra Large       | `xl`         | **≥ 1200px** | Large desktops                    |
| Extra Extra Large | `xxl`        | **≥ 1400px** | Large monitors, 2K displays       |

---

# Device Examples

| Device               | Typical Width | Bootstrap Breakpoint      |
| -------------------- | ------------: | ------------------------- |
| iPhone SE            |         375px | Extra Small               |
| iPhone 15            |         393px | Extra Small               |
| Samsung Galaxy S24   |         412px | Extra Small               |
| Large Phones         |     576–767px | Small (`sm`)              |
| iPad Mini (Portrait) |         768px | Medium (`md`)             |
| iPad Air (Portrait)  |         820px | Medium (`md`)             |
| iPad Pro 11"         |         834px | Medium (`md`)             |
| Small Laptop         |        1024px | Large (`lg`)              |
| Standard Laptop      |        1366px | Extra Large (`xl`)        |
| Full HD Desktop      |        1920px | Extra Extra Large (`xxl`) |

---

# Visual Representation

```text
Mobile
<576px
📱
Extra Small

↓

576px
📱
Small (sm)

↓

768px
📱 / 📱➡️
Tablet
Medium (md)

↓

992px
💻
Laptop
Large (lg)

↓

1200px
🖥️
Desktop
Extra Large (xl)

↓

1400px+
🖥️🖥️
Large Monitor
XXL
```

---

# Example

```html
<div class="col-sm-12 col-md-6 col-lg-4"></div>
```

### Behavior

### Mobile (<768px)

```text
--------------------
| Product 1        |
--------------------

--------------------
| Product 2        |
--------------------

--------------------
| Product 3        |
--------------------
```

One card per row.

---

### Tablet (≥768px)

```text
------------------------------
| Product 1 | Product 2 |
------------------------------

------------------------------
| Product 3 |
------------------------------
```

Two cards per row.

---

### Laptop/Desktop (≥992px)

```text
----------------------------------------
| Product1 | Product2 | Product3 |
----------------------------------------
```

Three cards per row.

---

# Memory Trick

| Breakpoint | Think Of          |
| ---------- | ----------------- |
| `sm`       | 📱 Large Phones   |
| `md`       | 📱➡️ Tablets      |
| `lg`       | 💻 Laptops        |
| `xl`       | 🖥️ Desktop PCs    |
| `xxl`      | 🖥️ Large Monitors |

---

## Imp Tip

For beginners, focus primarily on these three breakpoints:

- **`sm` (≥576px):** Large smartphones
- **`md` (≥768px):** Tablets
- **`lg` (≥992px):** Laptops and desktops
