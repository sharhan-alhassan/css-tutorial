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

## Reading attribute values
- `padding: 10px :` means for all sides (top, right, bottom, left)
- `padding: 10px 3px 4px 32px:` for all the sides starting with top, right, bottom, left
- `padding: 23px 34px 32px:` for top, right/left and bottom 

## CSS Grip Template 
- grid-template-columns: this property defines the number of columns in your grid layout, and it can define the width of each column. Use `auto` if all columns should have the same width
- grid-template-row: property defines the height of each row 
- `Box-sizing`: property allows to include the `padding` and `border` in an element's total width and height
- NB: **A responsive page has a width of 100% for the entire page**

## Media queries
- Design for mobile first: min-width
- `@media only screen and (min-width: 500px)`
- NB: use opposite logic for `min-width` and `max-width`
- *min-width*: if screen is **min-width** or MORE
- *max-width*: if screen size is **max-width** or LESS

## Bootstrap 4 notes:
- If you wanted for the 2 columns to go on the same line starting with `larger mobile phones (>= 576px) you would use col-sm, for tablets (>= 768px) .col-md and for extra large screens (>= 1200px) .col-xl.`
- Grid system
- [Alt text](images/bootstrap-grid.png)
- NB: Boostrap is designed for mobile friendly at first. So design for your device coming backwards from the right to the left
- Eg: <div class="col-sm-6 col-lg-3"> x 4 of them
- Meaning: For mobile first, pack all the 4 columns on each other, that is 1 column in a row 
- For small devices(sm), 2 columns in a row
- For large devices(lg), 4 columns in a row
# Offseeting columns
- If you don’t want your columns to be next to each other, you can use the class .offset-[breakpoint]-[size]together with the .col-[breakpoint]-[size]. Using this class is the same as adding an empty column before your column
- Eg: <div class="col-sm-4 offset-sm-4"> will great an empty column occupying first 4 spaces before it 