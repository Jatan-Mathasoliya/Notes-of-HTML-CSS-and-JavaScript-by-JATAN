## Images In HTML

- Images play a crucial role in enhancing the visual appeal and providing context to web content. In HTML, the `<img>` tag is used to embed images in a web page.

## Basic Syntax of the `<img>` Tag

The `<img>` tag is an empty (self-closing) tag, meaning it does not require a closing tag. It includes several attributes to specify the source, alternative text, and other properties of the image.

### **Basic Structure:**

`<img src="image.jpg" alt="Description of the image">`

## Key Attributes of the `<img>` Tag

1. `src` **(Source):**
    - Specifies the path to the image file.
    - Can be an absolute URL (full web address) or a relative URL (path relative to the current document).
    - **Example:**
 
        ```html
        <img src="https://www.example.com/images/photo.jpg" alt="A scenic photo">
        <img src="images/photo.jpg" alt="A scenic photo">
        ```
        
2. `alt` **(Alternative Text):**
    - Provides descriptive text for the image.
    - Important for accessibility, as it is read by screen readers for users with visual impairments.
    - Displayed in place of the image if the image fails to load.
    - **Example:**
  
        ```html
        <img src="photo.jpg" alt="A scenic view of mountains and a lake">`
        
3. `width` **and** `height`**:**
    - Specifies the width and height of the image in pixels or as a percentage.
    - Helps the browser allocate space for the image before it is fully loaded.
    - **Example:**

        ```html
        <img src="photo.jpg" alt="A scenic view" width="600" height="400">`
        
4. `title`**:**
    - Provides additional information about the image.
    - Displayed as a tooltip when the user hovers over the image.
    - **Example:**

        ```html
        <img src="photo.jpg" alt="A scenic view" title="Scenic Photo">`