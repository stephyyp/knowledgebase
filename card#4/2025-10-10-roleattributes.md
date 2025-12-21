# Card: 
When and How to Use `role` Attributes

# Source: 
MDN Web Docs – ARIA Roles

**Explanation**  

ARIA (Accessible Rich Internet Applications) roles help improve accessibility by explicitly telling assistive technologies what a particular element does. The `role` attribute can define elements that don’t have a clear semantic meaning or enhance native HTML elements. For example, `<div>` or `<span>` have no inherent meaning, but adding `role="button"` or `role="navigation"` informs screen readers and other assistive tools about their purpose. Proper use of ARIA roles ensures that all users, including those relying on assistive technologies, understand and interact with your website effectively. However, ARIA should **not replace native HTML elements** when they already convey meaning — for example, use `<button>` for actions instead of a `<div>` with `role="button"` unless necessary.


**When to Use**  

- ✅ Use ARIA roles when creating custom UI components that don’t have native semantic meaning.  
- ✅ Use `role` to enhance accessibility when styling or scripting removes native semantics.  
- ⚠️ Avoid unnecessary roles on elements that already have semantic meaning (like `<nav>`, `<header>`, or `<button>`).

**Example**  

```html
<!-- Custom button using div -->
<div role="button" tabindex="0" onclick="submitForm()">
  Submit
</div>

<!-- Navigation landmark -->
<nav role="navigation">
  <ul>
    <li><a href="/home">Home</a></li>
    <li><a href="/about">About</a></li>
  </ul>
</nav>

