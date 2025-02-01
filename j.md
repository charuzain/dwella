Grids and flexbox cheat sheet
Note: ‘|’ stands for alternatives or OR.

Grid 
The syntax for creating a grid:

321
selector{
    display: grid; /* or inline-grid */
}
Grid shorthand consists of the following properties with default values:

grid

A grid will allow you organize the various elements on your page. 

grid-template-rows: none

This feature allows you configure your elements so that they are organized similarly to rows on a table. 

grid-template-columns: none

This feature allows you configure your elements but with this setting the elements are organized like columns on a table. 

grid-template-areas: none

This feature allows you configure the names of a grid and how they sit in relation to one another. 

grid-auto-rows: auto

Default setting for all row sizes that have not been explicitly configured. 

grid-auto-columns: auto

Default setting for all column sizes that have not been explicitly configured. 

grid-auto-flow: row

Default location for rows that are not explicitly allocated. 

column-gap: normal

This sets the gap between the columns

row-gap: normal

This sets the gap between the rows

Grid properties for container
grid-template-columns: measurement units | % units |repeat()

Defines the line names, and maintains a constant size of column items. Can accept a range of different measurement sizes.

grid-template-rows: measurement units | % units |repeat()

Defines the line names, and maintains a constant size of rows. Can accept a range of different measurement sizes.

grid-auto-columns: measurement unit (fixed value for all columns)

Determines the default size for columns that have not been explicitly configured. 

grid-auto-rows: measurement unit (fixed value for all rows)

Determines the default size for rows that have not been explicitly configured.

grid-template: “header header” auto

This allows you define and maintain named cells on a grid 

“main right” 75vh

This defines two cells named main and right, that have a sizing of 75% of the viewport height. 

“footer footer” 20rem

This defines two cells named footer and footer, that have a sizing of 20 root em (rem). This defines the size in relation to the html font size. 

Gap
grid-gap: measurement units

Determines the gap between rows and columns 

grid-column-gap: measurement units

Determines the gap between columns

grid-row-gap: m-unit-1  m-unit-2

Determines the gap between columns

Alignment
justify-items: start | center | end | stretch

Defines the default space that is allot to each item on the grid 

align-items: start | center | end | stretch

Defines the default space related to an item along the grid’s block axis  

place-items: start | stretch /* shorthand for two properties above */

This feature allows you align items with  the block and inline directions.

Justification
justify-content: start | center | end | stretch | space-between | space-evenly | space-around

Defines browser allocation of space to content items in relation to the main-axis 

align-content: start | center | end | stretch | space-between | space-evenly | space-around

Defines browser allocation of space to content items in relation to cross axis and block axis  

place-content: center | start

This feature allows you align items with  the block and inline directions.

Positioning
grid-auto-flow: row | column | dense

This relates to how the items are placed automatically within the grid

grid-auto-columns: measurement units

This relates to the size for columns created without specific size specifications 

grid-auto-rows: measurement units

This relates to the size for rows created without specific size specifications 

Grid properties for items (child)
grid-column: column position /* E.g. 1/2  */

Allows for specifying where on the grid the column is to start. 

grid-column-start: column start position 

This property determines the starting column position an item is placed on a grid. 

grid-column-end: column end position 

This property determines the end column position an item is placed on a grid. 

grid-row: row position /* E.g. 1/2  */

Allows for specifying where on the grid the row is to start. 

grid-row-start: row start position 

This property determines the starting row position an item is placed on a grid. 

grid-row-end: row end position 

This property determines the end row position an item is placed on a grid. 

Justification and alignment
justify-self: start | center | end | stretch

Determines how  an item is positioned inside its aligned container in relation to the appropriate axis. 

align-self: start | center | end | stretch

Aligns an item within a grid area. 

place-self: start | stretch /* shorthand for two properties above */

This setting lets one align and justify an item within a block. 

Flexbox
The syntax for creating a flexbox:

1234
selector{
    display: flex | inline-flex
}

