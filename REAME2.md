CSS Rules to Play with:

Working With the width and height Properties

    width Property: This property specifies the width of an element. If you do not specify a width, then the default is set to auto. This means the element will take up the full width of its parent container.
    min-width Property: This property specifies the minimum width for an element.
    max-width Property: This property specifies the maximum width for an element.
    height Property: This property specifies the height of an element. Similarly, the height is auto by default, which means it will adjust to the content inside.
    min-height Property: This property specifies the minimum height for an element.
    max-height Property: This property specifies the maximum height for an element.

Different Types of CSS Combinators

    Descendant Combinator: This combinator is used to target elements that are descendants of a specified parent element. The following example will target all li items inside ul elements.

Example Code

<ul>
    <li>Example item one</li>
    <li>Example item two</li>
    <li>Example item three</li>
</ul>

Example Code

ul li {
    background-color: yellow;
}

    Child Combinator (>): This combinator is used to select elements that are direct children of a specified parent element. The following example will target all p elements that are direct children of the container class.

Example Code

<div class="container">
  <p>This will get styled.</p>

  <div>
    <p>This will not get styled.</p>
  </div>
</div>

Example Code

.container > p {
  background-color: black;
  color: white;
}

    Next-sibling Combinator (+): This combinator selects an element that immediately follows a specified sibling element. The following example will select the paragraph element that immediately follows the h2 element.

Example Code

<h2>I am a sub heading</h2>

<p>This paragraph element will get a red background.</p>

Example Code

h2 + p {
  background-color: red;
}

    Subsequent-sibling Combinator (~): This combinator selects all siblings of a specified element that come after it. The following example will style only the second paragraph element because it is the only one that is a sibling of the ul element and shares the same parent.

Example Code

<div class="container">
  <p>This will not get styled.</p>
  <ul>
    <li>Example item one</li>
    <li>Example item two</li>
    <li>Example item three</li>
  </ul>
  <p>This will get styled.</p>
</div>
<p>This will not get styled.</p>

Example Code

ul ~ p {
  background-color: green;
}

Inline, Block, and Inline-Block Level Elements

    Inline Level Elements: Inline elements only take up as much width as they need and do not start on a new line. These elements flow within the content, allowing text and other inline elements to appear alongside them. Common inline elements are span, anchor, and img elements.
    Block Level Elements: Block-level elements start on a new line and take up the full width available to them by default, stretching across the width of their container. Some common block-level elements are div, paragraph, and section elements.
    Inline-Block Level Elements: You can set an element to inline-block by using the display property. These elements behave like inline elements but can have a width and height set like block-level elements.

Margin and Padding

    margin Property: This property is used to apply space outside the element, between the element's border and the surrounding elements.
    padding Property: This property is used to apply space inside the element, between the content and its border.
    margin Shorthand: You can specify 1–4 values to set the margin sides. One value applies to all four sides; two values set top and bottom, then right and left; three values set top, horizontal (right and left), then bottom; four values set top, right, bottom, left.
    padding Shorthand: You can specify 1–4 values to set the padding sides. One value applies to all four sides; two values set top and bottom, then right and left; three values set top, horizontal (right and left), then bottom; four values set top, right, bottom, left.

_____________________________________________________________________________________


Styling Lists

    line-height Property: This property is used to create space between lines of text. The accepted line-height values include the keyword normal, numbers, percentages and length units like the em unit.
    list-style-type Property: This property is used to specify the marker for a list item. Acceptable values can include a circle, disc, or decimal.
    list-style-position Property: This property is used to set the position for the list marker. The only two acceptable values are inside and outside.
    list-style-image Property: This property is used to use an image for the list item marker. A common use case is to use the url function with a value set to a valid image location.

Spacing list items using margin

    Apart from line-height, margins can also be used in CSS to enhance the spacing and readability of list items.
    Margins create space outside each li element, allowing control over the gap between list items.
    margin-bottom is used to create space below each list item. For example, margin-bottom: 10px; will create a 10-pixel gap below each list item.

Styling Links

    pseudo-class: This is a keyword added to a selector that allows you to select elements based on a particular state. Common states would include the :hover, :visited and :focus states.
    :link pseudo-class: This pseudo-class is used to style links that have not be visited by the user.
    :visited pseudo-class: This pseudo-class is used to style links where a user has already visited.
    :hover pseudo-class: This pseudo-class is used to style an elements where a user is actively hovering over them.
    :focus pseudo-class: This pseudo-class is used to style an element when it receives focus. Examples would include input or select elements where the clicks or tabs on the element to focus it.
    :active pseudo-class: This pseudo-class is used to style an element that was activated by the user. A common example would be when the user clicks on a button.

