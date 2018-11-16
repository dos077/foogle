From The Odin Project's [curriculum](http://www.theodinproject.com/courses/web-development-101/lessons/html-css)
HTML assignment number one, recreating the homepage of Google.com

For both part of the assignment, I've stuck to the instruction and the basics, other than adding the hover effects. The html and css should be self explanatory.

There are few tricks I drew from past experiences and some subtle effects I didn’t copy exactly. I will try to make notes below.

Easy Part - frontpage of Google

Html are different and simplified. It’s not Google’s html is bloated, but they obviously have devised a more structured layouts for insertion of random daily modules.

The top nav and footer are absolute positioned. Didn’t spend the time to comb Google’s css. Just experience from many years back.

All hovering effects are presented, they are just slight variations on the class using .class:hover tags, except the I’m Feeling Lucky spinning effect. I know how to do it in Javascript, but pure css maybe janky and definitely too time consuming.

.class:focus effect did not render on the parent div of the text input box. Google also have a drop down on focus on the text box, it could be javascript, no further debugging was attempted.

Mouse pointer on the mic button is normal. Google’s html on the button is a jumbo mess. Looks like another javascript button. Just left it as plain img on my html.

Hard Part - search results of Google

Pardon the irregular size search icon. Downloaded the wrong image and didn’t want to spend time fixing it.

The page has a min-width of 1000px define by the top div. I am not sure if Google sets such thing or just have structured their divs as such. Since I am not programing the empty modules in the white space and the user shortcuts module is absolute positioned (probably should be float:right, but alignments of in-line items are PitA), I prefer to use a min-width to ensure correct rendering.

Hovering effects should be completed. 
The results page have a lot of content sensitive modules, I just put in the top results without image, otherwise it could be a black hole. div.top and div.content .top class was a mess, should’ve put the div.top into its own container or different name, such as div.header .top. Ended up doing some resets in div.content .top.

Google uses fragments of their logo for the page navigation. I ended up having some fun and render their logo in text instead. The layout might get trick up in some browsers or OS with different text rendering, but it’s just cooler and cleaning in code for me. The <a>s are rendered outside of the <span> elements using absolute position, so I only need to line up the <span>s correctly.
