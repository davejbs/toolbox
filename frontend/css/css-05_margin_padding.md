# Margin & Padding

## 1 — What Are They?

HTML elements follow the **CSS box model**:  
**content → padding → border → margin**

**Padding** controls the **inner space** (inside the border).  
**Margin** controls the **outer space** (outside the border).  
Both are key for spacing and layout.

---

# 2 — Margin

### What it does ?
`margin` sets the space **outside** the element’s border.

---

### Margin Syntax

#### 1) Single value
```css
margin: 20px;   /* all sides */
```

#### 2) Two values
```css
margin: 10px 20px;
/* 10px → top & bottom
   20px → left & right */
```

#### 3) Three values
```css
margin: 10px 20px 30px;
/* top → right/left → bottom */
```

#### 4) Four values
```css
margin: 10px 20px 30px 40px;
/* top → right → bottom → left */
```

#### Individual sides
```css
margin-top: 10px;
margin-right: 20px;
margin-bottom: 30px;
margin-left: 40px;
```

---

# 3 — Padding

### What it does
`padding` sets the space **inside** the border, between content and border.

---

### Padding Syntax

#### 1) Single value
```css
padding: 20px;
```

#### 2) Two values
```css
padding: 10px 20px;
```

#### 3) Three values
```css
padding: 10px 20px 30px;
```

#### 4) Four values
```css
padding: 10px 20px 30px 40px;
```

#### Individual sides
```css
padding-top: 10px;
padding-right: 20px;
padding-bottom: 30px;
padding-left: 40px;
```

---

# Visualization

```
          [ MARGIN ]
   +----------------------+
   |      [ BORDER ]      |
   |  +----------------+  |
   |  |   [ PADDING ] |   |
   |  |  +-----------+|   |
   |  |  | CONTENT   ||   |
   |  |  +-----------+|   |
   |  +----------------+  |
   +----------------------+
```
