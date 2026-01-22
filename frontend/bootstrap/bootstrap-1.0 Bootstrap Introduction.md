# Bootstrap — Introduction

## What is it?

Bootstrap is a **CSS framework** that provides prebuilt styles and components.
Instead of writing all CSS from scratch, you include Bootstrap in your project and use its predefined classes.

Bootstrap is not the only framework available.
Others include **Tailwind CSS**, **Foundation**, and more.

> A framework is a productivity tool.  
> A web developer should still understand how to write CSS without it.

---

## Why use Bootstrap?

Bootstrap is well known for its **12-column grid system**, built on top of Flexbox.
This system makes layouts **responsive by default** and supports a **mobile-first approach**.

### Mobile-first (brief explanation)

Mobile-first means designing layouts for **small screens first**, then progressively enhancing them for larger screens.
Bootstrap’s breakpoints and grid system are designed around this principle.

---

## What does Bootstrap allow you to do?

Bootstrap allows you to:
- build interfaces quickly
- maintain visual consistency
- reduce the amount of custom CSS needed

In practice, it trades **fine-grained control** for **speed and consistency**.

---

## Drawbacks

Bootstrap also has limitations:

- HTML and styling are tightly coupled through class names
- Customization can become harder over time
- Overuse can lead to similar-looking websites

These drawbacks matter more as projects grow in complexity.

---

## When to use it vs when not to

### Use Bootstrap when:
- you need a responsive layout quickly
- design is not the main focus
- consistency matters more than uniqueness

### Avoid Bootstrap when:
- building a complex, highly custom UI
- full design control is required
- the project is extremely small or extremely large

---

## Installing Bootstrap

Bootstrap can be used in two main ways: **via CDN** or **locally**.

### Using a CDN

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
```

```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

> A CDN (Content Delivery Network) hosts files on distributed servers to improve loading speed.

---

### Installing Bootstrap locally

Installing Bootstrap locally gives you **full control** over the files and avoids external dependencies.

#### Step 1 — Download Bootstrap

Download Bootstrap from the official website:
- https://getbootstrap.com/

Choose the **compiled CSS and JS** version.

#### Step 2 — Add files to your project

```text
project/
├── css/
│   └── bootstrap.min.css
├── js/
│   └── bootstrap.bundle.min.js
└── index.html
```

#### Step 3 — Link Bootstrap locally

```html
<link rel="stylesheet" href="css/bootstrap.min.css">
<script src="js/bootstrap.bundle.min.js"></script>
```

This approach is recommended when:
- working offline
- learning Bootstrap internals
- avoiding CDN usage

---

## Using Bootstrap with custom CSS

To override Bootstrap styles, always include your custom CSS **after** Bootstrap:

```html
<link rel="stylesheet" href="css/bootstrap.min.css">
<link rel="stylesheet" href="css/style.css">
```
