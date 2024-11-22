## 1. **Flexbox Layout**

Flexbox is a CSS layout model that makes it easy to design flexible and responsive layouts. It allows items in a container to align, distribute, and resize dynamically based on the available space.

### Key Concepts:

- **Parent Container**: The element with `display: flex;`.
- **Flex Items**: The direct children of the flex container.

### Key Flexbox Properties:

- **On the Container (Parent)**:
    - `display: flex;`: Activates flexbox for the container.
    - `flex-direction`: Defines the direction of items (row, column).
        - `row` (default): Items are placed in a row.
        - `column`: Items are placed in a column.
    - `justify-content`: Aligns items horizontally.
        - `flex-start`, `center`, `flex-end`, `space-between`, `space-around`, etc.
    - `align-items`: Aligns items vertically.
        - `stretch` (default), `center`, `flex-start`, `flex-end`.
    - `flex-wrap`: Allows items to wrap to the next line if needed.
        - `nowrap` (default), `wrap`.
- **On the Items (Children)**:
    - `flex`: Controls how items grow, shrink, and take up space.
    - `align-self`: Allows individual items to override `align-items`.

### Example:

```html
<div style="display: flex; justify-content: center; align-items: center; height: 200px; background: lightgray;">
  <div style="width: 50px; height: 50px; background: red;"></div>
  <div style="width: 50px; height: 50px; background: green;"></div>
  <div style="width: 50px; height: 50px; background: blue;"></div>
</div>
```

Here:

- Items are centered both horizontally (`justify-content`) and vertically (`align-items`).
