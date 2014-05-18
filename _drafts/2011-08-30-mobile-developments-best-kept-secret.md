---
title: 'Mobile Development&#8217;s Best Kept Secret?'
author: Bridget
layout: post
permalink: /2011/08/30/mobile-developments-best-kept-secret/
categories:
  - Web Stuff
---
For a little over a year now, I&#8217;ve worked in the portion of web development that focuses on mobile devices. That doesn&#8217;t mean I get to completely ignore larger display devices all the time, but being in a mobile centric workflow has broadened my planning scope to adapt to unforseen, unpredicted, and unknown display ranges. Very few, if any of us, know what is being invented in some random nerd&#8217;s mom&#8217;s basement that will change web access as we know it. Such being the case, I&#8217;m a strong believer in the [Adaptive Web Design][1], [Responsive Web Design][2], and [Mobile First][3] philosophies.

I prefer to build things with fluid layouts and flexible grids. I make extensive use of media queries. I find debugging User Interfaces (UIs) in these environments can be challenging.

Using Web Inspector or Firebug on a desktop/laptop doesn&#8217;t trigger layout variations based on device orientation and/or device-width in a consistent manner, essentially keeping those styles hidden from me if that is the trigger I want for a media query. It may have been some buggy behavior in those cases or just really poor formatting for the cascade on my part, but it wasn&#8217;t predictable and that was my beef with it. Debugging in the simulator is no more fun than what I described above.

## So, what are our options?

Right now, I only know of 2. I would really like to hear what other people are using, with a modicum of success in the comments for this post.

### Firebug Lite Bookmarklet

It&#8217;s possible to use the [Firebug Lite][4] Bookmarklet if you are debugging a web page that displays the address and bookmarks bar at the top of the browser. If, however, you are dealing with an HTML app that &#8220;installs&#8221; to the device&#8217;s home screen, that option isn&#8217;t available.

Regardless, my experience with the Firebug Lite Bookmarklet on the iPad was frustrating. Trying to target the tiny little plus signs to drill down into the elements of the DOM tree in order to access what was nested inside was painful. My sausage fingers couldn&#8217;t accomplish that task with any grace. Zooming in allowed me to tap the correct thing, but the display would usually be out of whack until somehting triggered it to refresh.

Using the tiny panel that opens at the bottom of the screen was painful, especially having to use 2-finger scrolling to get at stuff that was further down the Firebug screen. It&#8217;s response is slow and laggy on an iPad first generation. I can&#8217;t speak for the iPad 2 (yet). It is possible to open the Firebug panel in a new window, but then you have to flip back and forth between the web page you are targetting and Firebug panel. Argh!

I gave up on that as a plausible means for debugging on any grand scale. Minor quick tweaking tests might be something I would use it for. But even that felt like it took too long for something so minor.

### Weinre

What, you&#8217;ve never heard of [Weinre][5]? It stands for **We**b **In**spector **Re**mote. It is pronounced &#8220;winery&#8221; if you fancy yourself too highbrow for the other pronunciation. Otherwise, the 12-year-old-boy in all of us may just call it &#8220;weiner&#8221;.

It seems that Weinre made its first appearance on github in December of 2010. It&#8217;s developed by Patrick Mueller (<a href=http://twitter.com/#!/pmuellr>@pmuellr</a>) of IBM.

Anyway, I had never heard of this tool either. I don&#8217;t know how I missed it! My coworker, Kurt, was about to embark on a lengthy process trying to build some way for us to debug UIs in the device. I protested, &#8220;Surely someone super smart has already solved this by now.&#8221; So, I Googled. It wasn&#8217;t at the top of the search results. I don&#8217;t even think it was on the first page of results &#8211; which must mean I was really commited to finding something so that we wouldn&#8217;t have to build it. Once I stumbled upon Weinre, it seemed really promising! So, I shared it with Kurt who had a little trouble getting it to work for him. We got busy with other work stuff, and this sat on the shelf for a few weeks.

I didn&#8217;t think all that much of it during those weeks. I just planned to figure out how to make it work once we had a break in the onslaught of daily tasks. The day finally came and I committed to figuring out this tool that seemed like it would solve a lot of my debugging woes.

It was much easier to implement than the documentation led me to believe. I think it is written in some kind of Sysadmin-ese. All I needed to do was download the Mac app, create a <samp>~/.weinre/server.properties</samp> file with two options inside it:

1.  boundHost: -all-
2.  httpPort: (mine was 8080)

The only other thing I had to do to complete the setup was add this line to the file I would be debugging (Line wraps marked »):

`<script src="http://[my Mac's IP address]:8080 »<br />
/target/target-script-min.js#anonymous"></script>`

In my case, I&#8217;m trying to debug an entire app. We have different views and partials/includes going, so I was able to put that line in just the main.erb file (a Ruby thing) and it would be included in all the screens across the app.

Once those preliminary steps were done, I was able to point my iPhone to my local development version of our application, while debugging it using a familiar Web Inspector-esque interface on my Macbook Air!

One cool thing is when I hover over the element in the Weinre Elements tab on my laptop, I can see it in the display on the iPhone just as I am used to from using Web Inspector or Firebug in the past. I could make changes to the CSS in the inspector on my laptop and they would appear as changes on the iPhone. It even has a working Javascript console!

I certainly haven&#8217;t tested this particular tool extensively, but the preliminary results are very good! I&#8217;ll be diving into [Patrick Mueller&#8217;s blogspot][6] a bit more to find out what is available in this little gem. It is possible that I have found a tool that I can use on a grande scale for debugging the layouts and styles &#8211; and maybe even the interactions &#8211; of mobile apps and still manage to keep my sanity in check. The sanity part is clearly, debatable.

If you would like to watch the progress of the best kept secret for debugging mobile apps, check out [Weinre on github][7].

Thank you, Mr. Mueller, for your efforts on debugging mobile!

 [1]: http://easy-readers.net/
 [2]: http://www.abookapart.com/products/responsive-web-design
 [3]: http://oreilly.com/catalog/0636920020783/
 [4]: http://getfirebug.com/firebuglite
 [5]: http://phonegap.github.com/weinre/
 [6]: http://pmuellr.blogspot.com/
 [7]: https://github.com/phonegap/weinre