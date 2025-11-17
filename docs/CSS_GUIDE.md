# CSS Guide - Complete Reference

## Table of Contents
1. [Introduction](#introduction)
2. [CSS Syntax](#css-syntax)
3. [Selectors](#selectors)
4. [Box Model](#box-model)
5. [Layout](#layout)
6. [Responsive Design](#responsive-design)
7. [Best Practices](#best-practices)

## Introduction

CSS (Cascading Style Sheets) is used to style and layout web pages. It controls colors, fonts, spacing, and positioning.

## CSS Syntax

```css
selector {
    property: value;
    property: value;
}
```

### Example:
```css
h1 {
    color: blue;
    font-size: 24px;
}
```

## Selectors

### Basic Selectors:
```css
/* Element selector */
p { color: red; }

/* Class selector */
.class-name { color: blue; }

/* ID selector */
#id-name { color: green; }

/* Universal selector */
* { margin: 0; }
```

### Combinators:
```css
/* Descendant */
div p { color: red; }

/* Child */
div > p { color: blue; }

/* Adjacent sibling */
h1 + p { color: green; }

/* General sibling */
h1 ~ p { color: orange; }
```

### Pseudo-classes:
```css
a:hover { color: red; }
a:active { color: blue; }
a:visited { color: purple; }
input:focus { border: 2px solid blue; }
```

## Box Model

Every element is a box with:
- **Content**: The actual content
- **Padding**: Space inside the element
- **Border**: Border around padding
- **Margin**: Space outside the element

```css
.box {
    width: 300px;
    padding: 20px;
    border: 2px solid black;
    margin: 10px;
    box-sizing: border-box; /* Includes padding and border in width */
}
```

## Layout

### Flexbox:
```css
.container {
    display: flex;
    justify-content: center; /* Horizontal alignment */
    align-items: center; /* Vertical alignment */
    flex-direction: row; /* or column */
    flex-wrap: wrap;
}

.item {
    flex: 1; /* Grow and shrink */
}
```

### Grid:
```css
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 20px;
}

.item {
    grid-column: span 2;
    grid-row: span 1;
}
```

## Responsive Design

### Media Queries:
```css
/* Mobile first approach */
.container {
    width: 100%;
}

/* Tablet */
@media (min-width: 768px) {
    .container {
        width: 750px;
    }
}

/* Desktop */
@media (min-width: 1024px) {
    .container {
        width: 1200px;
    }
}
```

### Viewport Meta Tag:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## CSS Variables

```css
:root {
    --primary-color: #6366f1;
    --spacing: 1rem;
}

.element {
    color: var(--primary-color);
    padding: var(--spacing);
}
```

## Best Practices

1. **Use CSS Variables**: For consistent theming
2. **Mobile First**: Design for mobile, then scale up
3. **Organize Code**: Group related styles
4. **Use Shorthand**: `margin: 10px 20px;` instead of separate properties
5. **Avoid Inline Styles**: Use external stylesheets
6. **Performance**: Minimize CSS, use efficient selectors
7. **Naming Conventions**: Use consistent naming (BEM, etc.)

## Examples

See the `02-css-kategorisi/` folder for practical examples and exercises.

