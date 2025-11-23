# CSS's Border Properties

## 1 — What Is It?

Every HTML element follows the **CSS box model**:  
**content → padding → border → margin**

The **border** controls the outline around an element.  
You can adjust its **thickness**, **style**, and **color** to shape or highlight elements.

---
## 2 — The `border` Shorthand

```css
selector {
  border: thickness style color;
}
```

**Example**
```css
div {
  border: 10px solid black;
}
```

---

## 3 — Individual Borders

```css
border-top
border-right
border-bottom
border-left
```

**Example**
```css
div {
  border-top: 5px solid red;
  border-right: 3px dashed blue;
  border-bottom: 8px dotted green;
  border-left: 2px solid black;
}
```

---

## 4 — Border Width (including two‑value syntax)

```css
div {
  border-style: solid;
  border-width: 4px;
}
```

Two values:
```css
border-width: 10px 20px;
```
- 10px → top & bottom  
- 20px → left & right  

---

## 5 — Border Style

Common values:
- solid  
- dashed  
- dotted  
- double  
- none  

```css
div {
  border-style: dashed;
}
```

---

## 6 — Border Color

```css
div {
  border-color: red green blue yellow;
}
```

Order: top → right → bottom → left

---

## 7 — Border Radius

```css
/* Slight rounding */
.box {
  border: 1px solid #000;
  border-radius: 8px;
}

/* Circle (requires equal width & height) */
.avatar {
  border: 3px solid #333;
  border-radius: 50%;
}

.oval {
  border-radius: 20px / 8px;
}
```

---
