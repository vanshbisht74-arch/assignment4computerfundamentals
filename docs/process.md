Development Process & Future Improvements
 Development Workflow
Phase 1: Structural Foundation
I began by establishing the HTML5 skeleton. I prioritized semantic tags (<header>, <section>, <footer>) over generic <div> tags to improve code readability and accessibility.

Key Decision: I structured the "Projects" section using a wrapper div to prepare for the sliding animation logic.
Phase 2: Aesthetic Design (The "Neon" Look)
I wanted a unique visual style.

Gradient Text: I utilized background-clip: text combined with a linear gradient to create the multi-colored text effect in the header.
Animation: I defined a custom @keyframes neon_rainbow animation to shift the background position, creating a shimmering neon effect.
Phase 3: The CSS-Only Carousel
The most complex feature was the project slider. Instead of using JavaScript, I used CSS math.

I set the #wrapper width to 400% (since there are multiple slides).
I created a @keyframes slide animation that shifts the transform: translateX() property at specific percentage intervals (0%, 33%, 66%) to show one project at a time.
Phase 4: Responsiveness
Finally, I added Media Queries.

Challenge: The 40% width for the project box looked great on laptops but was too small on phones.
Solution: I implemented a @media (max-width: 768px) rule to increase the container width to 90% on smaller devices.
 Future Improvements
While the current version is fully functional, I plan to implement the following features in v2.0:

JavaScript Form Validation: currently, the contact section is static. I plan to add a functional input form that validates email addresses before sending.
Dark/Light Mode Toggle: A switch to allow users to toggle between the current light theme and a dark, high-contrast theme.
Project Detail Modals: Clicking on a project in the carousel should open a pop-up (modal) with more details about that specific assignment, rather than just showing an image.