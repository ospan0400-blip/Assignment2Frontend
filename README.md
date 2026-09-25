# Frontend Assignment 2

## Overview

This project is a frontend web development assignment demonstrating different CSS layout techniques using **HTML5 and CSS3**. The project is divided into three parts, with each part focusing on a different approach to arranging and styling webpage content.

The project demonstrates:

- Flexbox layouts
- CSS Grid layouts
- Responsive card layouts
- Navigation bars
- Image galleries
- Portfolio/project cards
- Hover effects and transitions
- Semantic HTML elements
- External CSS stylesheets

## Project Structure

```text
Assignment2Frontend-main/
│
├── index.html
├── index1.html
├── index2.html
│
├── style.css
├── style1.css
├── style2.css
│
├── favicon.ico
│
├── berriesimage.jpg
├── bluesky.jpg
├── bridgeimage.jpg
├── cityimage.jpg
├── desktopimg.jpg
├── landscapeimage.jpg
├── mountainsimage.jpg
├── project1image.jpg
├── project2image.jpg
├── project3image.jpg
├── railroads.jpg
├── shoppingimage.jpg
├── streetlightsimage.jpg
├── tulipimage.jpg
└── winterimage.jpg
```

## Part 1 — Flexbox Card Layout

**Files:**
- `index.html`
- `style.css`

The first part demonstrates a navigation bar and a row of responsive cards.

### Features

- Flexbox navigation menu
- Three content cards
- Images inside cards
- Card titles and descriptions
- "Explore" buttons
- Flexible card sizing using `flex`
- Hover effects
- Button transitions
- Responsive wrapping with `flex-wrap`

The cards are arranged using:

```css
.cardrow {
    display: flex;
    gap: 24px;
    flex-wrap: wrap;
}
```

Each card uses a flexible width:

```css
.card {
    display: flex;
    flex-direction: column;
    flex: 1 1 280px;
}
```

This allows the cards to adjust their size and move to another row when the available screen width becomes smaller.

---

## Part 2 — CSS Grid Layout and Image Gallery

**Files:**
- `index1.html`
- `style1.css`

The second part demonstrates a complete page layout using **CSS Grid**.

The page contains:

- Header
- Sidebar
- Main content
- Image gallery
- Footer

### Grid Structure

The page uses named grid areas:

```css
.pagegrid {
    display: grid;
    grid-template-columns: 220px 1fr;
    grid-template-rows: auto 1fr auto;

    grid-template-areas:
        "header header"
        "sidebar main"
        "footer footer";
}
```

This creates a layout where the sidebar is placed on the left and the main content is placed on the right.

### Image Gallery

The gallery also uses CSS Grid:

```css
.gallery {
    display: grid;
    grid-template-columns: 200px 200px 200px;
    grid-auto-rows: 200px;
    gap: 18px;
}
```

The images include hover effects. When the user moves the cursor over an image, it scales up and the image caption becomes visible.

---

## Part 3 — Portfolio Layout

**Files:**
- `index2.html`
- `style2.css`

The third part creates a portfolio-style webpage for **Omar Zhakiya**.

The page contains:

- Sticky navigation header
- Portfolio/project section
- Three project cards
- About section
- Contact section
- Footer

### Project Cards

Each project contains:

- Project image
- Project title
- Description
- "View project" button

Example projects include:

1. Atmospheric Narrative Engine
2. IoT Urban Garden Network
3. Accessibility-Focused Code Reviewer

### Grid + Flexbox

The main page structure uses CSS Grid:

```css
.layoutgrid {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 32px;
}
```

The individual project content uses Flexbox:

```css
.projectbody {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```

This demonstrates how **CSS Grid and Flexbox can be used together**.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and semantic elements |
| CSS3 | Styling and layouts |
| Flexbox | Navigation, cards, and component layouts |
| CSS Grid | Page and gallery layouts |
| CSS Transitions | Smooth hover animations |
| Images | Visual content for cards, gallery, and projects |

No JavaScript or external libraries are required.

---

## How to Run

### Option 1 - Open directly

1. Download or extract the project.
2. Open the `Assignment2Frontend-main` folder.
3. Double-click `index.html`.
4. The first part of the assignment will open in your browser.

You can also open:

```text
index1.html
```

for Part 2, or:

```text
index2.html
```

for Part 3.

### Option 2 - Using VS Code

1. Open the project folder in **Visual Studio Code**.
2. Open `index.html`.
3. Use the **Live Server** extension if installed.
4. Open the page in your browser.

---

### Option 3 - Github Pages

1. Open the repository in your **Github**.
2. Navigate to "Settings" option.
3. Open "Pages" button.
4. Open "Github Pages" live page link.

## Navigation

The first page contains links to the other assignment parts:

```html
<nav>
    <a href="index1.html">Part2</a>
    <a href="index2.html">Part3</a>
</nav>
```

Therefore, the project can be viewed as three separate demonstrations:

```text
index.html
    │
    ├── Part 1 — Flexbox Cards
    │
    ├── index1.html
    │       └── Part 2 — CSS Grid + Gallery
    │
    └── index2.html
            └── Part 3 — Portfolio Grid + Flexbox
```

## Learning Objectives

This project demonstrates practical understanding of:

- Using Flexbox for one-dimensional layouts
- Using CSS Grid for two-dimensional layouts

## Author

**Omar Zhakiya**

Frontend Development Assignment 2

© 2026
