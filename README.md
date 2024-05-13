<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  

- [CSS BOX MODEL](#css-box-model)
  - [What is the CSS Box Model?](#what-is-the-css-box-model)
  - [**Content Area**](#content-area)
    - [Elements of the width and height](#elements-of-the-width-and-height)
    - [Total Width Calculation](#total-width-calculation)
    - [Total Height Calculation](#total-height-calculation)
  - [**Padding Area**](#padding-area)
  - [**Border Area**](#border-area)
  - [**Margin Area**](#margin-area)
    - [Margin Values](#margin-values)
  - [Conclusion](#conclusion)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# CSS BOX MODEL

**CSS Box Model** is a Fundamental concept in CSS that governs how elements are structured and positioned on a webpage. By learning this model, you’ll create elements visually appealing that adjust seamlessly to various screen sizes. It is used to create the design and layout of web pages.

*In this article, we’ll learn the key components of the box model and its practical implications.*

## What is the CSS Box Model?

**The box model in CSS** is a container that contains various properties, including borders, margins, padding, and the content itself. These properties collectively determine the dimensions and spacing of an element.

The following figure illustrates the Box model in CSS.
![a cssmodel box example](tools/css-box-model.png)


Let’s break down the key components:
 - **Content:** The actual data in text, images, or other media forms can be sized using the width and height property. 
 - **Padding:** Padding is used to create space around the element, inside any defined border.
- **Border:** The border is used to cover the content & any padding, & also allows setting the style, color, and width of the border.

 **Margin:** Margin is used to create space around the element ie., around the border area.
 
 ***

 ![a html webpage showing css box implementation](tools/box.png)

 ***
 
## **Content Area**
Contains the actual data, such as text, images, or other media.
Sized using the width and height properties.
Bounded by the content edge.
### Elements of the width and height
Typically, when you assign the width and height of an attribute using the CSS width and height assets, it means you just positioned the height and width of the subject areas of that component. The additional height and width of the unit box is based on a range of influences.example in code
```CSS
p {
    width: 50%;
    height: 50%;
    margin: 40px;
    border: 40px solid black;
    padding: 40px;
}
```
### Total Width Calculation
Total element width = width + left padding + right padding + left border + right border

Total width of the element is 94px.
Total width = 80px (width) + 40px (left padding + right padding) + 40px (left border + right border) = 94px.
### Total Height Calculation
Total element height = height + top padding + bottom padding + top border + bottom border

Total height of the element is 84px.
Total height = 70px (height) + 40px (top padding + bottom padding) + 40px (top border + bottom border) = 84px.

## **Padding Area**
Surrounds the content area.
Space within the border box.
Dimensions are determined by the width and height of the padding box.
CSS has properties for specifying the padding for each side of an element:

 - padding-top
 - padding-right
 - padding-bottom
 - padding-left

All the padding properties can have the following values:

- **length** - specifies a padding in px, pt, cm, etc.
% - specifies a padding in % of the width of the containing element
- **inherit** - specifies that the padding should be inherited from the parent element
- **Note:** *Negative values are not allow*
 ```css
 p {
  padding-top:    40px;
  padding-right:  40px;
  padding-bottom: 40px;
  padding-left:   40px;
}
```
## **Border Area**
Lies between the padding and margin.
Width and height are defined by the border.
CSS borders are essential elements in websites, representing the edges of various components and elements.

 CSS Borders refer to the lines that surround elements, defining their edges. Borders can be styled, colored, and sized using CSS properties such as border style, border color, border width, and border radius. borders can be styled with the top border, the right border, the bottom border, and the left border.
 ```css
 p {
   
    border-top: 40px;
    border-left: 40px;
    border-right: 40px;
    border-bottom: 40px;
  }
  ```
## **Margin Area**
Separates the element from adjacent elements.
Dimensions specified by the margin-box width and height.
The CSS margin property allows us to create space around an element. They define the gap between an element and its neighboring elements. Margins can be set individually for each side (top, right, bottom, left).

### Margin Values
Length (e.g., px, rem, em, ex, vh, vw, etc)
Percentage (relative to the element’s width)
auto (calculated by the browser)
margin allows negative values.

**Margin Properties**
- **margin-top:** Sets the top margin of an element.
- **margin-right:** Sets the right margin of an element.
- **margin-bottom:** Specifies the margin at the bottom of an element.
- **margin-left:** Determines the width of the margin on the left side of an element.
example of code
```css
div {
    width: 50%;
    height: 50%;
    border: 40px solid black;
    padding: 40px;
    margin-top: 40px;
    margin-top: 40px;
    margin-top: 40px;
    margin-top: 40px;
}
```
## Conclusion
In conclusion, mastering the CSS box model is foundational for web development, as it lays the groundwork for precise layout and styling. By understanding how elements are structured and how properties such as padding, margin, border, and content interact, developers can create visually appealing and responsive designs. Through this documentation, we have explored the intricacies of implementing the CSS box model effectively, from its basic principles to advanced techniques. Armed with this knowledge, developers can confidently manipulate layout and presentation, ensuring their web projects are both visually striking and functionally robust.
