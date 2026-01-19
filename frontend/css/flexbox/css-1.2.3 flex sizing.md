# CSS Flex — Flex Sizing

## What is it?

Flexbox sizing follows a **priority order** that determines how space is distributed.
Understanding this order is critical for predicting layout behavior.

---

## Sizing Priority Order (lowest → highest)

```
Content size < width < flex-basis < min-width / max-width
```

---

## Content Size

The default size of an element based solely on its content.

---

## Width

Defines a fixed size for a flex item.

**Syntax**
```css
.item {
  width: 200px;
}
```

---

## Min-width

Defines the **minimum size** an element can shrink to.

**Syntax**
```css
.item {
  min-width: 150px;
}
```

The element will never become smaller than this value.

---

## Max-width

Defines the **maximum size** an element can grow to.

**Syntax**
```css
.item {
  max-width: 300px;
}
```

The element will never exceed this value.

---

## Flex-basis

Defines the **initial size of a flex item along the main axis**.
The default value is `auto`.

**Syntax**
```css
.item {
  flex-basis: 0;
}
```

Setting `flex-basis: 0` disables content-based sizing and allows pure flex distribution.

---

## Flex-grow

Controls how much an item **can grow** relative to other items.

**Syntax**
```css
.item {
  flex-grow: 1;
}
```

- `0` → item cannot grow
- `1` → item can grow

---

## Flex-shrink

Controls how much an item **can shrink** relative to other items.

**Syntax**
```css
.item {
  flex-shrink: 0;
}
```

- `0` → item cannot shrink
- `1` → item can shrink

---

## Flex Shorthand

Flex properties can be combined using shorthand syntax:

```css
.item {
  flex: grow shrink basis;
}
```

**Example**
```css
.item {
  flex: 1 1 0;
}
```

