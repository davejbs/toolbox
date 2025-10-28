# Understanding HTML

## 1. What is it?
**HTML (HyperText Markup Language)** is the standard language for structuring content on the web.  

It provides the **structure** and defines elements like headings, paragraphs, links, images, and forms, forming the foundation of every webpage. 

## 2. HTML File Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">    <!-- Character encoding -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">    <!-- Mobile-friendly scaling -->
    <title>Document</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>

```
---
## Most used Tags

### For Text Formatting
- `<h1> - <h6>` : Heading Element
- `<p>` : Paragraph Element
- `<br/>` : Line Break
- `<hr/>` : Horizontal rule
- `<strong>` : Bold Text
- `<em>` : Emphasis / Intonation

### Links
- `<a>`: Anchor (Hyperlink)

    **Attributes**
    - `href` : URL Destination
    - `target` : _self(same tab), _blank(new tab)

### Images
- `img` : Images

    **Attributes**
    - `src` : Image source
    - `alt` : Atlernative Text
    - `width, height` : Image's dimensions

### Lists
- `<ol>` : Ordered List
- `<ul>` : Unordered List

    **Attributes**
    - `start` : Sets the first item's number
    - `reversed` : Counts down instead of up
    - `type: (1,a, A,i,I) ` : Numbering style