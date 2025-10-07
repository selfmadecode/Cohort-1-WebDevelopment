# HTML and CSS Naming Conventions

This document defines the **naming conventions** and **best practices** for writing clean, scalable, and maintainable HTML and CSS code.

---

##  HTML Naming Conventions

### 1. General Rules
- Use **lowercase letters** only.
- Use **hyphens (`-`)** to separate words — *not underscores or camelCase*.
- Choose **meaningful, descriptive** names that convey purpose or content.
- Avoid using **presentational names** (like `red-box` or `big-text`).

 **Good Example:**
```html
<div class="main-header"></div>
<div class="user-profile"></div>
```

 **Bad Example:**
 ```html
<div class="MainHeader"></div>
<div class="red-box"></div>
```

## 2. ID Naming

Use IDs only for unique elements (e.g., <header>, <footer>, <main>).

Prefix IDs with the section or component name if necessary.

Avoid using IDs for styling — prefer classes.

✅ Good Example:
```html
<section id="hero-section"></section>
```

```html
<div id="blue-button"></div>
```

### 3. Class Naming (BEM Methodology)

Follow the BEM (Block-Element-Modifier) convention:

.block {}
.block__element {}
.block--modifier {}
```html
<article class="card card--featured">
  <h2 class="card__title">Article Title</h2>
  <p class="card__description">Description text here.</p>
</article>
```

Block → Standalone component (e.g., card, menu)

Element → Part of a block (e.g., card__title)

Modifier → Variation or state (e.g., card--featured)

CSS Naming Conventions
1. File Organization

Group styles by component or feature.

Use lowercase and hyphens for filenames.

✅ Example:
/css/
  ├── base.css
  ├── layout.css
  ├── components/
  │    ├── button.css
  │    └── card.css
  └── utilities.css


2. Variable Naming (CSS Custom Properties)

Use --kebab-case for variable names.

Prefix variables with a namespace if part of a specific component.

✅ Example:
:root {
  --color-primary: #007bff;
  --font-size-base: 16px;
}

.card {
  --card-padding: 1rem;
  padding: var(--card-padding);
}


https://stackoverflow.com/questions/1790455/whats-the-best-way-to-name-ids-and-classes-in-css-and-html



https://www.w3.org/QA/Tips/goodclassnames