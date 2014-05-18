---
title: 'Review: Adaptive Web Design by Aaron Gustafson'
author: Bridget
layout: article
permalink: /2011/08/27/review-adaptive-web-design-by-aaron-gustafson/
categories:
  - Web Stuff
---
In recent years, it seems that I have less and less time to do the things I would like to do as more and more of my time is taken up by the things that I must do. That&#8217;s why I often feel I don&#8217;t have the time to read everything about web technologies that one must read these days in order to keep up their skills. It seems that the trend in publishing, at least where web design is concerned, is to put the information &#8220;out there&#8221; in concise bits making the idea of reading a book less daunting than some of the voluminous tomes I have read in past years. At 135 pages (including the index), Adaptive Web Design is a quick read, packed with solid information.

In keeping with that theme, I&#8217;ll keep my review of the book brief, while still attempting to explain why I liked it so much.<!--more-->

I&#8217;m familiar with the idea of building sites using the principle of &#8220;Progressive Enhancement.&#8221; I&#8217;ve previously shared my [encapsulated explanation][1] of what it is. This book took that understanding up a notch. A pretty big notch, at that.

I&#8217;ve often thought of progressively enhancing sites/apps as the following:

1.  Write the cleanest HTML I can in order to get the job done.
2.  Layer on CSS, with whatever CSS3 additions are appropriate for the site&#8217;s designs and the level of acceptable fallbacks for older browsers agreed upon up front with my client.
3.  Top it off with the appropriate amount of Javascript goodness to achieve slick behaviors whilst chasing that ever elusive &#8220;seamlessness&#8221; that clients like to request.

Seems pretty simple, right? Three &#8220;layers&#8221; for progressive enhancement: HTML, CSS, Javascript. Au contraire! Aaron&#8217;s book exposed me to the layers of progressive enhancement that dwell within the Holy Trinity that is today&#8217;s web stack. That&#8217;s where this adaptive web design concept got exciting. Admittedly, I already make use of some of the points discussed by Aaron, but I had never really considered those things to be means by which enhancement progresses. Things like&hellip;

*   Meaningful element choices
*   Class names
*   ID names
*   Microformats

&hellip; as HTML enhancements. I won&#8217;t go into detail how those things progressively enhance markup. That&#8217;s what reading the book is for. Still, it was really cool to consider all of those pieces that I used daily as progressive enhancement, in and of themselves. I was already onboard the semantics train: sometimes spending more time than I care to divulge determining which is the right element or choosing the appropriate class name on a generic element. I understood that stuff was important, but now I don&#8217;t feel quite as guilty developing a plan for those pieces of the puzzle because I never felt guilty developing a plan for the CSS or Javascript enhancements I would use.

Additionally, Aaron details items like the following as CSS enhancements (along with other things).

*   Capitalizing on browsers ignoring syntax they don&#8217;t understand
    *   Selector-based screening techniques to target specific browsers
    *   Using Conditional Comments for IE
*   Using the cascade to separate concerns
    *   Typography
    *   Layout
    *   Color
    *   Effects
*   Using @media declarations and queries

Where CSS, Javascript and ARIA are concerned, Aaron expressed quite a few things I haven&#8217;t incorporated into my &#8220;UI Realization&#8221; flow yet. Yay for learning new things!

Not only does Aaron explain practical things for us to apply, he explains the concept of &#8220;fault tolerance&#8221; &#8211; something I had never really considered before, but think about *now* before I sit down to craft a site or a web app. Fault tolerance is an important concept that aids in understanding how HTML and CSS work to make the life of web authors a bit easier.

I promised to keep this review brief, so I think I&#8217;ll stop here. I hope I&#8217;ve shared enough about the book to make you think about reading it. It won&#8217;t take you long, that&#8217;s for certain. But you will walk away from it a stronger designer/developer. It&#8217;s worth it to find time to read *Adaptive Web Design*.

 [1]: http://shallowthoughts.org/2011/07/23/misunderstanding-progressive-enhancement/

 *[HTML]: HyperText Markup Language
 *[CSS]: Cascading Style Sheets
 *[IE]: Internet Explorer
 *[ARIA]: Accessible Rich Internet Applications
 *[UI]: User Interface