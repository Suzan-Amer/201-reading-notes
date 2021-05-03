# Read: 08 - More CSS Layout

# CSS Layout

## Key Concepts in Positioning Elements
### Building Blocks CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. Containing Elements If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

* ***block-level elements ***
   * start on a new line ex: <**h1**> <**p**> <**ul**> <**li**>
* ***inline element  ***   
   * flow in between suprouning text ex : <**img**> <**b**> <**i**>


## Controlling the Position of Elements
### CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property. To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.


![css](https://bs-uploads.toptal.io/blackfish-uploads/uploaded_file/file/197755/image-1583190798408-7af80aeb943477b9375814bc95245a4e.png)

## we have 3 position ic css :
## 1- position static
### normal flow, each block-level element sits on top of the next one.

## 2- position:absolute
### When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page

## 3-position:fixed
### Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

![pos](https://i.ytimg.com/vi/BVIdzytAtkg/maxresdefault.jpg)


## clering floats 
## clear 
### The clear property allows you to say that no element (within  the same containing element) should touch the left or right-hand sides of a box. It can take the following values:
* left 
   * The left-hand side of the box  should not touch any other elements appearing in the same containing element.
* right
   * The right-hand side of the box will not touch elements appearing in the same containing element.
* both
   * Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.
* none
   * Elements can touch either side.   


## Creating Multi-Column Layouts with Floats   
### Many web pages use multiple columns in their design. This is achieved by using a <**div**>element to represent each column. The following three CSS properties are used to position the columns next to each other: 
* width
  * This sets the width of the columns.
* float
  * This positions the columns next to each other.
* margin
  * This creates a gap between the columns.
 
## Screen Sizes
### Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

## Screen Resolution
### Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

## Layout Grids
### While a grid might seem like a restriction, in actual fact it:
* Creates a continuity between different pages which may use different designs
* Helps users predict where to find information on various pages
* Makes it easier to add new content to the site in a consistent way
* Helps people collaborate on the design of a site in a consistent way

![img](https://i.pinimg.com/originals/46/ed/1e/46ed1ea7060089aa46ec32af3d1eb55b.png)



