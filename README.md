## 🎙️ My Presentation Script

Below is the outline I followed when recording my 5–10 minute presentation for this project. It helped me explain my site, code, layout decisions, and what I’ve learned.

### 🟢 1. Introduction (30 sec – 1 min)

Hi, I’m Phillip-Rossouw Botha, and this is my resume website project built entirely using HTML and CSS.

This project taught me how to take a Figma design and translate it into a clean, responsive, and pixel-perfect website using only frontend tools.

One thing I’m especially proud of is how accurately I matched the layout, including the spacing, font sizes, and mobile responsiveness — without using any JavaScript or frameworks.

### 🟢 2. Walkthrough of the Resume (2–3 min)

#### 🧑‍💼 Profile & Summary

The site starts with my name, a short summary, and a circular profile image.
I wrote my summary to quickly describe who I am: a student developer and web-hosting tech who’s transitioning into frontend development.
I structured this section in HTML using a `<header>` tag, with a container that uses Flexbox to position the text and image side-by-side on desktop and stacked on mobile.

#### 📊 Proficiency Bars

Next are the proficiency bars — I used a container div for each skill, then a nested div with a class to represent the fill percentage.
The widths are controlled in CSS using percentage widths like 90%, 80%, etc., to match the Figma design exactly.

#### 🏷️ Skills Tags

For the skills section, I chose key tools I’ve worked with.
I used a simple grid layout with `display: flex; flex-wrap: wrap` and styled each skill as a tag using padding, borders, and consistent font sizing.

#### 🛠️ Projects

I included a section that highlights some of the projects I’ve worked on.
Each project card is structured using semantic HTML and styled with cards that have hover effects.
One project I’m proud of is [insert short mention of project title here] — I made sure each card has a title, role, and relevant tech stack icons.

#### 🎓 Education & 💼 Experience

This section displays my education and work history.
I followed the 2-column layout on desktop and a stacked layout on mobile.
I styled the date and details using grid and ensured spacing matched the design.

#### 🔗 Footer

At the bottom, I have a clean footer with working links to my GitHub, LinkedIn, and email.
Each icon or text link has a hover effect, and all are accessible and functional.

### 🟢 3. Responsiveness Demo (30 sec – 1 min)

To make my site responsive, I used a mobile-first CSS approach. That means my base styles are optimized for mobile, and I progressively enhanced the layout with media queries for tablets and desktops.

#### 📱 Mobile & Tablet

On smaller screens, I used Flexbox and Grid to stack elements vertically and control spacing. The `.profile-section`, for example, stacks the image and text vertically using Flexbox, and each section like `.proficiency-box`, `.skills-box`, and `.projects-box` uses full width with consistent padding.

#### 💻 Desktop View (1200px and up)

I used a `@media (min-width: 1200px)` query to create a grid layout across the entire page. The `.main-container` switches to `display: grid` with two columns: `2fr 1fr`. It defines `grid-template-areas` like this:

```css
grid-template-areas:
  'profile profile'
  'proficiency skills'
  'projects projects'
  'education tools'
  'experience experience'
  'contact contact';
```

This allowed me to assign each section like `.profile-section` or `.education-section` to their own `grid-area`, giving me full control over the desktop layout and spacing.

For example, the Proficiency and Skills sections sit side-by-side, as do Education and Tools. On larger screens, the project cards expand into a 4-column grid using `grid-template-columns: repeat(4, 1fr);`, which gives the page a more dynamic and professional feel.

Implementing the desktop media query was one of the more complex but rewarding parts of the build — it helped me understand how to use CSS Grid not just for components but for full-page layout.

### 🟢 4. Code Overview (2–3 min)

#### 🔍 HTML Structure

In my `index.html`, I kept things semantic and accessible.
I used `<header>`, `<main>`, `<section>`, and `<footer>` to logically group the page content.
I avoided unnecessary `div` nesting and kept my class names consistent and readable — like `.skills-grid` or `.project-card`.

#### 🎨 CSS Organisation

My CSS is organized into sections: I began with a reset, then global styles like fonts and colors, then specific sections.
I used variables for color and font sizes to stay consistent with the Figma design.

#### 💡 Layout Challenges

One challenge was aligning the profile section image perfectly — I fixed this using `align-items: center` in Flexbox and careful margin tweaks.
Another was spacing the skills and education sections, where I used Grid and `gap` properties to handle that cleanly.

### 🟢 5. Reflection (1 min)

The most challenging part was getting the layout to match Figma exactly, especially across devices.
But once I broke it into sections and used a mobile-first approach, it became easier to test each part on its own.

I’m proud of how clean and responsive the final result is, and that I didn’t rely on any frameworks — just raw HTML and CSS.

Next time, I’d love to explore adding JavaScript interactivity and maybe improving accessibility even more with ARIA labels.
