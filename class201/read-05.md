# Images
***There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.***

## Choosing Images for Your Site
**A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.**

## Storing Images on Your Site
**If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.**

## Adding Images
**'< img >':To add an image into the page you need to use an '< img >' element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:**

## Where to Place Images in Your Code
- **before a paragraph The paragraph starts on a new line after the image.**
- **inside the start of a paragraph The first row of text aligns with the bottom of the image.**
- **in the middle of a paragraphThe image is placed between the words of the paragraph that it appears in.**

## Three Rules for Creating Images
1. **Save images in the right format.**
2. **Save images at the right size.**
3. **Use the correct resolution**

## Image Dimensions
**The images you use on your website should be saved at the same width and height that you want them to appear on the page.**

## Cropping Images
**When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.**

## Image Resolution
**Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.**

## Vector Images
**Vector images differ from bitmap images and are resolution-independent. Vector images are commonly created in programs such as Adobe Illustrator.**

## Animated GIFs
**Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.**

## Transparency
**Creating an image that is partially transparent (or "see-through") for the web involves selecting one of two formats:**
- **Transparent GIF: If the transparent part of the image has straight edges and it is 100% transparent (that is, not semi-opaque), you can save the image as a GIF (with the transparency option selected).**
- **PNG: If the transparent part of the image has diagonal or rounded edges or if you want a semiopaque transparency or a dropshadow, then you will need to save it as a PNG.**

## Figure Caption
**'< figure >':Images often come with captions. HTML5 has introduced a new '< figure >' element to contain images and their caption so that the two are associated. You can have more than one image inside the '< figure >' element as long as they all share the same caption.**

# Color

**How to specify colors, as there are three common ways in which you can indicate your choice of colors:**
- RGB: Values Values for red, green, and blue are expressed as numbers between 0 and 255. "rgb(102,205,170)"
- Hex Codes: Hex values represent values for red, green, and blue in hexadecimal code."#66cdaa"
- Color Names: Colors are represented by predefined names. However, they are very limited in number."MediumAquaMarine"
## Contrast

**When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.**
- Low Contrast: Text is harder to read when there is low contrast between background and foreground colors. 
- High Contrast: Text is easier to read when there is higher contrast between background and foreground colors.
- Medium Contrast: For long spans of text, reducing the contrast a little bit improves readability.

## Opacity

***CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).***

***Color pickers can help you find the color you want.***


# Text
***The formatting of your text can have a significant effect on how readable your pages are. As we look through these properties I will also give you some design tips on how to display your type.***

## Techniques That Offer a Wider Choice of Typefaces
**There are several ways to use fonts other than those listed on the previous page. However, typefaces are subject to copyright, so the techniques you can choose from are limited by their respective licenses.**

## Specifying Typefaces
- **The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.**
- **The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:pixeles , percentage ,etc.....**
- **@font-face allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.**

## Underline & Strike
**The text-decoration property allows you to specify the following values:**
- **none: This removes any decoration already applied to the text.**
- **underline: This adds a line underneath the text.**
- **overline: This adds a line over the top of the text.**
- **line-through: This adds a line through words.**
- **blink: This animates the text to make it flash on and off (however this is generally frowned upon, as it is considered rather annoying).**

## Some definitions
- **Leading (pronounced ledding) is a term typographers use for the vertical space between lines of text. In a typeface, the part of a letter that drops beneath the baseline is called a descender, while the highest point of a letter is called the ascender. Leading is measured from the bottom of the descender on one line to the top of the ascender on the next.**
- **Kerning is the term typographers use for the space between each letter. You can control the space between each letter with the letter-spacingproperty.**
- **The text-align property allows you to control the alignment of text. The property can take one of four values:**
- **The vertical-align property is a common source of confusion. It is not intended to allow you to vertically align text in the middle of block level elements such as '< p >' and '< div >', although it does have this effect when used with table cells (the '< td >' and '< th >'elements).**
- **The text-indent property allows you to indent the first line of text within an element. he amount you want the line indented by can be specified in a number of ways but is usually given in pixels or ems.**
-**The text-shadow property has become commonly used despite lacking support in all browsers.**

> **Note: You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.**