Here the selector can refer to any of the following flex attributes 

Attribute selector

Class Selector

ID Selector 

Type Selectors 

Universal Selectors 

The display relates to how you want the selector to be shown. Setting display to flex makes the given selector a flex box. Setting display to inline-flex makes the selector a flex box container while will be inline. 

Properties for flexbox container
flex-direction: row | row-reverse | column | column-reverse

It is possible to specify the direction your elements will follow. Traditionally text goes from left to right which is flex’s default setting however it can be set from right to left or even top to bottom. The four flex-direction are:

row : organized from left to right 

row-reverse: organized from right to left 

 column: organized from top to bottom

 column-reverse: organized from bottom to top. 

flex-wrap: wrap | nowrap

The standard layout is to plot the elements from left to right in a straight line. The wrap feature allows you customize this to match the size of the window displaying the page. 

wrap: Automatically wrap the items with as the window space gets smaller. 

Nowrap: Default setting, items remain rigid and don’t respond  to adjustments made to the window size.

align-items: flex-start | flex-end | center |Stretch

This determines how the flex items are to be positioned on the page. Items can be aligned in a variety of ways 

Flex-start: Similar to standard writing, items start at the top left-hand corner and are positioned from left to right 

Flex-end: Position begins in the bottom right hand corner. 

Center: Item is positioned from the center. 

Stretch: item expands to fill the container. 

justify-content: flex-start | flex-end | center | space-between | space-evenly


Justify-content determines the alignment of the flex items. 

Flex-start: goes from right to left along the main axis. 

Flex-end: goes from left to right along the main axis. 

Center: Starting at the middle, alignments expands from there. 

Space-between: first and last item are flush with the left and right wall respectively, every other item is evenly spaced. 

Space-evenly: each item is equidistant from each other and the boundary wall 

Properties for flexbox items (child)
flex-grow: factor of flex’s main size  

This attribute enables the flex container to grow proportionally to the other containers present. 

flex-shrink: factor of flex’s main size

This allows elements to shrink in relation to items around it.

flex-basis: auto | factor of main’s size | measurement unit

The sets the initial main size of an item. It can be overridden if other stylized elements are configured. 

order:position in flex /* Set ascending by default */

The standard positioning of items is by source order, however this feature will enable you to configure where the items appear on the page. 

align-self:  start | center | end | stretch

This determines where on the page the child items will be positioned. Similar to the main flex attributes, start is to the left and end is to the right.





Pseudo-elements
Pseudo-elements help you style a specific part of an element. For example, you can decide to apply styling to only the first word or line in a given element. First, let’s examine the syntax of a pseudo-element.

Syntax
selector::pseudo-element {

 property: value; 

}


It is important to note that pseudo-elements use two colon (::) characters instead of one.

Now, let’s explore some examples of popular pseudo-elements.

Setting up the HTML and CSS files
You can practice the pseudo element code blocks below by adding the respective code inside the HTML and CSS files. Additionally, reference the CSS code in HTML by adding a link tag such as:

<link rel="stylesheet" href="style.css">

where style.css is the name of your CSS file. 

Additionally, add the HTML code inside the <body> tag in the HTML file. A sample code block for HTML will appear as below:

567891011124321
<!DOCTYPE html>

<html>
<head>
  <link rel="stylesheet" href="style.css">
</head>

<body>
    <!-- Add your HTML code here -->
</body>

Once both the HTML and CSS code is in place, right click on the HTML file in your VSCode side menu Explorer and select Show Preview. It will open a built-in VSCode Browser where you can preview the code.

Below are a few examples of the different pseudo-elements you can use:

::first-letter
You can use the first-letter pseudo-element to change the color of just the first letter of each of the three points in the example text.

HTML code:

25
<!DOCTYPE html> 

<html> 

    <head> 

        <link rel="stylesheet" href="pseudo4.css"> 

    </head> 


CSS code:

