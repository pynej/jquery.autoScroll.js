jquery.autoScroll.js
====================

jQuery Plugin to Scroll any Element with the Page using paddings or margins.

This script will make any element work similar of a position:fixed element in that it will cause the element to
scroll with the browser window vertically as the user scrolls up and down the page.

The benefit of this over the css attribute is that this method will retain the items original placement and flow 
instead simply adjust the margin-top or padding-top to replicate the scrolling logic.  Additional paddingTop 
and paddingBottom can be specified witch will act as minimum margins between the viewport and the floating item.
This means that it will work in nested scrolling sections for example and can be configured in more deatil then
simple fixed positioning.

Sample Code:

<pre>$("#element").autoScroll({ paddingTop: 30 });</pre>

Make it snap instead of scroll.
<pre>$("#element").autoScroll({ paddingTop: 30, animate: flase });</pre>

Adjust via padding instead of margins. (Usefull if the parent item has a fixed height.)
<pre>$("#element").autoScroll({ paddingTop: 30, scrollMode: "padding" });</pre>
