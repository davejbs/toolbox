# CSS Flex — Flex Direction

The `flex-direction` property defines the **direction in which flex items are laid out** inside a flex container.
By default, Flexbox uses a **row-based layout**.

Flexbox positioning relies on two axes:
- **Main axis**: the primary direction of item flow
- **Cross axis**: perpendicular to the main axis

---

## Flex-direction: row (default)

Items are laid out **horizontally**, from left to right.
The **main axis** runs horizontally.

**Syntax**
```css
.container {
  display: flex;
  flex-direction: row;
}
```

---

## Flex-direction: row-reverse

Same as `row`, but the order of items is reversed.

**Syntax**
```css
.container {
  display: flex;
  flex-direction: row-reverse;
}
```

---

## Flex-direction: column

Items are stacked **vertically**, from top to bottom.
The **main axis** becomes vertical.

**Syntax**
```css
.container {
  display: flex;
  flex-direction: column;
}
```

---

## Flex-direction: column-reverse

Same as `column`, but the order of items is reversed.

**Syntax**
```css
.container {
  display: flex;
  flex-direction: column-reverse;
}
```

---

## Why are the main axis and cross axis important?

Many Flexbox properties and layouts depend on the **direction of the main axis**.

Example:
- `flex-basis` controls the **size of an item along the main axis**
- Changing `flex-direction` changes whether `flex-basis` affects width or height

