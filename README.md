# CSS Notes

## -------------------LEVEL-1-------------------

### CSS (Cascading Style Sheets)
It is a language used to describe the style of a document.

**Basic syntax:**
```css
h3 { /* h3 is the selector. */
    color: red;
}
```
`color` = property and `red` = value

We can also assign one property to multiple elements using this method:
```css
e1, e2, en {
    property;
}
```

**Three methods of applying CSS to HTML:**
1. **Inline CSS**  
   Written in the opening tag of the element where CSS is applied.

2. **Style Tag CSS**  
   Written inside the `<head>` tag.

3. **External CSS**  
   Written in a separate file made for CSS and linked to the HTML file.

**Note:**  
Preference order: `Inline CSS` > `Style Tag CSS` > `External CSS`  
In case of conflicts, later CSS has higher importance.

---

### Color System
You can set color by name, but many colors have no names.

**RGB Color System:**  
Red, Green, and Blue are the three primary colors.  
Example: `rgb(255, 0, 0);` (Max value = 255)

**HEX (Hexadecimal) Color System:**  
Short form to set RGB values.  
Example: `#ff0000` → (Red: FF, Green: 00, Blue: 00)

**Note:**  
For better design, use a color palette instead of random colors.

---

### Selectors
- **Universal Selector:** `* {}` - Applies CSS to the whole document.
- **Class Selector:** `.className {}` - Applies to multiple elements with the same class.
- **Element Selector:** `elementName {}` - Applies to elements by tag name.
- **ID Selector:** `#idName {}` - Applies to a single, uniquely identified element.

---

### Text Properties
- **text-align:** `right | left | center`  
  Aligns text based on the parent container.
- **text-decoration:** `underline | line-through`  
  Underlines or removes underline from text.
- **font-weight:** `normal | bold | bolder | lighter`  
  Value range: 100–900
- **font-family:** Sets the font style.  
  Example: `font-family: Arial, Italic, Roboto;`
- **font-size:** Sets text size.
- **line-height:** Sets spacing between lines.
- **text-transform:** `uppercase | lowercase | capitalize`

---

### Units in CSS
Two types of units:
1. **Absolute:**  
   - px (96px = 1 inch)  
   - cm, mm, m

---

## --------------------LEVEL-2--------------------

### Box Model in CSS
CSS boxes have 3 areas:
1. **Padding** – Space between content and border.
2. **Border** – The line after padding.
3. **Margin** – Space between elements.

**Border Properties:**
- color, width, style, radius

**Shorthand:**
```css
border: width style color;
```

**Padding Shorthand:**
```css
padding: top right bottom left;
```

**Margin Shorthand:**
```css
margin: top right bottom left;
```

**Note:**  
To create circles, use a square box with `border-radius: 50%`.

---

### Display Property
- **inline:** Takes only necessary space. Cannot set width/margin/padding.
- **block:** Takes full width.
- **inline-block:** Like inline, but allows margin/padding.
- **none:** Removes element from flow.

**Visibility vs Display:**
- `visibility: hidden` hides element but reserves space.
- `display: none` removes element and space.

**RGBA Color System:**
Adds alpha (opacity).  
Example: `rgba(255, 0, 0, 0.75)`

---

## -------------------LEVEL-3-------------------

### Relative Units
1. **% (percent):** Based on parent size.
2. **em:** Based on parent font size.
3. **rem:** Based on root element font size.
4. **vh:** Viewport height.
5. **vw:** Viewport width.

---

### Position Property
Defines element position:
1. `static` – Default.
2. `relative` – Relative to itself.
3. `absolute` – Relative to the nearest positioned ancestor.
4. `fixed` – Relative to browser window.
5. `sticky` – Based on scroll position.

**z-index:**  
Defines stacking order.  
Higher value = above.

---

### Background Image
```css
background-image: url("path");
background-size: cover; /* contain, auto */
background-repeat: no-repeat;
```

---

## -------------------LEVEL-4-------------------

### Flexbox (Flexible Box Layout)
One-dimensional layout method (row/column).

**Flex Container:** Parent of flex items.  
- Main axis: horizontal  
- Cross axis: vertical

**Container Properties:**
- `display: flex`
- `flex-direction: row | column | reverse`
- `justify-content: flex-start | center | space-between`
- `align-items: flex-start | center`

**Item Properties:**
- `align-self`
- `flex-grow`
- `flex-shrink`

**Note:**  
Items stay in container unless content exceeds it.

---

### Media Queries
Used for responsive design.
```css
@media (width: 600px) {
    div {
        background-color: red;
    }
}

@media (min-width: 360px) and (max-width: 600px) {
    /* styles */
}
```

---

## -------------------LEVEL-5-------------------

### Transitions
```css
transition-property: property;
transition-duration: time;
transition-timing-function: ease;
transition-delay: time;
```
**Shorthand:**  
`transition: property duration timing-function delay;`

---

### Pseudo Classes
```css
element:hover { /* on mouse hover */ }
element:active { /* when clicked */ }
```

---

### CSS Transforms
- `rotate(deg)`
- `scale(x, y)`
- `translate(x, y)`
- `skew(deg)`

**Note:**  
Apply to both container and content.  
Rotation may make elements invisible due to axis position.

---

### Animations
```css
@keyframes myAnimation {
    from { ... }
    to { ... }
}

animation-name: myAnimation;
animation-duration: 2s;
animation-delay: 1s;
animation-iteration-count: infinite;
animation-direction: alternate;
```

**Shorthand:**  
`animation: name duration function delay count direction;`

**Using %:**
```css
@keyframes myAnim {
    0% { ... }
    50% { ... }
    100% { ... }
}
```

**Tip:** Use **Font Awesome** for free icons and fonts.

---

### CSS Grid
A layout system with rows and columns (like Excel).

**Container Properties:**
- `grid-template-rows`
- `grid-template-columns`
- `row-gap`
- `column-gap`
- `grid-template-columns: repeat(n, size)`
- `grid-template-rows: repeat(n, size)`

**Item Properties:**
- `grid-column-start`, `grid-column-end`
- `grid-row-start`, `grid-row-end`

**Note:**  
Items can overlap. Use `z-index` to control stacking.

---
