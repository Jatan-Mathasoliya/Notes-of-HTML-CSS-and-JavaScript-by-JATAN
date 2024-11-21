## Tables in HTML

Tables are used in HTML to display data in a structured, grid-like format with rows and columns. They are particularly useful for presenting information such as financial data, schedules, and any data that requires a tabular layout.

### Basic Table Structure

- A basic HTML table is created using the `<table>` tag, with rows defined by the `<tr>` tag (table row), and cells within those rows defined by the `<td>` tag (table data).

**Example:**

```html
<table>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

### Table Headers

Table headers are defined using the `<th>` (table header) tag. These cells are typically displayed in bold and centered.

**Example:**

```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

### Table Sections

HTML tables can be divided into three sections: the table header (`<thead>`), the table body (`<tbody>`), and the table footer (`<tfoot>`).

**Example:**

```html
<table>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Row 1, Cell 1</td>
      <td>Row 1, Cell 2</td>
    </tr>
    <tr>
      <td>Row 2, Cell 1</td>
      <td>Row 2, Cell 2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Footer 1</td>
      <td>Footer 2</td>
    </tr>
  </tfoot>
</table>
```

### Table Attributes

- `border`**:** Specifies the width of the border around the table cells.

    ```html
    <table border="1">
      <tr>
        <td>Cell 1</td>
        <td>Cell 2</td>
      </tr>
    </table>
    ```
    
- `cellpadding`**:** Specifies the space between the cell content and the cell border.

    ```html
    <table cellpadding="10">
      <tr>
        <td>Cell 1</td>
        <td>Cell 2</td>
      </tr>
    </table>
    ```
    
- `cellspacing`**:** Specifies the space between individual table cells.

    ```html
    <table cellspacing="10">
      <tr>
        <td>Cell 1</td>
        <td>Cell 2</td>
      </tr>
    </table>
    ```
    

### ***Spanning Cells***

- `colspan`**:** Merges cells horizontally.
    
    html
    
    ```html
    <table border="1">
      <tr>
        <th colspan="2">Header spanning 2 columns</th>
      </tr>
      <tr>
        <td>Row 1, Cell 1</td>
        <td>Row 1, Cell 2</td>
      </tr>
    </table>
    ```
    
- `rowspan`**:** Merges cells vertically.
 
    ```html
    <table border="1">
      <tr>
        <th rowspan="2">Header spanning 2 rows</th>
        <td>Row 1, Cell 2</td>
      </tr>
      <tr>
        <td>Row 2, Cell 2</td>
      </tr>
    </table>
    ```


 ## Summary

- **Basic Structure:** `<table>`, `<tr>`, `<td>`, `<th>`

- **Sections:** `<thead>`, `<tbody>`, `<tfoot>`

- **Attributes:** `border`, `cellpadding`, `cellspacing`

- **Spanning Cells:** `colspan`, `rowspan`

- **Styling:** Use CSS for visual enhancements