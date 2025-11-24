# CSS Float

The `float` property lets an element move to the left or right so other content can wrap around it. Images are a common example, but floats work with any block‑level element.

---

## 1. Float Left

Moves the element to the **left**, and text wraps around it on the **right**.

**Syntax**
```css
img {
  float: left;
}
```

---

## 2. Float Right

Moves the element to the **right**, and text wraps on the **left**.

**Syntax**
```css
img {
  float: right;
}
```
---

## 3. Float None 
This is useful when you want an element to return to the normal document flow, especially in responsive layouts where floats can break the structure on smaller screens.

**Syntax**
```css
img {
  float: none;
}
```
---

## 4. Clear

`clear` tells an element to **ignore previous floats** so it won’t wrap next to them.  
This is commonly used for elements like footers that must appear **below** floated content.

Possible values:  
- `left`  
- `right`  
- `both`

**Syntax**
```css
footer {
  clear: both;
}
```

> `clear` must be applied **on the element that needs to avoid floats**, not on the floated element.

