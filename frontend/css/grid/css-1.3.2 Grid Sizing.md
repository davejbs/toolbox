# CSS Grid — Sizing

## What is it?

Grid sizing controls how rows and columns **take space** inside the grid container.
Instead of relying on content alone, Grid lets you define clear sizing rules.

Understanding sizing is essential, because most Grid layout issues come from **misunderstood track sizes**.

---

## Common Grid Units

| Unit / Function | Description |
|-----------------|-------------|
| `px` | Fixed size that does not adapt to screen changes |
| `rem` | Relative to the root font size, useful for scalable layouts |
| `auto` | Size is based on content and available space |
| `fr` | Fractional unit that distributes remaining free space |
| `minmax(min, max)` | Defines a size range for a track |
| `repeat(n, value)` | Repeats a track definition to reduce repetition |

---

## The `fr` Unit (Important)

The `fr` unit represents a **fraction of the available space**.

Instead of setting fixed dimensions, `fr` allows the browser to distribute leftover space dynamically.
This is especially useful when you want columns or rows to resize **relative to each other**, not to the viewport.

In practice, `fr` makes layouts more flexible and easier to maintain.

---

## minmax(min, max)

The `minmax()` function defines **boundaries** for a track.

It allows a column or row to grow and shrink within safe limits.
This prevents elements from becoming too small or excessively large as the viewport changes.

```css
.container {
  grid-template-columns: minmax(150px, 1fr);
}
```

---

## Implicit Tracks

If there are **more grid items than explicitly defined tracks**, Grid creates additional tracks automatically.
These are called *implicit tracks*.

To control their size, use:
- `grid-auto-rows`
- `grid-auto-columns`

```css
.container {
  grid-auto-rows: 150px;
}
```

Without these properties, implicit tracks can lead to unexpected sizing behavior.
