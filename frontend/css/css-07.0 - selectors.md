
# CSS Selectors
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
* You can apply multiple classes to an element 

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
