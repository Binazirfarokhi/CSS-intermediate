# CSS-intermediate
Create a nice layout with CSS
In this week we are going to cover the intrmediate CSS styling : 
Today’s lesson: 
Visual studio code 
 

We are going to talk about the EMMET Equation: 
https://docs.emmet.io/cheat-sheet/

Child >
Sibling + 
Level up  ^ 
Multiple  * 
Literal text {} 
Add class .
Add ID #
 Different measurement in css style: 




CSS font-size : 
Best Practices for Choosing Units:
Use rem for consistent, scalable font sizes.
The default size of the root element is 16 px, now 4 rem means 4*16 : 64 px


Use viewport units (vh, vw) for responsive layouts.
Use px for precise, fixed designs or where scaling isn’t needed.
Use em for component-level scaling when child elements depend on parent sizes. Em is proportional to the font size of the  current element. It follows what the parent  element size is and then applies  the proportion. 1.5em * 16 
% (Percentage)Definition: Relative to the font size of the parent element. It will look at the parent and fix its content to that area.




Use % for the width and vh for the height

CSS box model means margin padding and border 
Padding : add space between contents of the box and the edge of the box
Margin: add space around the outside of the box. 
Border is outside of the padding 

box-sizing=border-box 
Makes it easier to control layouts.
Total size of an element remains consistent even when padding or borders are added.


We have different margin for different layout : more specific: 
Margin can be top right bottom left 

Padding as well. Is the same as the margin 
Body{
Margin:0}


Preferences: !important > inline > IDs > classes > elements 

https://www.w3schools.com/css/css_boxmodel.asp



Classes- IDs - Fragment Identifier 
.
#



  Classes are used to label HTML elements with a name; you can use classes to select HTML elements in CSS. Many HTML elements can have the same class.
               <h2>IDs</h2>
An ID is used to label a single element in a page. You can use as many IDs as you want, but each ID can be used only once. IDs can be used to link to different parts of your page with anchor tags.



        <h2>Fragment Identifiers</h2>

     One can make a link to an element with a particular ID by adding the ID to the end of the URL, prefixed by a #. For example: http://langara.ca#some-id (Takes you to the part of the page with id="some-id"

The more classes the more specificity you will have. 

Preferences: !important > inline > IDs > classes(more classes more specific) > elements 
If the selector specificity is the same then the order matters in the html and css codes.

Specificity calculation : 
(NO. of Ids, NO. of classes, NO. of elements)
Fragment Identifiers on URIs: 
Adding the id of the element to the end of the URL. for instance: http://langara.ca#tag-id
Example: http://langara.ca#tag-id
The browser will scroll to the element with the id="tag-id" on the page.
==========================
Week 4 : css box model and box-sizing




Use margin to make space around element :
If two margins overlap each other , the margin with higher  value will be applied to the code.






Use padding to make space inside the elements : 
If you give only two values t padding will be up and down the first one and the second one will be left and right.
Padding: 1rem 0;


Margin:auto will make the content centered in the content of its parent. If only the element you targeted is smaller than window,
Use a border to show the edge of the element.

Box-sizing: content-box is the default value of this property.
Now if you apply a width on a box and use this property that box-sizing:border-box it will include the padding and the border  with the width you applied.(if you do not use this it looks like that box is bigger than normal, but once you apply the border-box everything will be included in the box you have added.)  
The width of the content is just the width of that content. But the width of the container is included with padding and border.

Display: In-line and inline-block & block and none: 
https://developer.mozilla.org/en-US/docs/Web/CSS/display


https://www.digitalocean.com/community/tutorials/css-display-inline-vs-inline-block


Which elements have display blocks? They stack on top of each other. 
H1 h2 h4 
Div 
Header 
Nav 
UI
Li 
By default take all available horizontal space unless width is specified.they line up vertically

Css box model properties works as one would expect
. 



Inline-elements: 
We can not apply width and height to the element, they can not go beyond their content that's why 
Margin just apply to left and right 
You can apply border 


Anchor tags are inline elements.
Span
A
Strong 
Em
Img
Br
Input
Cite
small
There is no effect of width on the inline elements.
Similarly, for height also,
If you add padding or border they will overlap that on the other elements around them.
We can make our anchor tags or our inline elements block elements. 
Span is an inline element.
Inline-block: you can add padding - border - width and height. 
So it is a kink of mix of inline and block elements.
If you apply margin to the inline elements it will just apply to the right and left. Will not apply to the bottom and top.
Display :none; remove the elements form the user view.
Centering the elements : 
Max-width : 400px ; 
Margin : auto;



