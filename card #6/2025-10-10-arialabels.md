# Card: 
ARIA Labels and Descriptions — 
`aria-label`, `aria-labelledby`, `aria-describedby`

**Explanation**  

ARIA attributes like `aria-label`, `aria-labelledby`, and `aria-describedby` are essential tools for improving web accessibility. They give screen readers and other assistive technologies extra information about the purpose or meaning of elements, helping users navigate and interact with a website more effectively. `aria-label` provides an **explicit label** for an element that might not have visible text, such as icon buttons. `aria-labelledby` allows an element to **reference another element’s text** as its label, which can reduce duplication and maintain consistency. `aria-describedby` points to one or more elements that **provide additional descriptive information**, like hints or instructions for a form input. Using these attributes correctly ensures that users relying on assistive technology can understand the function, context, and details of interactive elements, improving usability and creating a more inclusive experience.  

**When to Use**  

- ✅ `aria-label`: For buttons, icons, or inputs that have no visible text.  
- ✅ `aria-labelledby`: When an element’s label exists elsewhere in the DOM, like a heading or form label.  
- ✅ `aria-describedby`: When additional instructions or hints need to be associated with a form field or interactive element.

**Example**  

```html
<!-- Using aria-label for an icon button -->
<button aria-label="Close menu">
  <span class="icon-close"></span>
</button>

<!-- Using aria-labelledby -->
<label id="username-label">Username</label>
<input type="text" aria-labelledby="username-label">

<!-- Using aria-describedby -->
<input type="email" aria-describedby="email-help">
<p id="email-help">Enter your email in the format user@example.com</p>