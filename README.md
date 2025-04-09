# Responsive Flexbox Gallery Tutorial

Learn how to create a responsive photo gallery using CSS Flexbox. This tutorial covers fundamental layout techniques
suitable for HTML/CSS beginners.

## Live Demo
[View on GitHub Pages](https://github.com/Confusemoon/Flexbox-Photo-Gallery-Tutorial)

## Features
- Responsive grid layout
- Hover effects
- Mobile-first approach
- Flexible card components

## Technologies
- HTML5
- CSS3 (Flexbox)

## Installation
```bash
git clone https://github.com/Confusemoon/Flexbox-Photo-Gallery-Tutorial.git
cd responsive-flex-gallery
open index.html
```

# Step-by-step tutorial and Code Explanation:

## 1.HTML Structure
### Create the basic gallery container and card components:

```html
<div class="gallery-container">
    <div class="gallery-card">
        <img src="image.jpg" alt="Description">
        <div class="caption">Image Title</div>
    </div>
    <!-- Add more cards -->
</div>
```

## 2.Flexbox Container
### Style the parent container for responsive flex layout:

```css
.gallery-container {
    display: flex;
    flex-wrap: wrap;
    gap: 1.5rem;
    justify-content: center;
    padding: 2rem;
}
```

### 3.Responsive Cards
### Create flexible cards with size constraints:

```css
.gallery-card {
    flex: 1 1 300px; /* Flex-grow | Flex-shrink | Flex-basis */
    max-width: 400px;
    background: #fff;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}
```
### 4. Add Hover Effects
### Enhance interactivity with CSS transitions:

```css
.gallery-card {
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.gallery-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0,0,0,0.15);
}
```
## Customization
### Modify these properties to match your needs:
```css
/* Change columns */
.gallery-card { flex-basis: 250px; }

/* Adjust spacing */
.gallery-container { gap: 2rem; }

/* Modify card appearance */
.gallery-card {
    background: #f8f9fa;
    border-radius: 12px;
    border: 1px solid #dee2e6;
}
```

## Customization

1, Change columns: Adjust flex-basis value

2, Modify spacing: Update gap property

3, Change card style: Edit background/border-radius

## CSS transitions

1, Media queries

2, Modern layout techniques
