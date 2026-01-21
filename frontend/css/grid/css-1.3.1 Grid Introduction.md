# CSS Grid — Introduction

## What is it?

CSS Grid is a layout system, similar to Flexbox, designed to create **grid-based layouts**.
Unlike Flexbox, which works along a single axis (row *or* column), Grid operates on **two axes at the same time**:
- rows
- columns

This two-dimensional approach makes Grid especially suitable for **structured page layouts** such as dashboards,
galleries, or full-page designs.

> A grid container must be placed inside another element (for example `body`, `html`, or a wrapper `div`).
> Viewport units (`vw`, `vh`) are commonly used to size the grid relative to the screen.

---

## Display Mode

Grid introduces its own display mode:

```css
.container {
  display: grid;
}
```

Once an element becomes a grid container, all of its direct children turn into **grid items**.

---

## Responsive Behavior

In practice, Grid layouts tend to remain **visually stable** when the viewport changes.
Rows and columns keep their relative positions, which makes Grid easier to reason about for complex layouts
compared to Flexbox.

This is why Grid is often preferred for **overall page structure**, while Flexbox is used for local alignment.

---

## How Grid Works

### grid-template-rows & grid-template-columns

These properties define the number and size of rows and columns explicitly.

> Grid does not guess your structure — you must describe it.

**Example**
```css
.container {
  display: grid;
  grid-template-rows: 1fr 1fr;        /* two horizontal tracks */
  grid-template-columns: 1fr 1fr 1fr; /* three vertical tracks */
}
```

Here, the grid is divided into **six cells** (2 × 3), each sized proportionally.

---

### grid-template (shorthand)

The `grid-template` shorthand combines rows and columns in a single declaration:

```css
.container {
  display: grid;
  grid-template: 1fr 1fr / 1fr 1fr 1fr; /* rows / columns */
}
```

This syntax is shorter, but the long-form version is often clearer and easier to read when learning Grid.
