## 2. **CSS Grid Layout**

- CSS Grid is a layout system designed for building two-dimensional layouts (rows and columns). It’s perfect for creating more complex, structured layouts like grids.

### Key Concepts:

- **Grid Container**: The element with `display: grid;`.
- **Grid Items**: The direct children of the grid container.

### Key CSS Grid Properties:

- **On the Container (Parent)**:
    - `display: grid;`: Activates grid layout.
    - `grid-template-columns`: Defines the number and size of columns.
        - **Example**: `grid-template-columns: 1fr 2fr 1fr;` creates 3 columns with varying widths.
    - `grid-template-rows`: Defines the number and size of rows.
    - `gap`: Adds space between grid items.
        - **Example**: `gap: 10px;`.
    - `justify-items`: Aligns items horizontally.
    - `align-items`: Aligns items vertically.
- **On the Items (Children)**:
    - `grid-column`: Specifies which column an item spans.
    - `grid-row`: Specifies which row an item spans.

### Example:

```html
<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px;">
  <div style="background: red; height: 50px;"></div>
  <div style="background: green; height: 50px;"></div>
  <div style="background: blue; height: 50px;"></div>
</div>
```

Here:

- The grid has 3 equal-width columns (`1fr` each).
- Items are spaced with a `10px` gap.