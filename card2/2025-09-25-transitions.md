---
title: View Transitions API — Smooth Page Transitions with CSS
date: 2025-01-21
category: web-api
difficulty: intermediate
source: https://developer.mozilla.org/en-US/docs/Web/API/View_Transition_API
author: Stephanie Perdomo
---

# View Transitions API — Smooth Page Transitions with CSS

## Explanation

The View Transitions API is a modern browser feature that enables smooth visual transitions when switching between pages, components, or states—without needing heavy JavaScript libraries or full single-page application frameworks. Normally, moving from one page to another triggers a full reload, which can feel abrupt. With the View Transitions API, the browser captures the current view, loads the next view, and animates the difference between them.

Developers enable this by giving elements a `view-transition-name` in CSS and calling `document.startViewTransition()` in JavaScript to trigger the animation. During the transition, the browser creates snapshots of both the old and new content, then animates shared elements—such as images, titles, or cards—so they smoothly morph between states. This makes interactions feel more fluid and app-like.

Because the API is still new, browser support continues to improve, but it already allows developers to create polished transitions like fades, slides, or element morphing with minimal code. It’s a powerful tool for elevating user experience on modern websites.

---

## Example

```html
<button id="next-page">Go to Next Page</button>

<script>
document.getElementById('next-page').addEventListener('click', () => {
  document.startViewTransition(() => {
    // Replace the content during the transition
    document.body.innerHTML = '<h1>New Page Content</h1>';
  });
});
</script>

<style>
h1 {
  view-transition-name: title;
}
</style>
