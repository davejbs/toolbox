# CSS Positioning

CSS provides several ways to position HTML elements on a page.  
Each positioning method affects how an element behaves in the layout.

---

## 1. Static Positioning

This is the **default** position for all elements.  
A static element cannot be moved using `top`, `left`, `right`, or `bottom`.  
It simply appears in the normal document flow, stacking under the previous element.

**Syntax**
```css
element {
  position: static;
}
```

---

## 2. Relative Positioning

The element keeps its **original place** in the normal flow,  
but it can be shifted **relative to that position** using:

- `top`
- `left`
- `right`
- `bottom`

**Syntax**
```css
element {
  position: relative;
  top: 10px;
  left: 20px;
}
```

The surrounding elements still behave as if the element never moved.

---

## 3. Absolute Positioning

The element is removed from the normal flow and positioned **relative to the closest positioned ancestor**  
(the nearest parent with `position: relative`, `absolute`, or `fixed`).

If no such ancestor exists, it positions relative to the **top-left corner of the page**.

**Syntax**
```css
element {
  position: absolute;
  top: 0;
  right: 0;
}
```

---

## 4. Fixed Positioning

The element is positioned relative to the **browser window (viewport)**.  
It stays in the same place even when scrolling.

**Syntax**
```css
element {
  position: fixed;
  bottom: 10px;
  right: 10px;
}
```

Common uses include:  
- Floating chat buttons  
- Back-to-top buttons  
- Sticky utility icons  

---

## Z-Index

`z-index` controls which elements appear **on top** of others.  
It only applies to elements using a positioned value (`relative`, `absolute`, `fixed`).

Higher number → shown above lower ones.

**Syntax**
```css
element {
  position: relative;
  z-index: 10;
}
```
