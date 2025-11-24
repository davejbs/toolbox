# CSS Media Queries

Media queries make a website **responsive**.  
Depending on the device (phone, tablet, laptop, desktop), elements on the page adapt to different screen sizes.

> Media queries help make a site responsive, but other techniques like flexible layouts, Flexbox, Grid  work too.

---

## Basic Syntax

```css
@media (max-width: 600px) {
  /* Styles applied when screen width is 600px or less */
}
```

A media query checks the screen size and applies CSS when the condition is met.

---

## How Breakpoints Work

- **max-width** → applies to screens **equal or smaller** than the value  
- **min-width** → applies to screens **equal or larger** than the value  

­­
> You can also combine two breakpoints : 
Example:
```css
@media (min-width: 600px) and (max-width: 900px) {
  /* Styles for medium screens */
}
```

---

## Common Breakpoint Types

These are commonly used : 

### Mobile Devices

#### Android (common widths)
- 360px  
- 393px  
- 412px  

#### iPhone (common widths)
- iPhone SE → 375px  
- iPhone 12–15 → 390px  
- iPhone Pro Max → 430px  

**Recommended mobile breakpoint**
```css
@media (max-width: 480px) { ... }
```

---

### Tablets
Typical tablet widths:
- 600px  
- 768px (iPad)  
- 834px  
- 1024px  

**Recommended tablet breakpoint**
```css
@media (max-width: 768px) { ... }
```

---

### Laptops & Desktops
Common widths:
- 1024px (small laptop)  
- 1280px  
- 1440px  
- 1600px  
- 1920px+  

**Recommended desktop breakpoint**
```css
@media (min-width: 1024px) { ... }
```

---

## Example: Simple Responsive Layout

```css
/* Desktop (default) */
.container {
  width: 900px;
}

/* Tablet */
@media (max-width: 768px) {
  .container {
    width: 90%;
  }
}

/* Mobile */
@media (max-width: 480px) {
  .container {
    width: 100%;
  }
}
```

---

## Quick Reference Table

| Device Type     | Typical Breakpoint |
|------------------|--------------------|
| Small phones     | 360–400px          |
| iPhones          | 375–430px          |
| Tablets          | 600–768px          |
| Small laptops    | 1024px             |
| Desktops         | 1280–1440px        |
| Large screens    | 1600–1920px        |


## Orientation 

You can also target device orientation directly, for example using (orientation: landscape) without needing @media screen.

```css
@media (orientation: landscape) {
  /* Styles for landscape mode */
}
```