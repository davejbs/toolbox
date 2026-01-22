# Bootstrap — Layout

## 12-Column Grid System

Bootstrap’s layout system is based on **12 columns** and relies on three main elements:

1. A `.container` (layout wrapper)
2. A `.row` inside the container
3. Column elements inside the row

```html
<div class="container">
  <div class="row">
    <div class="col">Column</div>
    <div class="col">Column</div>
  </div>
</div>
```

By default, Bootstrap distributes space **evenly** across columns.

---

## Responsive Columns

Bootstrap containers and columns are responsive.
Breakpoints are activated using suffixes such as:


![Boostrap Grid Breakpoint](./images/Boostrap%20Breakpoints.png)

### Bootstrap Grid Breakpoints — Practical Mapping

### Bootstrap Grid Breakpoints — Practical Mapping

| Class Suffix | Min Width | Max Width | Typical Devices (mental model) | Notes |
|-------------|-----------|-----------|--------------------------------|-------|
| `col-*` (no suffix) | `≥ 0px` | `< 576px` | Mobile phones (default) | Applies to all sizes unless overridden |
| `col-sm-*` | `≥ 576px` | `< 768px` | Large phones / small screens | First explicit breakpoint |
| `col-md-*` | `≥ 768px` | `< 992px` | Tablets | Common layout shift point |
| `col-lg-*` | `≥ 992px` | `< 1200px` | Laptops / small desktops | Typical desktop layout starts here |
| `col-xl-*` | `≥ 1200px` | `< 1400px` | Desktops | Wider screens |
| `col-xxl-*` | `≥ 1400px` | ∞ | Large desktops / wide screens | No upper bound |


Example:
```html
<div class="col-sm-6 col-lg-3"></div>
```

This means:
- 6 columns on small screens and up
- 3 columns on large screens and up

---

## Sized Columns

You can explicitly control column width as long as the total does not exceed 12.

```html
<div class="col-4"></div>
<div class="col-8"></div>
```

Here, the first column takes 4/12 of the row, the second takes 8/12.

---

## Containers

Bootstrap provides multiple container sizes:

- `.container`
- `.container-sm`
- `.container-md`
- `.container-lg`
- `.container-xl`
- `.container-fluid`

Each container adapts to screen size based on breakpoints.

---

## Reduced Need for Media Queries

Because Bootstrap handles responsiveness through its grid and utilities,
custom media queries are often unnecessary.

However, they are still useful for advanced or custom layouts.

---

## Spacing Utilities

Bootstrap includes spacing helpers using the `m` (margin) and `p` (padding) utilities.

Example:
```html
<div class="mt-3 px-4"></div>
```

---

## Dark Mode

Bootstrap supports dark mode using the `data-bs-theme` attribute:

```html
<html data-bs-theme="dark">
```

This switches all compatible components to dark mode automatically.
