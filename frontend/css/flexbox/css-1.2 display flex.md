# CSS Display Flex

`display: flex` is a layout method used to arrange elements more easily.  
To use it, you wrap the elements you want to control inside a **container**, then apply `display: flex` (and usually a `gap`) to that container.

- Flex changes how the **children** behave by turning them into flex items.  
  Their usual block/inline behavior doesn’t matter anymore.
- By default, items take **only the space they need**, unless you allow them to stretch using properties like `flex-grow`.

>  Flex only affects the **direct children** of the container.

---

## 1. `display: flex`

The regular flex container:

- Acts like a block element  
- Takes the full available width  
- Places items on one line unless you enable wrapping

**Syntax**
```css
.container {
  display: flex;
  gap: 1rem;
}
```

---

## 2. `display: inline-flex`

Same flex behavior for the children, but:

- The container behaves like an inline element  
- It only takes up the space it actually needs

**Syntax**
```css
.container {
  display: inline-flex;
  gap: 1rem;
}
```
