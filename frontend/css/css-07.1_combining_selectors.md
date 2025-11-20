# Combining Selectors

It is possible to combine selectors to target elements more precisely or apply the same rule to multiple elements.

Below are the main ways to combine them.

---

## 1 — Grouping Selectors (`,`)

Used to apply the **same style** to different selectors.

**Syntax**
```css
selector1,
selector2,
selector3 {
  property: value;
}
```

---

## 2 — Child Selector (`A > B`)

Targets elements that are **direct children only** of a parent — exactly **one level** below.

**Syntax**
```css
parent > child {
  property: value;
}
```

---

## 3 — Descendant Selector (`A B`)

Matches an element at **any depth** inside another element.

**Syntax**
```css
ancestor descendant {
  property: value;
}
```

---

## 4 — Chaining (no spaces)

Combines multiple conditions on the **same element**.  
Used to increase precision/specificity.

**Syntax**
```css
element#id.class[attr="value"] {
  property: value;
}
```

**Example**
```css
h1#title.big.heading {
  color: purple;
}
```

---

## 5 — Combining Combiners

You can mix different selector types together.  
Less common, but completely valid.

**Example (HTML)**
```html
<ul>
  <p class="done">Other items</p>
</ul>
```

**Example (CSS)**
```css
ul p.done {
  font-size: 0.5rem;
}
```

This matches a `<p>` element with class `"done"` inside a `<ul>`, no matter the nesting depth.
