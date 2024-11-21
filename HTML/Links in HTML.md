## **Links :**
- Links or hyperlink are one of the most essential feture of HTML.
- Using Links we can Connect Web-Pages, Connect multiple pages of a website, navigate diffrent section of web-page.
- Links can be used to connect to external websites, email, phone number, etc.

### **Basic stuctuer of Link :**
- Link start with `<a>` tag. The most crucial attribute of the `<a>` tag is the `href` attribute, which specifies the destination of the link.

### **Ex:**
```html
<a href="https://www.google.com">Google</a>
```

### **Explaination :**
- In the above example, the link is pointing to Google's website
- `<a>` is the anchor tag of the link
- `href="https://www.google.com"`:  This Provides the URL of destination of the link.
- `</a>` This is a closing tag of link.

## Types of Links

### 1. **Absolute URLs:**  
Absolute URLs contain the full address of the destination, including the protocol (http, https, ftp, etc.), domain name, and path.
    
    
    `<a href="https://www.example.com/page.html">Absolute URL</a>`
    
### 2. **Relative URLs:**
Relative URLs specify a path relative to the current document. They are often used for linking to pages within the same site.
    
    
    `<a href="/contact.html">Relative URL</a>`
    
### 3. **Anchors:**
Anchors are used to link to a specific part of the same page. This is done by using the `id` attribute on the target element and referencing it with a hash symbol (#).
    
    
    `<a href="#section2">Go to Section 2</a>
    
    <h2 id="section2">Section 2</h2>`
    
### 4. **Email Links:**
Email links use the `mailto:` scheme in the `href` attribute to open the user's default email client with a new email draft.
    
    
    `<a href="mailto:example@example.com">Send Email</a>`
    
### 5 . **Telephone Links:**
Telephone links use the `tel:` scheme to initiate a phone call on devices that support calling.
    
    
    `<a href="tel:+1234567890">Call Us</a>`


## Styling Links

Links can be styled using CSS to change their appearance. Common pseudo-classes used for styling links include:

- `:link` - Unvisited links
- `:visited` - Visited links
- `:hover` - When the mouse is over the link
- `:active` - When the link is being clicked

### **Example CSS:**

CSS

```css
a:link {
    color: blue;
}  
a:visited {
    color: purple;
}
a:hover {
    color: red;
}
a:active {
    color: green;
}
```

### Additional Attributes

 **1. `target`**  
The `target` attribute specifies where to open the linked document.  
    -  `_blank`: Opens the link in a new tab or window.  
        `<a href="https://example.com" target="_blank">Open in New Tab</a>`  
    -  `_self`: Opens the link in the same frame (default behavior).   
    - `_parent`: Opens the link in the parent frame.  
    - `_top`: Opens the link in the full body of the window.  

 **2.`title`** 
The `title` attribute provides additional information about the link, which appears as a tooltip when the user hovers over the link.

    `<a href="https://example.com" title="Visit Example Site">Hover Over Me</a>`

    
3. `rel`**:**
The `rel` attribute specifies the relationship between the current document and the linked document. It is commonly used with the `nofollow` value to instruct search engines not to follow the link.

    `<a href="https://example.com" rel="nofollow">Nofollow Link</a>`
