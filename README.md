## 🎙️ Presentation Script (Detailed Version)

### 🟢 1. Introduction

Hi, I’m Phillip-Rossouw Botha. This is my resume website, built from scratch using only HTML and CSS. I used a Figma design as my reference and focused on making the site both visually accurate and fully responsive, without any JavaScript or frameworks.

### 🟢 2. Resume Walkthrough

- **Profile:**  
  The top section shows my name, a short summary, and a profile image. I used a `<header>` tag and Flexbox to place the text and image side-by-side on desktop, and on mobile for better readability.

- **Proficiency Bars:**  
  Each skill is displayed with a horizontal bar showing my proficiency. I created a container for each skill and used a nested div for the fill, setting its width in CSS (like 90% or 80%) to visually represent my skill level, matching the Figma design.

- **Skills Tags:**  
  I listed my main tools and technologies as tags. This section uses Flexbox with `flex-wrap` to allow the tags to wrap onto new lines. Each tag is styled with padding, borders, and consistent font size to keep the look clean and organized.

- **Projects:**  
  My projects are shown as cards, each with a title, role, and tech stack icons. I used semantic HTML for each card.The cards are arranged in a grid that adapts to screen size, expanding to four columns on large screens.

- **Education & Experience:**  
  This section lists  education and work history. On desktop, I used a two-column grid layout, while on mobile, the columns stack vertically. Dates and details are styled for clarity, and spacing is controlled with CSS Grid and gap properties.

- **Footer:**  
  The footer contains links to my GitHub, LinkedIn, and email. Each link has a hover effect for feedback, and I made sure all links are accessible and easy to use.

### 🟢 3. Responsiveness Demo

- **Mobile-first CSS:**  
  I started with styles for mobile devices, then used media queries to adjust layouts for tablets and desktops. This ensures the site looks good and works well on any device.

- **Desktop Layout:**  
  For larger screens, I used CSS Grid to create a two-column layout for the main content. The `.main-container` uses `grid-template-areas` to precisely place each section. Project cards expand into a four-column grid, making the site look more dynamic and professional on desktop.

### 🟢 4. Code Overview

- **HTML:**  
  I used semantic elements like `<header>`, `<main>`, `<section>`, and `<footer>` to organize the content logically. Class names are consistent and descriptive, such as `.skills-grid` and `.project-card`, making the code easy to read and maintain.

- **CSS:**  
  My CSS starts with a reset, then sets global styles for fonts and colors. I used CSS variables for colors and font sizes to match the Figma design and keep things consistent. Flexbox and Grid are used throughout for layout, and I separated styles by section for clarity.

### 🟢 5. Reflection

The hardest part was matching the Figma layout exactly, especially across different devices. Breaking the site into sections and using a mobile-first approach made it manageable. I’m proud of the clean, responsive result using just HTML and CSS. In the future, I’d like to add JavaScript for interactivity and improve accessibility even further.


Link to Loom VId - https://www.loom.com/share/c6301086ad8c4cbe8b749d1ad762f752?sid=78c52f25-c51e-4c5f-9322-732d963f2bfa

