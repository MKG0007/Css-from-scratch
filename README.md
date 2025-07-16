# Css-from-scratch
# 🌐 CSS Notes – Beginner to Advanced

This repository contains my handwritten and typed notes on **CSS (Cascading Style Sheets)**, structured from **Level 1 to Level 5**, covering everything from basic syntax to layout techniques, animations, and more.

---

## 📚 Topics Covered

### 🟦 Level 1 – CSS Basics

* **What is CSS**: CSS (Cascading Style Sheets) is a language used to describe the style of a document.
* **Syntax**:

  ```css
  h3 {
    color: red; /* color = property, red = value */
  }
  ```
* **Multiple Selectors**:

  ```css
  e1, e2, en {
    property: value;
  }
  ```
* **Types of CSS**:

  1. **Inline CSS** – Written inside the element's opening tag.
  2. **Internal CSS** – Written inside a `<style>` tag in the `<head>`.
  3. **External CSS** – Linked via an external `.css` file.
* **Preference Order**: Inline > Internal > External

#### 🎨 Color Systems

* **RGB**: `rgb(255, 0, 0)` (max value per color = 255)
* **HEX**: `#ff0000` (00-ff range)
* Use color palettes for consistent design.

#### 🔍 Selectors

* Universal: `* {}`
* Class: `.classname {}`
* ID: `#idname {}`
* Element: `tagname {}`

#### 📝 Text Properties

* `text-align: left | right | center`
* `text-decoration: underline | line-through`
* `font-weight: normal | bold | 100–900`
* `font-family: Arial, Italic, Roboto`
* `font-size`, `line-height`, `text-transform`

#### 📏 Units

* **Absolute**: `px`, `cm`, `mm`, `m`

---

### 🟨 Level 2 – Box Model & Display

#### 📦 Box Model

* **Padding**: Space between content and border
* **Border**: Solid line around content
* **Margin**: Space outside the element

#### Border Properties

* `border-color`, `border-width`, `border-style`, `border-radius`
* Shorthand: `border: width style color;`

#### Padding & Margin Shorthand

```css
padding: top right bottom left;
margin: top right bottom left;
```

* Single value applies to all sides equally.

#### 🧱 Display

* `inline`, `block`, `inline-block`, `none`
* `visibility: hidden` (reserves space)
* `display: none` (removes element from flow)

#### 🎨 RGBA

* `rgba(255, 0, 0, 0.75)` – sets color with opacity

---

### 🟩 Level 3 – Relative Units & Positioning

#### 📐 Relative Units

* `%` – Relative to parent size
* `em` – Relative to parent font size
* `rem` – Relative to root font size
* `vh`, `vw` – Relative to viewport height/width

#### 📌 Position Property

* `static` – Default (no positioning)
* `relative` – Relative to itself
* `absolute` – Relative to nearest positioned ancestor
* `fixed` – Relative to browser window
* `sticky` – Sticks based on scroll
* `z-index` – Controls stacking

#### 🌄 Backgrounds

* `background-image: url('path')`
* `background-size: contain | cover`
* `background-repeat: no-repeat`

---

### 🟥 Level 4 – Flexbox & Media Queries

#### 🧰 Flexbox Basics

* One-dimensional layout (row/column)
* `display: flex;`

#### Flex Container Properties

* `flex-direction: row | column | row-reverse | column-reverse`
* `justify-content: flex-start | center | space-between | space-around`
* `align-items: flex-start | center | stretch`

#### Flex Item Properties

* `align-self`, `flex-grow`, `flex-shrink`

#### 📱 Media Queries

```css
@media (max-width: 600px) {
  div {
    background-color: red;
  }
}
```

* Can combine `min-width` and `max-width` for ranges

---

### 🟪 Level 5 – Transitions, Animations & Grid

#### 🔄 Transitions

* `transition-property`, `transition-duration`, `transition-timing-function`, `transition-delay`
* Shorthand:

  ```css
  transition: all 0.3s ease-in-out;
  ```

#### 👆 Pseudo Classes

* `:hover`, `:active`

#### 🎮 Transformations

* `transform: rotate(45deg)`
* `transform: scale(1.5)`
* `transform: translate(50px, 100px)`
* `transform: skew(45deg)`

#### 🌀 Animations

```css
@keyframes slide {
  from { left: 0; }
  to { left: 100px; }
}
```

* Properties: `animation-name`, `animation-duration`, `animation-delay`, `animation-iteration-count`, `animation-direction`
* Use `%` for keyframe stages: `0%`, `50%`, `100%`

#### 🌐 Font Awesome

* Use it for free icons in your websites.

---

### 📐 CSS Grid Layout

* Grid = layout with rows & columns (like Excel)

#### Grid Container Properties

* `display: grid`
* `grid-template-columns`, `grid-template-rows`
* `column-gap`, `row-gap`
* Example: `grid-template-columns: repeat(3, 1fr);`

#### Grid Item Properties

* `grid-column-start`, `grid-column-end`
* `grid-row-start`, `grid-row-end`

---

## ✅ Sample Project

A basic **Amazon Clone** layout using Flexbox and CSS concepts is included in this repo. See the `project` folder for full HTML/CSS code.

---

## 📌 Note

These notes are part of my learning journey and are organized for quick reference and revision.

---

## 🔗 Author

**Mayank Kumar Gupta**
*For queries or collaboration, connect via [LinkedIn](https://www.linkedin.com)*
