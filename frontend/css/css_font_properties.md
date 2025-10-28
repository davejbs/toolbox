# CSS's Font Properties

> Note: This is **not an exhaustive list**

##  What is it?

The `font*` properties control the visual appearance of **text**: typeface, size, weight (thickness), style (italic/oblique), variants (small caps, tabular numbers), stretching, etc.  



## Font-Size

The `font-size` property controls the **displayed size** of text inside an element.

**Syntax**
```css
p{
    font-size: value
}
```

***Possible values***


| Value | Meaning                                     | Reference Size          | Pros                                       | Cons                                  |
| ----- | ------------------------------------------- | ----------------------- | ------------------------------------------ | ------------------------------------- |
| `px`  | Absolute pixel size                         | `1px ≈ 1/96in ≈ 0.26mm` | Very precise and consistent                | Not accessible or scalable            |
| `pt`  | Print typography point                      | `1pt ≈ 1/72in ≈ 0.35mm` | Standard for print                         | Not recommended for web UI            |
| `em`  | Relative to the **parent** font-size        | `1em = 100% of parent font-size (commonly 16px)`  | Scales with its container                  | Can compound and become hard to track |
| `rem` | Relative to the **root** (`html`) font-size | `1rem = 100% of root`   | Best for consistent and accessible scaling | Does not adapt to parent elements     |


## Font-Weight

The `font-weight` property controls the **thickness (boldness)** of the text.  
It can be defined using **keywords**, **numeric values**, or **relative values** based on a parent.

**Syntax**
```css
p {
  font-weight: value;
}
```

 ***Possible Values***

| Value Type            | Examples              | Meaning / Behavior                           | Notes                                                              |
| --------------------- | --------------------- | -------------------------------------------- | ------------------------------------------------------------------ |
| **Keyword**           | `normal`, `bold`      | Standard weights (typically `400` and `700`) | Easiest to read and commonly used                                  |
| **Numeric (100–900)** | `100`, `200`, … `900` | Allows fine control of thickness             | Depends on font availability  not every font supports all weights |
| **Relative**          | `bolder`, `lighter`   | Adjusts compared to the parent's weight      | Browser-calculated  can vary depending on context                 |

---

## Font-Family

Specifies the **typeface stack** used to render text. Always provide a **primary font** followed by **fallbacks**, and end with a **generic family**. You can also load a **custom font** (see `@css_custom_font_family.md`).


**Syntax**
```css
p {
  font-family: typeface,backup_generic_font_type;
}
```
**If the font has many words**

```css
p {
  font-family: "Primary Font Name", "Fallback Name", generic-family;
}

```
***Possible values***


| Type | Example(s) | Notes |
|------|------------|------|
| Custom font files | `"Inter"`, `"Poppins"` | Must be loaded via `@font-face` or a web font provider |
| System fonts | `"Segoe UI"`, `Roboto`, `Helvetica`, `Arial` | Fast and optimized for UI |
| Monospace | `"Fira Code"`, `"Roboto Mono"`, `Courier New` | For code or fixed-width text |
| Generic families | `serif`, `sans-serif`, `monospace`, `cursive` | Always include one as fallback |

> There are many other font families, choose based on your design needs and font availability.
