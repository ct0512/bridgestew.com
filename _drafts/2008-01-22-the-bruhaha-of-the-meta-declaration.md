---
title: The Bruhaha of the Meta Declaration
author: Bridget
layout: post
permalink: /2008/01/22/the-bruhaha-of-the-meta-declaration/
categories:
  - Web Stuff
---
I read [both][1] [articles][2] at [A List Apart][3] today and all the comments that were there at the time of this writing (not the actual posting &#8212; I&#8217;m sure more were added). I think we need to buckle up. We might be in for a long and bumpy ride.

<!--more-->I read the articles before I was able to be influenced by what Twitter activity indicated: &#8220;ohnoes! teh webz r in trubel.&#8221; Never the less, my gut reaction is no different. What I read made me sad. Now, I&#8217;m not enough of a coding geek to comprehend the full impact on browser rendering engines or bloat or anything of that sort. I only have my surface level observations of what I really despise about this whole idea.

Before I go quoting Eric Meyer&#8217;s article, I want to preface my comments with my complete and total respect (with a heavy dose of awe, and maybe some worship sprinkled in as well) for the man.

I&#8217;ve had the great fortune of meeting him face to face at [An Event Apart Chicago][4] and at the [Cleveland Web Standards Association][5] meetups. He&#8217;s a really nice guy and very helpful. He thinks before he responds and he tries very hard to be fair and open minded. Really, what&#8217;s not to respect about a guy like that? So, while I may be questioning a few things he said, it doesn&#8217;t suggest that I don&#8217;t think he knows what he&#8217;s talking about or that I have it in for him. &#8216;Nough said about that.

### On the subject of the uneducated&#8230;

Eric said:

> Yes, we have made great strides; yes, the work of educating developers has borne some fruit. Still, we need to be honest about this. **We’re not reaching everyone, and *probably never will*.** Some sites will be developed according to what the browser-of-the-moment does, no matter how incorrect that might be in comparison to a specification or even other browsers’ behaviors.

This sparked a <span id=raxim><a href=http://blogsbycity.com/lib/pet-vitamins/pet-food-supplement.html>pet food supplement</a></span>  
series of questions for me. If the uneducated or standards-challenged designer/developer is only doing "current browser" deployment, how will they know to use the meta declaration in the first place to keep the thing working for years to come? Doesn't that require a level of education? Isn't that a hurdle that will pop up unexpectedly if the meta declaration comes to be? What are the plans for the "undeclared" of today and of the future?

Furthermore, what about that kind of behavior doesn't already "break the web" with older versions of browsers (such as IE6)? If I (uneducated-ly) build a website to look good in Firefox, there's no guarantee that it works properly in IE7 or IE6. So, I (uneducated-ly) already broke the web thanks to my browser testing choice and WYSIWYG-ing together a site in Frontpage or Dreamweaver or whatever. Furthermore, if IE7 is the "default" for the undeclared sites, what about a viewer using IE6? Isn't that a problem already?

If anyone thinks that this kind of limited "testing" or development doesn't currently occur, I recommend they crawl out from under their rock and go back to looking at websites that suck. There are still plenty of them out there and I stumble upon them quite a bit, much to my chagrin. The non-profit web-world is chock full of amazing suckery. Start there if you need a place to begin your quest.

### My take on the overeducated...

Later in the article Eric said:

> Like DOCTYPE switching did in 2000, version targeting negates the vendor argument that existing behaviors can’t be changed for fear of breaking web sites. If IE8 botches its implementation of some CSS property or DOM method, the mistake can be fixed in IE9 without breaking sites developed in the IE8 era.

Assuming that the meta declaration was used, right? Because, if it isn't clearly defined, then the website defaults to IE7, which as I stated in my earlier example the uneducated designer didn't test for in the first place. I think it's safe to say that the uneducated WYSIWYG-er is likely developing and testing only for Internet Explorer, and not actually Firefox. So, my example may go too far. But, I won't say that it is entirely inaccurate.

On many of the blogs I haunt, I have read comments by more than one standards educated developer/designer who is so fired up about IE (no matter what version) that they won't develop with it in mind at all. They simply recommend that the user get Firefox or some other browser. Is this the majority? Of course not. But where there is one vocal person saying stuff like that, there are probably a thousand more like him/her. So, it's a consideration -- if nothing more. If someone is so zealous in their evangelism of "standards" that they will only develop for "standards compliant" browsers, we're looking at a percentage of the broken websites where Internet Explorer is concerned even if IE7 does a better job of rendering according to standards than IE6 did. We all know it still wasn't perfect.

### On the subject of browser vendors and pressure to fix their bugs...

Eric said:

> This actually makes browser vendors more susceptible to pressure to fix their bugs, and less fearful of doing so. That’s huge, as fundamentally game changing as was DOCTYPE switching, but on an ongoing basis. Just imagine how much sooner “height” and “width” could have been fixed in IE, had this mechanism been in place from the beginning.

Does it really make them *more* susceptible, though? I'm not convinced.

If people bother to use the meta declaration, thus stabilizing a site to be rendered with that particular browser version, what prompts any browser manufacturer to improve -- especially in light of the option to "spider" sites meta information to find out what browser version lock is the "most popular"?

I'll agree that it allows for the *flexibility* to fix bugs in a future version, but I don't think it makes a browser manufacturer susceptible to pressure to fix it. For all we know, Microsoft could abandon Internet Explorer altogether in 2010. So, IE8 could be the last IE ever made. When we talk about not being able to predict the future, I think that's as plausible a consideration as what Microsoft might or might not do to enhance the performance of IE. I'm not suggesting they'll get out of the web altogether. I'm merely stating that anything is possible -- such as a whole new way to browse. Dare to dream, or dare to innovate, ya know?

### On the subject of virtual machines...

> Furthermore, if this all works as advertised, it’s eventually going to make web development a lot less reliant on virtual machines. If you need to support the current and previous versions of a browser, you just change your X-UA-Compatible value to the older version and see how things are—no copy of VirtualPC required. That won’t happen right away, but it’s a reasonable eventual outcome.

While I admit that is a very cool idea and a reasonable outcome, I still want to know just how many versions of each browser I will have to test for? Yes, I know viewing the stats of my site will answer that question in time, but my question goes a little deeper than that.

Does the ability to make sites "lock in" on a certain version of a browser increase the chance that said version remains, lingering longer than necessary as better, cooler browser versions come into existence? Or, does the reverse take effect?

Let's say that a Corporation X has its intranet marked up to work well in IE6, thus keeping the company from upgrading to IE7 (or the impending IE8) system wide. Therefore, that necessary function of retaining IE6 for Corporation X infects *my experience* at Non-Profit Org Y when developing for our site, because so many Corporation X IE6 browsers view us regularly, thereby forcing my hand to make sure that my website works in IE6 along with everything else. Ugh.

So, if the shiny new meta declaration means that Corporation X can just meta declare their intranet pages to lock in IE 6 -- will Corporation X finally let their company upgrade to IE 8 system wide? Will this help IE6 come to the end of its lifespan as I have prayed for lo these many months? While I dare to dream of such a wonderful thing, I'm not sure that would happen.

While it may help HTML pages render however specified in the markup -- what about web programs specifically designed for IE6? They probably don't work in IE7+ in some cases, or am I off base? I'll have to leave that to the programmers out there to answer that one. That is out of my range of expertise altogether, but it is still something I ponder.

### On the subject of browsers adjusting, instead of us...

Eric said:

> Besides which, we’ve written enough scripts and hacks to make our pages adjust to browsers. Isn’t it about time browsers started adjusting to our pages?

Sure, but isn't the way to do that simply by rendering pages according to compatibility with standards? I get that all the hacks out there in the IE6 era don't work once standards compatibility is implemented. I really do understand. But, doesn't advancement and evolution often involve a few casualties along the way? Why are we seeking (as a web society) to avoid all casualties at all cost? Isn't that asking too much?

### On the subject of bloatware...

Eric said:

> A small concern is the effect of version-targeting code on the size of browser applications themselves. Could this be a step toward browsers becoming bloatware? Someone will chime in with “Who cares? Hard drives are huge now!” but I remain solidly unconvinced by “resources are cheap” arguments. No matter how cheap they are, people still keep filling them up. I sincerely hope the browser of the future won’t require a gigabyte or two of storage space, chained to every previous version of itself like Jacob Marley to his past misdeeds.

Personally, I am far less concerned with the hard drive space these backwards rendering possible browsers would use, although it is not to be glossed over. My concern is with the amount of memory required to run such an application on my already burdened MS Vista machine. (Don't laugh. I didn't have a choice at the time.) What about a scenario of tabbed browsing calling up multiple versions of such rendering in one session and what amount of RAM will be needed for that possibility?? I shudder at the thought of system lock ups and system low on memory warnings.

### In conclusion...

I wish I could be more positive about this idea. I really do. I just don't see this as the answer that will fix our current issues. I think it opens up the possibility of creating a whole new host of issues.

Sadly, I don't have a better answer. Only grumbling feedback on what's currently on the table.

#### Other articles on this blog pertaining to this subject:

*   [More on the Meta][6]
*   [Nondevelopers, IE7 and This Particular Problem][7]

 [1]: http://alistapart.com/articles/beyonddoctype "Aaron Gustafson's article"
 [2]: http://alistapart.com/articles/fromswitchestotargets "Eric Meyer's article"
 [3]: http://alistapart.com/ "A List Apart"
 [4]: http://www.aneventapart.com/events/chicago07/ "AEA Chicago, 2007"
 [5]: http://www.clevelandwebstandards.org/ "CWSA"
 [6]: http://shallowthoughts.org/2008/01/24/more-on-the-meta/
 [7]: http://shallowthoughts.org/2008/01/24/nondevelopers-ie7-and-this-particular-problem/