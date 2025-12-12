Card 1 Learning Journey – CSS Units
🔬 Experiments Conducted

For this card, I experimented with how px, em, rem, and % behave differently in the browser. I tested each unit by creating small demo elements and adjusting the root font size to watch how em and rem scale. I also tried using percentages inside differently sized containers to see how fluid layouts respond. I spent time comparing the results in Live Server to understand how these units actually look on a page.

💡 Key Discoveries

I learned that px is completely fixed, while em depends on its parent and can become unpredictable with deep nesting. rem felt the most reliable because it always references the root, which is why so many developers use it for typography. % finally made sense too — it doesn’t scale the text but the layout around it. Seeing everything in an actual HTML file helped the concepts click much faster.

⚠️ Challenges Faced

The biggest challenge was understanding why em values were acting weird when I changed parent font sizes. Nesting changed the math more than I expected. Also, styling the HTML version of the card confused me at first because I wasn’t viewing the correct file in Live Server and thought my CSS wasn’t working.

Card 2 Learning Journey – View Transitions API
🔬 Experiments Conducted

For this card, I tried out the View Transitions API by writing a small script that swaps content on click. I tested how the browser captures the old view and transitions into the new one. I also experimented with the view-transition-name CSS property to see how shared element transitions behave.

💡 Key Discoveries

I learned that View Transitions are surprisingly powerful for how little code they require. The browser is doing most of the heavy lifting—capturing snapshots, animating between states, and handling timing. It feels like a mini SPA experience without a framework. I also realized that this API is still new and not fully supported everywhere, which explains why demos sometimes behave inconsistently.

⚠️ Challenges Faced

At first, I expected the transitions to work like a full router or a framework animation, so I was confused about what exactly gets animated. Once I realized it only transitions elements with matching names, things made more sense. Another challenge was writing clean HTML/CSS versions for my site, but once I had a reusable card layout, everything began to slot into place.

Card 3 Learning Journey – Button vs Link
🔬 Experiments Conducted

I compared real <a> and <button> elements by testing navigation vs. UI actions. I also inspected how screen readers interpret each element, which helped reinforce why semantics matter. I tried wiring a button to a simple JavaScript function to see how it differs from navigation behavior.

💡 Key Discoveries

I learned that buttons and links are not interchangeable even if we can style them to look identical. Buttons are for actions on the current page, and links are for navigation — simple, but super important for accessibility. It was also interesting to see how confusing it becomes when a link behaves like a button or vice versa.

⚠️ Challenges Faced

My biggest struggle wasn’t the HTML—it was managing the Git workflow for separate branches per card. I kept running into remote issues, missing commits, and VS Code errors. Once I understood what origin was pointing to and how to push each branch, everything made more sense.

🌱 Weekly Reflection
✅ What concepts clicked for you this week?

CSS units finally clicked for me, especially the difference between em and rem. I also understood semantic HTML much better after working on the Button vs Link card. Additionally, the View Transitions API helped me see how modern web APIs can replace heavier JavaScript animation libraries.

🧭 What are you still exploring?

I’m still getting comfortable with Git branching and pull requests. I also want to experiment more with advanced transitions and maybe add more animations to my card layouts. And I’m still learning how to structure HTML and CSS cleanly for reusable components.

🤖 How did AI assistance help your learning?

AI helped me break concepts down into clear explanations and gave me examples that actually worked when I pasted them into my project. It also saved me from hours of frustration by diagnosing Git and Live Server issues. The custom styles.css and complete HTML templates helped me understand card layout structure in a real-world way.

🔄 What will you do differently next week?

Next week, I want to slow down when creating branches and make sure I’m always working from the updated main branch before starting a new card. I also want to start validating each card earlier so I don’t have to fix formatting at the end. And I want to keep my folder structure cleaner so I always know where my files live.

✏️ Notes

This week had a lot of “I finally get it!” moments — especially with Git, Live Server, and how to structure my HTML/CSS properly. Once the first card styling worked, everything snowballed and became easier. I’m definitely building confidence and starting to feel more like a real web developer.
