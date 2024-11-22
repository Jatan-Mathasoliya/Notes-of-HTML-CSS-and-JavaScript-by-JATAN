## CSS Syntax and Selectors

**CSS Syntax:**
CSS is composed of selectors and declarations. A CSS rule set consists of a selector and a declaration block.

**Example:**

```css
selector {
  property: value;
}
```

### **Selectors:**
- Selectors are used to target HTML elements for styling.

### **Type Selector:** Targets elements by their tag name.
 ```css
    p {
      color: blue;
    }
```
    
### **Class Selector:** Targets elements with a specific class attribute. Prefixed by a dot (`.`).

  ```css
  .classname {
      color: red;
    }
```
    
### **ID Selector:** Targets an element with a specific id attribute. Prefixed by a hash (`#`).
  
```css
    #idname {
      color: green;
    }
 ```
    
### **Attribute Selector:** Targets elements with a specific attribute.
       
```css
    a[href] {
      color: orange;
    }
```
    
### **Descendant Selector:** Targets elements that are descendants of another element.

```css
    div p {
      color: purple;
    }
```