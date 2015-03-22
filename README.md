# scroll-ease
Angular scroll(to) directive with options for easing and duration

##Usage
First, bring the script into your index page:

`<script scr="ScrollEaseDirective.js"></script>`

You can use this as an element or an attribute.  As an attribute it can be used on any type of element, whether it's an element in the tabindex or not.

html:

`<button data-scroll-ease="section1" data-easing="easeOutCubic" data-duration="1000">Learn More</button>`

or

`<scroll-ease="section1" easing="easeOutCubic" duration="1000">Learn More</scroll-ease>`

The settings for this directive are as follows:

###Element to scroll TO
The element you're scrolling to is set by `<data-scroll-ease="section1"` where section1 is the id of an element in the DOM.

###Easing
Set easing with `data-easing="easing option"`

There are a bunch of easing options that are available:

- easeInOutQuad
- easeInCubic
- easeOutCubic
- easeInOutCubic
- easeInQuart
- easeOutQuart
- easeInOutQuart
- easeInQuint
- easeOutQuint
- easeInOutQuint
- easeInSine
- easeOutSine
- easeInOutSine
- easeInExpo
- easeOutExpo
- easeInOutExpo
- easeInCirc
- easeOutCirc
- easeInOutCirc
- easeInElastic
- easeOutElastic
- easeInOutElastic
- easeInBack
- easeOutBack
- easeInOutBack
- easeInBounce
- easeOutBounce
- easeInOutBounce

If an easing option isn't defined easeOutCubic will be used by default.

###Duration
Duration is set with `data-duration="time in milliseconds"`

If the duration is not defined the default is 1000 (1 second)


*If you're building accessible or validated html sites use this directive (and all others) as an attribute, not as an element.  I use data- to precede all directive tags and settings to pass html validation
