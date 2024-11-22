## **CSS Positing :**

- **CSS positioning is a way to control how elements are placed on a webpage. There are several positioning types, and each one behaves differently. Let’s break them down in simple terms:**

### **1. Static Positioning (Default)**
**Default behavior:** All elements are positioned as part of the normal flow of the page.  
**No special positioning:** Elements are stacked one after another, like blocks in a document.  
**No CSS needed:** This is the default if you don’t specify a position.
Example:
```html
<div style="position: static;">I am static (default).</div>
```
- Static elements don’t respond to top, left, right, or bottom properties.


### **2. Relative Positioning**
**Relative to itself:** The element’s position is adjusted relative to where it would normally be (static position).  
**Shifts without affecting other elements:** Other elements don’t move, and the original space for the element is preserved.  

How it works:

Use top, left, right, or bottom to move it from its original position.
Example:
```html
<div style="position: relative; top: 20px; left: 10px;">
  I moved 20px down and 10px to the right from my original position.
</div>
```
- The element still occupies its original space in the flow, even though it appears shifted.

### **3. Absolute Positioning**
**Removed from normal flow:** The element is taken out of the document flow, so it no longer affects or is affected by other elements.  
**Positioned relative to the nearest positioned ancestor:**
If no ancestor has a position set, it positions itself relative to the <html> (the entire page).  

**How it works:**
Use top, left, right, or bottom to specify exact positioning.
Example:
```html
<div style="position: relative;">
  <div style="position: absolute; top: 0; left: 0; background: yellow;">
    I’m absolutely positioned relative to my parent (the nearest positioned ancestor).
  </div>
</div>
```

### **4. Fixed Positioning**
**Stays fixed in place:** The element does not move even if the page is scrolled.
**Positioned relative to the viewport:** The viewport is the visible area of the webpage.

**How it works:**
Use top, left, right, or bottom to fix the element’s position on the screen.
Example:
```html
<div style="position: fixed; top: 10px; left: 10px; background: lightblue;">
  I’m fixed to the top-left corner of the viewport and don’t move when you scroll.
</div>
```

**Practical Example :**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Positioning</title>
  <style>
    .box {
      width: 100px;
      height: 100px;
      margin: 10px;
      text-align: center;
      line-height: 100px;
      color: white;
      font-size: 14px;
    }

    .static { background: gray; position: static; }
    .relative { background: blue; position: relative; top: 10px; left: 10px; }
    .absolute { background: green; position: absolute; top: 50px; left: 50px; }
    .fixed { background: red; position: fixed; top: 10px; right: 10px; }
  </style>
</head>
<body>
  <div class="box static">Static</div>
  <div class="box relative">Relative</div>
  <div class="box absolute">Absolute</div>
  <div class="box fixed">Fixed</div>
</body>
</html>
```

**Static:** Appears in the normal flow. 

**Relative:** Moves but leaves a gap in its original space.  

**Absolute:** Positioned at (50px, 50px) from its containing block.  

**Fixed:** Sticks to the corner, unaffected by scrolling.