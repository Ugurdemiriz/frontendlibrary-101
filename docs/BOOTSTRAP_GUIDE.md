# Bootstrap Guide - Complete Reference

## Table of Contents
1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Grid System](#grid-system)
4. [Components](#components)
5. [Utilities](#utilities)
6. [Best Practices](#best-practices)

## Introduction

Bootstrap is a popular CSS framework for building responsive, mobile-first websites. It provides pre-built components and a powerful grid system.

## Getting Started

### CDN Link:
```html
<!-- CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- JavaScript -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

## Grid System

Bootstrap uses a 12-column grid system:

```html
<div class="container">
    <div class="row">
        <div class="col-md-6">Half width on medium+</div>
        <div class="col-md-6">Half width on medium+</div>
    </div>
</div>
```

### Breakpoints:
- `xs`: < 576px (default)
- `sm`: ≥ 576px
- `md`: ≥ 768px
- `lg`: ≥ 992px
- `xl`: ≥ 1200px
- `xxl`: ≥ 1400px

### Examples:
```html
<!-- Equal columns -->
<div class="row">
    <div class="col">Column 1</div>
    <div class="col">Column 2</div>
    <div class="col">Column 3</div>
</div>

<!-- Responsive columns -->
<div class="row">
    <div class="col-12 col-md-6 col-lg-4">Responsive</div>
</div>
```

## Components

### Buttons:
```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-outline-primary">Outline</button>
```

### Cards:
```html
<div class="card">
    <div class="card-body">
        <h5 class="card-title">Title</h5>
        <p class="card-text">Content</p>
    </div>
</div>
```

### Navigation:
```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
        <a class="navbar-brand" href="#">Brand</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                </li>
            </ul>
        </div>
    </div>
</nav>
```

### Forms:
```html
<form>
    <div class="mb-3">
        <label for="email" class="form-label">Email</label>
        <input type="email" class="form-control" id="email">
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
</form>
```

## Utilities

### Spacing:
```html
<div class="m-3">Margin all sides</div>
<div class="p-4">Padding all sides</div>
<div class="mt-2">Margin top</div>
<div class="mb-3">Margin bottom</div>
```

### Display:
```html
<div class="d-none">Hidden</div>
<div class="d-block">Block</div>
<div class="d-flex">Flex</div>
<div class="d-md-none">Hidden on medium+</div>
```

### Text:
```html
<p class="text-center">Centered</p>
<p class="text-primary">Primary color</p>
<p class="fw-bold">Bold</p>
<p class="text-muted">Muted</p>
```

## Best Practices

1. **Use Container**: Always wrap content in `.container` or `.container-fluid`
2. **Mobile First**: Design for mobile, then enhance for larger screens
3. **Customize**: Override Bootstrap styles with custom CSS
4. **Components**: Use Bootstrap components as starting points
5. **Accessibility**: Ensure proper ARIA labels and semantic HTML
6. **Performance**: Only include needed Bootstrap components

## Examples

See the `03-bootstrap-kategorisi/` folder for practical examples and exercises.

