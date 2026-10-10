# Assignment 2

## Part A: Concept Questions

### Question 1 (4 marks)
What does "responsive design" mean? Give two reasons why it matters.

#### Answer
Responsive design means creating a website that automatically adapts its layout, text, and spacing to fit different screen sizes and devices, such as phones, tablets, and desktops.

Two reasons it matters are:
1. Better user experience: users can read and navigate the site easily on any device without zooming or horizontal scrolling.
2. Higher reach and engagement: since many people browse the web on mobile devices, a responsive site keeps visitors engaged and reduces the chance they leave because the layout is broken or difficult to use.

### Question 2 (4 marks)
Explain the "mobile-first" approach. Why do many developers prefer it to designing for desktop first?

#### Answer
The mobile-first approach means designing and building the website for small screens first, then adding more styles as the screen gets larger. This makes the base layout simple, focused, and optimized for the most constrained device.

Many developers prefer it because:
1. It keeps the code cleaner and easier to manage: start with a simple single-column layout and expand it for larger screens instead of removing complexity from a desktop layout.
2. It prioritizes important content: on mobile, space is limited, so designers must focus on what matters most.
3. It matches real traffic patterns: mobile usage is often higher than desktop, so it gives the main audience the best experience first.

### Question 3 (4 marks)
Why do we prefer units like `%`, `rem`, and `vw` over `px` for values that should adapt? Give one situation where `px` is still a sensible choice.

#### Answer
We prefer `%`, `rem`, and `vw` because they scale more naturally across different screen sizes and user settings. `%` adapts to the parent container, `vw` adapts to the viewport width, and `rem` scales based on the browser’s root font size, which helps support accessibility and responsive typography.

`px` is still sensible for small, precise values where exact control is important, such as border thickness, icon sizes, or carefully aligned pixel-based design details.

### Question 4 (4 marks)
What does `box-sizing: border-box` do, and why do we put it at the start of a stylesheet?

#### Answer
`box-sizing: border-box` makes the width and height of an element include its padding and border, instead of adding them on top. This means the element keeps the size you set, and content area shrinks to fit inside it.

We put it at the start of the stylesheet because it gives a predictable layout foundation for all elements, which makes responsive design easier and prevents unexpected overflow caused by padding and borders increasing an element’s total size.

### Question 5 (5 marks)
Flexbox lays out items in a single direction. What is the difference between the main axis and the cross axis, and how does `flex-direction: column` change them?

#### Answer
The main axis is the direction in which flex items are placed and distributed. The cross axis is perpendicular to that direction. For example, in a row layout, the main axis is horizontal and the cross axis is vertical.

When `flex-direction: column` is used, the main axis becomes vertical and the cross axis becomes horizontal. This means items stack from top to bottom instead of left to right, and alignment properties like `justify-content` now work vertically while `align-items` works horizontally.

### Question 6 (4 marks)
What is the difference between `align-items` and `align-content`? Under what condition does `align-content` have any effect?

#### Answer
`align-items` aligns flex items within a single line along the cross axis. It controls how items are positioned relative to each other in one row or column.

`align-content` controls spacing and alignment between multiple lines of flex items when the container wraps onto more than one line. It has any effect only when `flex-wrap: wrap` (or `wrap-reverse`) is used and the flex container has multiple rows or columns, creating extra space along the cross axis.

