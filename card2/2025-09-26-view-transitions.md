---

# Card: View Transitions API: Smooth Page Transitions with CSS #42

---


# Explanation
The View Transitions API is a modern web feature that makes switching between pages or views feel smooth and polished without needing heavy JavaScript frameworks. Traditionally, navigating from one page to another in a website causes a full reload, which can feel jarring to users. With the View Transitions API, the browser can animate elements from the old page to the new page, letting developers create seamless visual effects. This works by marking elements with a view-transition-name in CSS and then using document.startViewTransition() in JavaScript to trigger the transition. During the transition, the browser captures the current layout, loads the new content, and animates elements from the old state to the new state. It’s especially useful for things like fading content in and out, sliding sections between views, or smoothly transforming shared elements (like images or cards) between pages. The API is still relatively new, so browser support is improving, but it’s a powerful tool for making websites feel more interactive and responsive without relying on heavy animations or external libraries.

# Source: https://developer.mozilla.org/en-US/docs/Web/API/View_Transition_API?
MDN Web Docs – View Transitions API

---

# Example:

<button id="next-page">Go to Next Page</button>

<script>
document.getElementById('next-page').addEventListener('click', () => {
  document.startViewTransition(() => {
    // Example: swap content
    document.body.innerHTML = '<h1>New Page Content</h1>';
  });
});
</script>

<style>
h1 {
  view-transition-name: title;
  transition: transform 0.5s ease;
}
</style>

---

# When to Use:

    - Use for smooth page or view changes to enhance UX.

    - Ideal for single-page apps or sites where content updates frequently.

    - Best for shared elements between pages, like images, cards, or sections that appear in both views.

    - Avoid for very old browsers or simple pages where a full reload is fine.