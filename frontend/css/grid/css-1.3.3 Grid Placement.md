# CSS Grid — Placement

## What is it?

Grid allows precise placement of elements inside rows and columns.
Each intersection of a row and a column forms a **cell**.

An element can occupy:
- a single cell
- multiple cells (spanning rows and/or columns)

---

## Grid-column & grid-row

Elements can be placed using `grid-column` and `grid-row`.

### Using span

```css
.item {
  grid-column: span 2;
}
```

This makes the element span across two columns.

---

## Grid-column-start & grid-row-start

Defines where an element starts.

```css# CSS Grid — Placement

## What is it?

Grid allows precise placement of elements inside a two-dimensional layout.
Each intersection of a row and a column forms a **cell**.

An element can:
- occupy a single cell
- span multiple rows or columns
- overlap other elements

This level of control is one of Grid’s main strengths.

---

## grid-column & grid-row

Elements can be positioned using `grid-column` and `grid-row`.

```css
.item {
  grid-column: span 2;
}
```

This makes the element extend across **two adjacent columns**.

In practice, `span` is easier to read than explicit start/end values for simple layouts.

---

## grid-column-start & grid-row-start

These properties define **where placement begins**.

```css
.item {
  grid-column-start: 1;
}
```

> Negative values count from the end of the grid, but they reduce readability and are rarely recommended.

---

## grid-column-end & grid-row-end

These properties define **where placement stops**.

```css
.item {
  grid-column-end: 3;
}
```

Together with the start values, they determine how much space the item occupies.

---

## grid-column / grid-row (shorthand)

Start and end values can be combined:

```css
.item {
  grid-column: 1 / 3;
}
```

This is useful when exact placement matters.

---

## grid-area

The `grid-area` shorthand combines row and column placement into one declaration:

```css
.item {
  grid-area: row-start / column-start / row-end / column-end;
}
```

This syntax becomes especially powerful when used with named grid areas.

---

## Overlapping Elements

Unlike Flexbox, Grid allows elements to **overlap naturally**.

When overlapping elements, transparency helps visualize stacking order:

```css
.item {
  background-color: rgba(255, 0, 0, 0.5);
}
```

Overlaps should be used deliberately, as they can impact readability.

  grid-column-start: 1;
}
```

> Negative values count from the end but are generally **not recommended** for readability.

---

## Grid-column-end & grid-row-end

Defines where an element ends.

```css
.item {
  grid-column-end: 3;
}
```

---

## Grid-column / grid-row (shorthand)

Combines start and end values:

```css
.item {
  grid-column: 1 / 3;
}
```

---

## Grid-area

Combines row and column placement into one declaration:

```css
.item {
  grid-area: row-start / column-start / row-end / column-end;
}
```

---

## Overlaying Elements

Unlike Flexbox, Grid allows elements to **overlap**.

To make overlaps visible, transparency is often used:

```css
.item {
  background-color: rgba(255, 0, 0, 0.5);
}
```
