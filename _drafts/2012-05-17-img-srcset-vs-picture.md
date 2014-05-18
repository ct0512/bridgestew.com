---
title: '&lt;img srcset=&#8221;"&gt; vs. &lt;picture&gt;'
author: Bridget
layout: article
permalink: /2012/05/17/img-srcset-vs-picture/
categories:
  - Web Stuff
---
My pal, [Brad Dielman][1], alerted me that a bruhaha regarding responsive images existed. He had to focus my attention on it because I missed all the Twitter traffic highlighting the web community&#8217;s ire was raised over something other than vendor prefixes. As a result, I&#8217;ve read a lot about the proposals for addressing content images (stuff inside the `<img />` tag in HTML) in an increasingly &#8220;Responsive Web Design&#8221; colored world.<!--more-->

First, I read [other][2] [people&#8217;s][3] [synopses][4] of what took place. It seemed like a good place to distill what all the varying parties had to say, and I was right. These articles contained relevant links pointing to [other][5] [commentary][6] or [background][7] [information][8] and I found myself reading those, too.

In the end, I couldn&#8217;t resist heading over to the [WHATWG mailing list archive][9] for even more context.

The item in particular that provided, at least for me, the most bang for my buck on the decision made by Ian Hickson (a.k.a &#8220;Hixie&#8221;) was [this one][10]. It&#8217;s a long read, but incredibly worthwhile. In this, Mr. Hickson addresses what he believes the issue to be and many of the points made by various interested parties. I continued through the entire thread and read other entries on the WHATWG mailing list, but admittedly not everything that is there for the month of May. I plan to get through as much of it as possible, though!

A few key things became clear to me:

1.  **Hixie is genuinely aware of responsive design as a means for moving the web forward** as the volume of web capable devices (and their varied screen sizes) increases. At first it seems he believed that CSS was sufficient to address the issue, then changed his position with regard to the `<img />` element, as it is a different animal than images declared in CSS.
2.  **Tackling the issue of bandwidth and latency (one of the issues brought up by web developers) is not simple**. I don&#8217;t think anyone believed it was simple, but what Hixie wrote about the issue sold me on the notion that latency and bandwidth issues are better addressed by the browser, magically handled by some man behind the curtain, rather than (micro?-)managed via design and front end development.
3.  **Ian Hickson has content authors (web designers and developers) interests at heart in his decision making process**. I suspect this last point is not going to be very popular, but that&#8217;s what I took away from his response about the decision he made.

With that said, I don&#8217;t know how I feel about the `srcset` attribute just yet. I have mixed feelings, both for and against. I am willing to see how it plays out as the spec gets a bit further along.

What I like about the `srcset` idea is that it provides alternate images for specific conditions in a relatively concise manner. Essentially, that&#8217;s what we need &#8211; different images to be served in different cases that we outline. And, the less typing (in my case, TYPO-ing) the better.

What I don&#8217;t like about the `srcset` idea is that it is declared in an attribute. The definition of an attribute (in general English) is: *an inherent characteristic* — and that is pretty much how I have thought of attributes in HTML &#8212; as characteristics of the item to which they are attached. In this case, it would be a characteristic of the `<img />` element. Only, the syntax for `srcset` isn&#8217;t quite that clean. While it lists alternate sources for an image to be displayed for this particular element, there is additional syntax that isn&#8217;t &#8220;inherent&#8221; to the image at all, *but rather is related to the viewport*. I think that bit is confusing.

That&#8217;s not even my largest concern. Separation of content from presentation is something we strive for as professional web developers and designers. This issue blurs that line. *A lot*. On the one hand, we have a piece of content, an image, we want to provide to all devices accessing it in a way that looks best in the context it is being viewed. On the other hand, that same content requires special consideration based on presentational demands and/or limitations because we are allowing all devices to access it.

Text reflows. That&#8217;s an easy issue to address. If we are conscientious about presentation we alter reading lengths, font sizes, leading, etc to provide an optimized experience. This is all handled outside the HTML and done in the CSS. Separation of concerns regarding text presentation is not that difficult in the grand scheme of things.

Images and media are in another bucket: The-This-Is-Hard-To-Separate-Concerns-Bucket. At the root, what we are asking for is the ability to send to the client some form of media based on *presentation*. This is why I understand Hixie&#8217;s initial thoughts that this was a CSS problem, not an HTML problem. This is also why the `<picture></picture>` element has strong leanings toward using CSS Media Queries with each image option (while using the `<video></video>` element syntax pattern) to try to address the issue. This is a *presentational* problem. We all seem to get that, and yet we are all trapped (for now) trying to solve this presentational issue in the HTML, the content area.

I don&#8217;t know how to address the problem. I feel very confident, though, that really smart people are working hard to resolve it. Those people are both web devs (considered authors according to standards bodies) and browser makers (considered implementors according to standards bodies). Jeffrey Zeldman brought up a point on [zeldman.com][6] that actually prompted me to write this post:

> One way the tension between principle and reality plays out is in not uncommon incidents like the one we’re reacting to now. According to the priority of constituencies, designer/developer feedback should be welcomed, if not outright solicited. In principle, if there is conflict between what designer/developers advise and what browser makers advise, priority should be given to the advice of designer/developers. After all, their needs matter more according to the priority of constituencies — and designer/developers are closer to the end-user (whose needs matter most) than are browser makers.

I get where Jeffrey is coming from. I really do. Even still, I don&#8217;t think it&#8217;s as cut and dried as, &#8220;If there is a conflict on how to solve a problem, lean toward what the developers want over the browsers.&#8221; Mainly because most web developers don&#8217;t have a clue how a browser works. Even brilliant web devs like Mat &#8220;Wilto&#8221; Marquis (@wilto), Ethan Marcotte (@beep), and Jason Grigsby (@grigs) – guys for whom I have the utmost respect and consider to be in the top percentile of our industry – have not claimed to understand all the dark arts at play that allow us to have [gif wars][11] and [puppies every day][12].

I hope I&#8217;m not misreading Jeffrey&#8217;s point. I very well could be. I am not advocating that the priority of constituencies be reversed. Not by a longshot. But I hope this scenario plays out differently than the complaints registered of the past. I hope that the brilliant theurgists who give me the internet in my pocket can hear the pleas of my fellow web devs about our needs to provide the best possible experience to end users (which is the same goal the browsers have!) and work **together** to arrive at a mutually agreeable solution.

 [1]: http://braddielman.com/
 [2]: http://timkadlec.com/2012/05/wtfwg/
 [3]: http://adactio.com/journal/5474/
 [4]: http://www.alistapart.com/articles/responsive-images-and-web-standards-at-the-turning-point/
 [5]: http://mattwilcox.net/archive/entry/id/1090/
 [6]: http://www.zeldman.com/2012/05/17/editor-vs-constituencies/
 [7]: http://www.w3.org/community/respimg/
 [8]: http://junkyard.damowmow.com/507
 [9]: http://lists.whatwg.org/pipermail/whatwg-whatwg.org/2012-May/subject.html
 [10]: http://lists.whatwg.org/pipermail/whatwg-whatwg.org/2012-May/035855.html
 [11]: http://sfy.co/xq3
 [12]: http://www.dailypuppy.com/

 *[HTML]: Hypertext Markup Language
 *[WHATWG]: Web Hypertext Application Technology Working Group
 *[a.k.a]: also known as
 *[CSS]: Cascading Style Sheets