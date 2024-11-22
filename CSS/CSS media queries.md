
## 3. **Responsive Web Design (Media Queries)**

- Responsive web design ensures that a webpage looks good on all devices (desktops, tablets, smartphones). **Media queries** allow us to apply different styles depending on the screen size or device type.

### How Media Queries Work:

- Media queries check the screen size or other conditions (e.g., orientation) and apply specific CSS when the condition is true.

### Syntax:

```css
@media (condition) {
  /* CSS rules here */
}
```

### Common Use Cases:

1. Adjust layout for smaller screens:
    
    ```css
    @media (max-width: 600px) {
      body {
        font-size: 14px;
      }
    }
    ```
    
    This rule makes the font smaller if the screen width is 600px or less.
    
2. Switch to a single-column layout for small screens:
    
    ```css
    @media (max-width: 600px) {
      .container {
        display: flex;
        flex-direction: column;
      }
    }
    ```
    
3. Handle orientation:
    
    ```css
    @media (orientation: landscape) {
      body {
        background-color: lightblue;
      }
    }
    ```
    

### Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-family: Arial, sans-serif;
    }
    .box {
      width: 200px;
      height: 200px;
      background: red;
    }
    @media (max-width: 600px) {
      .box {
        background: blue;
      }
    }
  </style>
</head>
<body>
  <div class="box"></div>
</body>
</html>
```

In this example:

- The `.box` is red by default.
- If the screen width is 600px or less, the `.box` turns blue.