Working with Backgrounds and Borders

    background-size Property: This property is used to set the background size for an element. Some common values include cover for the background image to cover the entire element and contain for the background image to fit within the element.
    background-repeat Property: This property is used to determine how background images should be repeated along the horizontal and vertical axes. The default value for background-repeat is repeat meaning the image will repeat both horizontally and vertically. You can also specify that there should be no repeat by using the no-repeat property.
    background-position Property: This property is used to specify the position of the background image. It can be set to a specific length, percentage, or keyword values like top, bottom, left, right, and center.
    background-attachment Property: This property is used to specify whether the background image should scroll with the content or remain fixed in place. The main values are scroll (default), where the background image scrolls with the content, and fixed, where the background image stays in the same position on the screen.
    background-image Property: This property is used to set the background image of an element. You can set multiple background images at the same time and use either the url, radial-gradient or linear-gradient functions as values.
    background Property: This is the shorthand property for setting all background properties in one declaration. Here is an example of setting the background image and setting it to not repeat: background: no-repeat url("example-url-goes-here");
    Good Contrast for Background and Foreground Colors: It is important to ensure that the background and foreground colors have good contrast to make the text readable. The Web Content Accessibility Guidelines (WCAG) recommend a minimum contrast ratio of 4.5:1 for normal text and 3:1 for large text.

Borders

    border-top Property: This property is used to set the styles for the top border of an element. border-top: 3px solid blue; sets a 3-pixel-wide solid blue border on the top side of the element.
    border-right Property: This property is used to set the styles for the right border of an element. border-right: 2px solid red; sets a 2-pixel-wide solid red border on the right side of the element.
    border-bottom Property: This property is used to set the styles for the bottom border of an element. border-bottom: 1px dashed green; sets a 1-pixel-wide dashed green border on the bottom side of the element.
    border-left Property: This property is used to set the styles for the left border of an element. border-left: 4px dotted orange; sets a 4-pixel-wide dotted orange border on the left side of the element.
    border Property: This is the shorthand property for setting the width, style, and color of an element's border. border: 1px solid black; sets a 1-pixel-wide solid black border.
    border-radius Property: This property is used to create rounded corners for an element's border.
    border-style Property: This property is used to set the style of an element's border. Some accepted values include solid, dashed, dotted, and double.

Gradients

    linear-gradient() Function: This CSS function is used to create a transition between multiple colors along a straight line.
    radial-gradient() Function: This CSS function creates an image that radiates from a particular point, like a circle or an ellipse, and gradually transitions between multiple colors.

_____________________________________________________________________________________


Absolute Units

    px (Pixels): This absolute unit is a fixed-size unit of measurement in CSS. It is the most common absolute unit and provides precise control over dimensions. 1px is always equal to 1/96th of an inch.
    in (Inch): This absolute unit is equal to 96px.
    cm (Centimeters): This absolute unit is equal to 25.2/64 of an inch.
    mm (Millimeters): This absolute unit is equal to 1/10th of a centimeter.
    q (Quarter-Millimeters): This absolute unit is equal to 1/40th of a centimeter.
    pc (Picas): This absolute unit is equal to 1/6th of an inch.
    pt (Points): This absolute unit is equal to 1/72th of an inch.

Relative Units

    Percentages: These relative units allow you to define sizes, dimensions, and other properties as a proportion of their parent element. For example, if you set width: 50%; on an element, it will occupy half the width of its parent container.
    em Unit: These units are relative to the font size of the element. If you are using ems for the font-size property, the size of the text will be relative to the font size of the parent element.
    rem Unit: These units are relative to the font size of the root element, which is the html element.
    vh Unit: vh stands for "viewport height" and 1vh is equal to 1% of the viewport's height.
    vw Unit: vw stands for "viewport width" and 1vw is equal to 1% of the viewport's width.

calc Function

    calc() Function: With the calc() function, you can perform calculations directly within your stylesheets to determine property values dynamically. This means that you can create flexible and responsive user interfaces by calculating dimensions based on the viewport size or other elements.