1234567891011
li::first-letter { 

color:coral; 

font-size: 1.3em; 

font-weight: bold; 

line-height: 1; 


Output

The output when the pseudo-element first-letter are used to change the size and color of the first letter of list items.
Although the code only changed the first letter of each bullet point, it makes a big difference in terms of presentation. Now let’s change the font in a different way. 

::first-line
First-line will change the complete first line of each of the bullet points to light sea green. 

CSS code:

34567891021
ul{
    list-style-type: none;
}

li::first-line {
    color: lightseagreen;
    text-decoration: underline;
    line-height: 1;
}

Output:

Display of underlined first line of each bulleted item item
Because it’s only the first line of each bullet point, it almost functions like dividers between the three different points instead of having to rely on bullets.  

Note that the contents of the line to which this pseudo-element is applied will change as you increase or decrease the size of your viewport. 

Output:

Output for the first underlined line in the increased size format of the text
::selection
::selection is another useful pseudo-element. For example, you may use it when you are taking notes on your device because it allows you to highlight specific text. The effect of it becomes obvious only after the user selects content. On web pages today, you will typically see inverted colors from white-black to black-white when selecting a portion of text.

CSS code:

12345678910
ul{
    list-style-type: none;
}

li::selection {
    color:brown;
    background-color: antiquewhite;
    line-height: 1;
}

 Here is an example of a selection of text.

 Output:

Output for selection of text display
And another example of the same text but with a different section selected and highlighted.

Output:

Selection of different part of text display
  Different segments of the text are highlighted depending on the text that is selected at any given point.    

::marker  
::marker is typically used to add style elements to a list, for instance, to color bullet points. For example, you can enhance the user experience when you use a marker in the following way.    

CSS code:

345612
li::marker {
    color: cornflowerblue;
    content: '<> ';
    font-size: 1.1em;
}

Output

Output for the demonstration of markers
  

Now the bullet points are cornflower blue and they have the shape specified in the code.

::before and ::after
One more pair of pseudo-elements are the ::before and ::after pseudo-elements. They allow you to add content before and after an element on which they are allowed. In other words, new content can be added to a page without adding HTML code for it. You can also add styling options for this content. Let’s do an example where text is added both before and after some cooking guidelines to identify them as important tips. 

HTML code:

123456
<body>
    <p id="tips"> Don't rinse your pasta after it is drained. </p>
    <p> Slice the tomatoes. Take the extra efforts to seed them. </p>
    <p id="tips"> Peel and seed large tomatoes. </p>
</body>

CSS code:

1234567891011121314151617
#tips::before{
    background: darkkhaki;
    color:darkslategray;
    content: "Tip:";
    padding-left: 3px;
    padding-right: 5px;
    border-radius: 10%;
}

#tips::after{

Output:

Selection of texts preceding and following a statement
The “content” property is where the text for the guidelines goes. The word “tip” has been added before each guideline thanks to the rules added for tips::before. And, each of the three guidelines now has two exclamation marks after them thanks to the rules added for tips::after. Note how the second <p> element inside the HTML code remains unaffected. You don’t have to use ::before and ::after together like this, but sometimes it is useful to combine them.

Conclusion
The examples covered here illustrate that adding simple code for pseudo-elements can greatly enhance the appearance of websites. There are plenty of other pseudo-elements and some of them are more popular than others. You can follow your own style and explore the creative possibilities that pseudo-classes and pseudo-elements offer.


Additional resources
The following resources will be helpful as additional references in dealing with different concepts related to the topics you have covered in this section.

Broad overview of layouts in CSS

Detailed overview of flexboxes

Detailed overview of grids (1)

Detailed overview of grids (2)

Commonly used selectors

Combinator selectors

Comprehensive list of selectors

Comprehensive list of pseudo-classes

Comprehensive list of pseudo-elements


// -1 works with explicit grid only
//The HTTP POST method is more secure than the HTTP GET method. When a form is submitted using the Post method, the form data is inserted into the content of the HTTP request instead of appended at the end of the URL as is done with the GET method.
