# 🃏 Card: CSS Houdini — Introduction to the CSS Paint API

**Explanation**  
The CSS Paint API, part of the CSS Houdini suite, allows developers to programmatically create custom CSS graphics directly in the browser. With this API, you can define a JavaScript function (a "paint worklet") that draws shapes, patterns, or effects, and then use it as a background or border image in CSS. This enables dynamic, procedural graphics without relying on images or complex SVG code. CSS Houdini gives developers more control over how CSS is rendered, bridging the gap between CSS and JavaScript and allowing for more creative and responsive designs.  

**When to Use**  
- ✅ When you need dynamic backgrounds, gradients, or textures that can change based on variables or user input.  
- ✅ When you want to create reusable, programmable graphics that integrate smoothly with CSS.  
- ⚠️ Avoid using it for static images where a normal CSS background or SVG would suffice, as the Paint API adds extra complexity.

**Example**  
```javascript
// register a paint worklet
if ('paintWorklet' in CSS) {
  CSS.paintWorklet.addModule('stripes.js');
}

// stripes.js
class Stripes {
  paint(ctx, size) {
    ctx.fillStyle = 'red';
    ctx.fillRect(0, 0, size.width, size.height);
  }
}
registerPaint('stripes', Stripes);