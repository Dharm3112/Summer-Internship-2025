# CSS Grid Project - Testimonials Grid Section

A responsive testimonials grid layout built using **HTML5** and **CSS Grid**. This project demonstrates the power of CSS Grid for creating complex, two-dimensional layouts that adapt seamlessly to different screen sizes.

## 📂 Project Structure

  * **`index.html`**: The main HTML structure containing the testimonial cards.
  * **`style.css`**: Stylesheet handling the grid layout, card styling, and responsiveness.
  * **`images/`**: Contains profile pictures and background patterns (e.g., `bg-pattern-quotation.svg`).

## ✨ Features

  * **CSS Grid Layout**: Utilizes `grid-template-columns`, `grid-column` spanning, and `grid-row` spanning to create a masonry-style layout on desktop screens.
  * **Responsive Design**: transitions from a 4-column complex grid on large screens to a single-column stacked layout on mobile devices (max-width: 768px).
  * **Card Components**: Distinct card styles with varying background colors (Purple, Gray-Blue, Black-Blue, White) and typography.
  * **Custom Typography**: Uses the 'Barlow Semi Condensed' font family.

## 🛠️ Technologies Used

  * **HTML5**
  * **CSS3** (CSS Grid, Flexbox for internal card alignment)

## 🚀 How to Run

1.  Clone or download this repository.
2.  Navigate to the `CSS Grid Project` folder.
3.  Open `index.html` in any modern web browser (Chrome, Firefox, Edge, etc.).

## 📖 Code Highlights

The core of the desktop layout is defined in `style.css`:

```css
.testimonials {
    display: grid;
    grid-template-columns: repeat(4, 1fr); /* 4 Column Grid */
    gap: 30px;
}

/* Spanning the first card across two columns */
.card:nth-of-type(1) {
    grid-column: 1/3;
}

/* Spanning the tall card across two rows */
.card:nth-of-type(5) {
    grid-column: 4/5;
    grid-row: 1/3;
}
```

## 📱 Mobile Responsiveness

On screens smaller than 768px, the layout simplifies to a single column:

```css
@media(max-width: 768px) {
    .testimonials {
        grid-template-columns: 1fr;
    }
}
```

## 🎓 Acknowledgments

  * **Learning Source**: [Sahajanand Digital](https://github.com/sahajananddigital)
    
  * **Concept**: Based on a common frontend challenge (Testimonials Grid Section) to practice CSS Grid skills.
    
  *  **Done By [Dharm Patel](https://github.com/Dharm3112)**
