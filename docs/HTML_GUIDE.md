# HTML Guide - Complete Reference

## Table of Contents
1. [Introduction](#introduction)
2. [HTML Document Structure](#html-document-structure)
3. [Basic Elements](#basic-elements)
4. [Semantic HTML5](#semantic-html5)
5. [Forms](#forms)
6. [Best Practices](#best-practices)

## Introduction

HTML (HyperText Markup Language) is the standard markup language for creating web pages. It describes the structure of a web page semantically and originally included cues for the appearance of the document.

## HTML Document Structure

Every HTML document should follow this basic structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Page description">
    <title>Page Title</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```

### Key Elements:
- `<!DOCTYPE html>`: Declares HTML5 document type
- `<html>`: Root element
- `<head>`: Contains metadata
- `<body>`: Contains visible content

## Basic Elements

### Headings
```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
<!-- h4, h5, h6 available -->
```

### Paragraphs
```html
<p>This is a paragraph.</p>
```

### Links
```html
<a href="https://example.com">Link Text</a>
<a href="#section">Internal Link</a>
<a href="mailto:email@example.com">Email Link</a>
```

### Images
```html
<img src="image.jpg" alt="Description" width="300" height="200">
```

### Lists

**Unordered List:**
```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>
```

**Ordered List:**
```html
<ol>
    <li>First item</li>
    <li>Second item</li>
</ol>
```

**Description List:**
```html
<dl>
    <dt>Term</dt>
    <dd>Definition</dd>
</dl>
```

## Semantic HTML5

Semantic elements provide meaning to the structure:

```html
<header>Header content</header>
<nav>Navigation links</nav>
<main>Main content</main>
<article>Independent content</article>
<section>Section of content</section>
<aside>Sidebar content</aside>
<footer>Footer content</footer>
```

### Benefits:
- Better SEO
- Improved accessibility
- Clearer code structure
- Better screen reader support

## Forms

### Basic Form Structure:
```html
<form action="/submit" method="POST">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    
    <button type="submit">Submit</button>
</form>
```

### Input Types:
- `text`: Single-line text input
- `email`: Email address
- `password`: Password field
- `number`: Numeric input
- `date`: Date picker
- `checkbox`: Checkbox
- `radio`: Radio button
- `file`: File upload
- `submit`: Submit button

## Best Practices

1. **Use Semantic HTML**: Prefer semantic elements over divs
2. **Accessibility**: Always include alt text for images
3. **Valid HTML**: Ensure your HTML is valid
4. **Indentation**: Use consistent indentation
5. **Comments**: Add comments for complex sections
6. **Meta Tags**: Include proper meta tags for SEO
7. **Language Attribute**: Always specify the lang attribute

## Examples

See the `01-html-kategorisi/` folder for practical examples and exercises.

