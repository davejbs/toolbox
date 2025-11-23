# CSS Display

The `display` property controls how an element behaves in the page layout.  
It affects whether elements stack, sit next to each other, or if they can be resized.

Here are the 4 display types you’ll use the most.

---

## 1. Block

A block element:

- Always starts on a **new line**
- Takes the **full width** available
- Stacks vertically with other block elements
- Lets you change its width and height

**Syntax**
```css
element {
  display: block;
}

```

**Visual Example**
```
+-----------+
| Block 1   |
+-----------+

+-----------+
| Block 2   |
+-----------+

+-----------+
| Block 3   |
+-----------+
```

---

## 2. Inline

An inline element:

- Sits **next to other inline elements**
- Only uses the space it needs
- Cannot be resized with width or height
- Does not force a line break

**Syntax**
```css
element {
  display: inline;
}
```

**Visual Example**
```
[Inline1][Inline2][Inline3]
```

---

## 3. Inline-Block

Inline-block is basically a mix of block and inline:

- Elements stay **on the same line**
- But can still be resized
- Great for buttons, badges, small layout boxes, etc.

**Syntax**
```css
element {
  display: inline-block;
}
```

**Visual Example**
```
+---------+    +-------------------+    +----------+
| Box 1   |    |       Box 2       |    |  Box 3   |
| short   |    |   taller element  |    | medium   |
+---------+    |   more content    |    +----------+
                +-------------------+
```

---

## 4. None

This removes the element completely:

- It’s not shown
- It doesn’t take any space
- Useful for hiding list items, buttons, or anything you want to toggle on/off

**Syntax**
```css
element {
  display: none;
}
```
