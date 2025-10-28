# A Few Styling Properties
> Note: This is **not an exhaustive list**

## Font Formatting
- `font-size`: Controls text size.
  
  **Values**
  - Absolute: `px` (e.g., `16px`)
  - Relative: `rem`, `em`, `%`
  - Fluid: `clamp(min, preferred, max)`

- `font-weight`: Sets text thickness.
  
  **Values**
  - Keywords: `normal`, `bold`, `bolder`, `lighter`
  - Numeric: `100`–`900` (e.g., `400`, `700`)

- `font-family`: Chooses the typeface stack.
  
  **Values**
  - Named + fallback: `"Inter", system-ui, sans-serif`
  - Generic families: `serif`, `sans-serif`, `monospace`

- `line-height`: Controls line spacing.
  
  **Values**
  - Unitless number (recommended): `1.4`, `1.6`
  - Length/percent: `24px`, `150%`

- `letter-spacing`: Adjusts spacing between characters.
  
  **Values**
  - Length: `0.02em`, `1px`, `normal`

---

## Color & Background
- `color`: Text color.
  
  **Values**
  - `#hex`, `rgb()`, `hsl()`, `currentColor`

- `background-color`: Element background.
  
  **Values**
  - `#hex`, `rgb()`, `hsl()`, `transparent`

- `background-image`: Background image or gradient.
  
  **Values**
  - `url("/path/img.jpg")`, `linear-gradient(...)`, `radial-gradient(...)`

- `background-size`: How the background is fit.
  
  **Values**
  - `cover`, `contain`, `auto`, `<length> <length>`

- `opacity`: Overall transparency.
  
  **Values**
  - `0` (transparent) → `1` (opaque)

---

## Box Model
- `width` / `height`: Element size.
  
  **Values**
  - `auto`, `px`, `%`, `rem`, `min()`, `max()`, `clamp()`

- `margin`: Outer spacing.
  
  **Values**
  - Shorthand: `margin: 16px;`
  - Axis: `margin: 8px 16px;`
  - Sides: `margin: 4px 8px 12px 16px;`

- `padding`: Inner spacing.
  
  **Values**
  - Same shorthands as `margin`

- `border`: Border width/style/color.
  
  **Values**
  - Shorthand: `1px solid #e5e7eb`
  - Styles: `solid`, `dashed`, `dotted`, `none`

- `border-radius`: Corner rounding.
  
  **Values**
  - `8px`, `50%` (circle), elliptical `a / b`

- `box-shadow`: Drop shadow.
  
  **Values**
  - `<x> <y> <blur> <spread> <color>` (e.g., `0 6px 18px rgba(0,0,0,.06)`)

---

## Layout & Display
- `display`: Layout mode.
  
  **Values**
  - `block`, `inline`, `inline-block`, `flex`, `grid`, `none`

- `position`: Positioning scheme.
  
  **Values**
  - `static`, `relative`, `absolute`, `fixed`, `sticky`

- `top` / `right` / `bottom` / `left`: Offsets for non-static positioned elements.
  
  **Values**
  - Lengths or percentages: `0`, `16px`, `10%`

- `z-index`: Stacking order (when positioned).
  
  **Values**
  - Integers: `0`, `10`, `1000` …

- `overflow`: What happens when content overflows.
  
  **Values**
  - `visible`, `hidden`, `scroll`, `auto`

---

## Text & Decoration
- `text-align`: Inline content alignment.
  
  **Values**
  - `left`, `right`, `center`, `justify`, `start`, `end`

- `text-decoration`: Underlines/lines.
  
  **Values**
  - `none`, `underline`, `line-through`, `overline`
  - Extras: `text-underline-offset`, `text-decoration-thickness`

- `text-transform`: Case transformation.
  
  **Values**
  - `none`, `uppercase`, `lowercase`, `capitalize`

---

For more CSS properties and detailed documentation, reference:   https://developer.mozilla.org/en-US/docs/Web/CSS/Reference
