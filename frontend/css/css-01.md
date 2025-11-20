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

