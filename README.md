# Travel Blog

### A simple single page static website built with HTML and CSS.

## Learning outcomes:

- Use of HTML elements like image, paragraph, forms, buttons, anchor tags and so on
- Use of Flexbox css for designing the webpage layout
- Implementation of different css selectors like class selector, id selector, desendent combinator, grouping selector

## Challenge faced and steps taken :

1. Header section:

   - Problem:
     - Presenting top-bar text and icon right and left with equal gaps on right and left of text
     - Presenting nav-bar logo and menu list right and left with equal gaps on right and left
     - Highlight nav menu on hover
   - Solution:
     - For equal left and right space, apply padding of 100px on both top-bar and nav-bar
     - use display: flex; and justify-content: space-between; on both top-bar and nav-bar
     - use pseudo class selector li:hover property to implement highlight nav menu on hover

2. Hero section:

   - Problem:
     - displaying a partial transparent box on center with text with image on background
   - Solution:
     - First approach,
       - use position: relative for main section and position: absolute for box to place on center
     - Second approach,
       - use background-image property to set image background
       - use flex box to display box on center
     - For transparent box either use background: rgba or opacity;

3. Blog Cards section:
   - Problem:
     - Background image
     - Display partial transparent cards which contains image on left and content on right, also contents arraged in vertical manner where button is aligned right, also buttons contains shadow and border of cards and buttons has radius
     - Display filter section lists on trasparent box
     - Arrange all cards on left and filters on right
   - Solution:
     - For transparent box either use background: rgba or opacity as before and background-image for image on back;
     - Designing Card:
       - Use display:flex; for card with image and content aligned right and left
       - use display: flex; and flex-direction: column; on content to display it vertically;
       - wrap button into a div and use display: flex; with justify-content: end; to display it on right
       - use border-radius: 6px; to achieve border radius
       - use box-shadow: -8px 8px 16px 6px <color>; i.e. horizontal-value vertical-value blur spread-radius color;
   - To arrange cards and filters on left and right, wrap both the container in single one and use display: flex; with gap: 10px;
