# Understanding CSS

## What is CSS?

CSS (Cascading Style Sheets) is a styling language that controls how web pages look. It allows us to style elements like colors, spacing, and layout to create clean, consistent, and responsive designs.


## How to Add CSS

There are three main ways to apply CSS to HTML:

### 1) Inline CSS
- Applied **directly** to an HTML element using the `style` attribute  
- Highest priority in most cases  
- Good for quick tests, **not recommended** for full styling

**Example:**
```html
<p style="color: blue;">Blue text</p>
```

### 2) Internal CSS
- Written inside a `<style>` tag in the `<head>` section  
- Useful for small pages or prototypes  
- Not reusable across multiple files

**Example:**
```html
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```

### 3) External CSS (Recommended)
- Stored in a separate `.css` file  
- Best option for organization, scaling, and browser caching  
- Styles can be reused across multiple pages

**Example:**
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

## CSS Selectors
Selectors are used to target specific HTML elements so we can style them. Here are some of the most common ones:

### Element Selector
Targets all elements of the same type.

**Syntax**
```css
h1 {
  color: blue;
}
```

---
### Class Selector
- Targets elements that share the **same class**
- Recommended for most styling (reusable and maintainable)

**Syntax**
```css
.className {
  property: value;
}
```

---
### ID Selector
- Targets a **unique element** by its ID
- Should only be used **once per page**
- Higher specificity than classes

**Syntax**
```css
#uniqueId {
  property: value;
}
```
---

### Attribute Selector
- Targets elements based on **HTML attributes** and/or their values
- Useful for styling forms, links, or specific element states

**Syntax**
```css
selector[attribute="value"] {
  property: value;
}
```
---

### Universal Selector
- Targets **every element** on the page
- Often used for global resets and normalization

**Syntax**
```css
* {
  property: value;
}
```
---

### Descendant Selector (`A B`)
- Targets any element `B` **inside** element `A` (at any level)
- More general than the child selector (`A > B`)

**Syntax**
```css
parent descendant {
  property: value;
}

```
---

### Child Selector (`A > B`)
- Targets **direct children only** inside a parent element
- More specific than a descendant selector (`A B`)

**Syntax**
```css
parent > child {
  property: value;
}
```
---