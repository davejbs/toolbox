# CSS — The Cascading Nature of Styles

## 1 — What Does “Cascading” Mean?

CSS stands for **Cascading Style Sheets**.  
“Cascading” means that when several rules apply to the same element, CSS follows an ordered system to decide **which rule wins**.

Imagine it like a waterfall:  
styles at the **bottom** have more priority than those at the top.

```
   Highest level (least priority)
            |
            v
   +------------------+
   |  External file   |
   +------------------+
            |
            v
   +------------------+
   |  Internal <style> |
   +------------------+
            |
            v
   +------------------+
   |   Inline style    |
   +------------------+
            |
            v
   +------------------+
   |  !important rule  |
   +------------------+

   Lower you go → more priority
```

---

## 2 — How CSS Decides What Wins

CSS uses **four main criteria**, always checked in this order:

1. **Position**
2. **Specificity**
3. **Type (Inline / Internal / External)**
4. **Importance (`!important`)**

---

## 2.1 — Position (Source Order)

If two rules have equal power,  
**the last one in the file wins**.

```css
p { color: blue; }
p { color: red; }  /* red wins */
```

---

## 2.2 — Specificity

Specificity measures how *targeted* a selector is.

From **lowest** to **highest**:
- Element selectors → `div`, `p`
- Class  → `.title`
- Attribute →  `[attr]`
- ID selectors → `#main`

```css
p { color: green; }
.article p { color: blue; }
#intro p { color: red; }   /* strongest → wins */
```

---

## 2.3 — Type (Where the style comes from)

Priority from low to high:

1. External stylesheet (`styles.css`)
2. Internal `<style>` block
3. Inline style attribute

```html
<p style="color: orange;">...</p>
```

---

## 2.4 — Importance (`!important`)

`!important` overrides almost everything.

```css
p { color: blue !important; }
```

If multiple rules have `!important`, CSS falls back to specificity and order again.

---

