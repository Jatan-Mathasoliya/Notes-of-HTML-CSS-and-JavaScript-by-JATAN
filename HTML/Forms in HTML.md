## **Forms**
- Forms in HTML are used to collect user input and send it to a server for processing. They are an essential part of any web application, enabling interaction between users and the system.

### **Basic Structure of an HTML Form**
```html
<form action="/submit-form" method="POST">
  <!-- Form Elements Go Here -->
</form>
```

`<form>`Tag:  
- `action`: Specifies the URL where the form data will be sent.
- `method`: Determines how the data will be sent (e.g., GET, POST).

### **Common Form Elements**

**Text Input (`<input type="text">`):**

- Used to collect single-line text.
```html
<label for="name">Name:</label>
<input type="text" id="name" name="name">
```

**Password Input (`<input type="password">`):**

- Masks user input for security.
```html
<label for="password">Password:</label>
<input type="password" id="password" name="password">
```
**Radio Buttons (`<input type="radio">`):**

- Allows the user to select one option from a group.
```html

<label><input type="radio" name="gender" value="male"> Male</label>
<label><input type="radio" name="gender" value="female"> Female</label>
```
**Checkboxes (`<input type="checkbox">`):**

- Lets users select multiple options.
```html

<label><input type="checkbox" name="hobby" value="reading"> Reading</label>
<label><input type="checkbox" name="hobby" value="sports"> Sports</label>
```
**Dropdown List (`<select>`):**

- Provides a dropdown menu for selecting an option.
```html
<label for="country">Country:</label>
<select id="country" name="country">
  <option value="us">United States</option>
  <option value="uk">United Kingdom</option>
  <option value="in">India</option>
</select>
```
**Textarea (`<textarea>`):**

- Allows multi-line text input.
```html

<label for="message">Message:</label>
<textarea id="message" name="message"></textarea>
```
**Submit Button (`<input type="submit"> or <button>`):**

- Submits the form data to the specified action URL.
```html

<button type="submit">Submit</button>
```
**File Input (`<input type="file">`):**

-Enables users to upload files.
```html

<label for="file">Upload File:</label>
<input type="file" id="file" name="file">
```
**Hidden Input (<input type="hidden">):**

- Stores hidden data sent with the form submission.
```html

<input type="hidden" name="userID" value="12345">
```

### **Additional Attributes for Inputs**
**required: Makes a field mandatory.**

```html

<input type="text" name="username" required>
```
**placeholder: Provides a hint inside the input field.**

```html

<input type="email" placeholder="Enter your email">
```

**maxlength and minlength: Limit the number of characters.**

```html

<input type="text" maxlength="10" minlength="5">
```
**pattern: Validates input using a regular expression.**

```html

<input type="text" pattern="\d{3}-\d{2}-\d{4}" placeholder="123-45-6789">
```
**readonly and disabled:**

- readonly: Prevents editing.
- disabled: Makes the input non-interactive.
```html

<input type="text" value="Read Only" readonly>
<input type="text" value="Disabled" disabled>
```
### **Form Validation**
HTML5 includes built-in form validation:

- required: Ensures the field is filled.
- type="email": Ensures a valid email address.
- type="number": Ensures numeric input.
- Custom Validation: Add custom messages using JavaScript.
### **Form Example**
```html

<form action="/submit-form" method="POST">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br>

  <label for="gender">Gender:</label>
  <input type="radio" name="gender" value="male"> Male
  <input type="radio" name="gender" value="female"> Female<br>

  <label for="hobby">Hobbies:</label>
  <input type="checkbox" name="hobby" value="reading"> Reading
  <input type="checkbox" name="hobby" value="sports"> Sports<br>

  <button type="submit">Submit</button>
</form>
```

### **Features of Forms**
- Data Collection: Collects structured data from users.
- Accessibility: Easily styled and accessible.
- Validation: Ensures proper input before submission.
Forms are a backbone of user interaction on the web!