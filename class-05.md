# Read: 05 - HTML Images; CSS Color & Text

# ***HTML Images***

## What is the resons to put images in your web?
## you might want to include a logo, photograph, illustration, diagram, or chart.


![img](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2020/07/html-images-df.jpg)
## CHOOSING IMAGESE YOUR SITE
### A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.

## STORING IMAGES ON YOUR SITE
### If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.

## ADDING IMAGES
<***img***> To add an image into the page you need to use an <***ing***> element.
## It must carry the following two attributes:

* ***src*** : This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.

* ***alt*** : This provides a text description of the image which describes the image if you cannot see it.
![img1](https://cdo-curriculum.s3.amazonaws.com/media/uploads/img_tag.png)


## height and width of images
### there are two  attributes we use it to  specify its size

* height :This specifies the height of the image in pixels.

* width : This specifies the width of the image in pixels

three rules for creating images


## Where an image is placed in the code ?
* befor a paragraph
* inside the start of a paragraph
* in the middle of a paragraph 

## what is the rules to creating imges ?
* Save images in the right format ex *** test.png***
* Save images at the right size 
* Use the correct resolution

## notes for img
* the <***img***> element is used to add images to a web page
* you must always specify a **src** attribute indicate the source of an image
* you should save images at the size you will be using them on the web page and in the appropriate format
* photograghs are best saved as **JPEGs** illustrations or  logos that use flat colors are better saved as **GIFs**

## CSS Color & Text
### Color can really bring your pages to life So we need CSS to help us to make the page colorful and beautiful


## Foreground Color
### There are 3 ways to define colors
* rgb values
  * These express colors in terms of how much red, green and blue are used to make it up. *** For example: rgb(100,100,90) *** 

* hex codes
  * These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash #sign. *** For example: #ee3e80***

* color names
  * There are 147 predefined color names that are recognized by browsers. ***For example:DarkCyan***
    ![color](https://images.sampletemplates.com/wp-content/uploads/2015/06/Css-Color-Code-Chart.jpg)

      ##  Background Color
### CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.
#### You can specify your choice of background color in the same three ways you can specify foreground colors:
 * RGB values
* hex codes
*  color names
  
  ## Every color on a computer screen is created by mixing amounts of red,green, and blue. To find the color you want, you can use a color picker.

  ![rgb](https://t7m8e9c8.rocketcdn.me/wp-content/uploads/2020/07/colores-rgb.jpg)

## notes for colors 

* Color not only brings your site to life, but also helps convey the mood and evokes reactions. 
*
* There are three ways to specify colors in CSS: RGB values, hex codes, and color names. 
* Color pickers can help you find the color you want.
 
 * CSS3 has introduced an extra value for RGB colors to indicate opacity.  It is known as RGBA. 
 * CSS3 also allows you to specify colors as HSL values, with an optional opacity value.  It is known as HSLA.

# text

## TYPEFACE TERMINOLOGY

* **SERIF** Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
* **SANS-SERIF** Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
* **MONOSPACE** Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

## The xyz 
* WEIGHT 
   * Light -Medium - Bold -Black
* STYLE
  *  Normal -Italic- Oblique

* STRETCH
   *  Condensed- Regular= Extended


    ## **CHOOSING A FOR YOUR WEBSITE TYPEFACE** When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

* **SERIF Serif*** fonts have extra details on the end of the main strokes of the letters,

* **SANS-SERIF**  Sans-serif fonts have straight ends to letters and therefore have a much cleaner design.

* **SPECIFYING TYPEFACES font-family** The font-fanily property allows you to specity the typeface that shouid be used for any text inside the element(s) to which a CSS rule applies.


## PIXELS
### Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px. PERCENTAGESs The detault size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.

## notes for text
* There are properties to control the choice of font, size, weight, style, and spacing. 
*  There is a limited choice of fonts that you can assume most people will have installed. 
* If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them. 
* You can control the space between lines of text, individual letters, and words. Text.can also be aligned to the left, right, center, or justified. It can also be indented. 
*  You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

![text](https://www.tutorialbrain.com/wp-content/uploads/2019/02/Font-in-HTML.jpg)