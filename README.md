# css-tutorial
## css grid and positioning 

**Block vs Inline**
- Block elements behave like paragraphs and Inline elements behave like words
- `span` is Inline by default while `h1`, `p`, and `div` are block by default
- Think inside the box: Every element is a box
- every of those boxes is into 4 parts: Padding, Content, Border and Margin
- *Abbreviated as: Please Come Be Mine*
- **Padding** and **Margin** are often used 
- *Margin*: Keeps other boxes at a distance from its box
- Position values: static, relative, absolute, fixed, sticky
-  `fr`: "units of free space" basically instruct the grid to divide untaken
space proportionally between rows and columns that are in fr units

## Units of measurements
- The major ones are px(pixels) and em(current font size of the element relative to some base font)
- body{
    font-size: 18px
}
- h1 {
    font-size: 1.6em
}   
- Meaning the `h1` should scale 1.6 times the base font of the body. so we ever decide to change the base font of the body the `h1` font will scale accordingly