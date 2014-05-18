---
title: Nondevelopers, IE7 and This Particular Problem
author: Bridget
layout: post
permalink: /2008/01/24/nondevelopers-ie7-and-this-particular-problem/
categories:
  - Web Stuff
---
My latest round of articles here have been spawned as retorts, replies and general questions to the comments of others in the web community. I quote these folks so that they get the proper credit for what they said, but I fear that my latest posts could be construed in a manner in which I do not intend &#8212; as antagonizing. So, please allow me to state that I am not attempting to call out these brilliant minds to defend their declarations, per se. I&#8217;m seeking answers to the questions I have as a result of the things they have said regarding [browser version targeting][1].

<!--more--> Jeffrey Zeldman provided a 

[poignant comment on his blog][2] regarding why he is in favor of the version targeting idea, having moved past his original misgivings.

### Web developers who aren&#8217;t developers&#8230;

Jeffrey stated:

> When I think of the IE7 default Microsoft intends to use in version targeting, I think of the people who don’t read this site, don’t read ALA, don’t attend conferences — not because they are bad, lazy developers, but because they are not web developers at all.
> 
> There are millions of them out there.

I understand this concept very well. I still think this solution has not been thought through all the way to a proper conclusion.

### Utopian implementation&#8230;

Jeffrey stated:

> If CSS and <span id=haug><a href=http://blogsbycity.com/lib/pet-vitamins/dog-muscle-supplement.html>dog muscle supplement</a></span>  
> HTML had been introduced to the world in tandem; if browsers had supported them accurately from day one, with no browser wars and no need for The Web Standards Project; if CSS-based layout were so easy that nobody needed to read Meyer or Cederholm to figure out how to do it; then there’d be no need for expensive authoring tools, no need for the DOCTYPE switch, no need for hacks, and no need — today — to protect schoolteachers, rabbis, shop owners, and other nonprofessional creators of websites from the complexities of web development and browser rendering issues.

Ok, and we all know that is not how the web developed. But what other product/service/industry can claim that all their tools, best practices and standards were handed to them on a silver platter when it originated? Still, they have managed to persevere.

### This particular problem...

Jeffrey stated:

> Version targeting is not a noble attempt to educate all the people who build websites the wrong way; it is an attempt, perhaps noble in its own way, to protect incompetent web developers from things they don’t understand, and to protect non-specialists from the maddening aggravation that comes with browser updates.

Ok, I hear ya, but I still don't see version targeting and IE7 as the default where no target is specified as being the proper solution to *this particular problem*. It presupposes that IE7 is adopted by all Internet Explorer users, doesn't it?

Jeffery said:

> If the idea came from Firefox instead of Microsoft, and if it had been publicly discussed before it was announced, the reaction, I believe, would have been more positive.

Why would Firefox offer this particular solution when they didn't create this particular problem? I think that it is Microsoft's problem and as a result it is their responsibility to fix it. I applaud them for trying, but not for the proposal itself. I'm not going into a "Microsoft sucks" rant because, it isn't helpful or productive. So, here is where my thought process leads on why the proposal described on [A List Apart][3] and on the [IE Blog][4] falls short:

### IE7 as the default rendering engine doesn't make sense...

From my very shallow observations of the subject at hand, this solution is not going to fulfill the needs of the above described class of folks (web developers who aren't developers) building websites.

First and foremost, I am still waiting for someone to explain to me why it was IE7 that was chosen as the default rendering engine *over IE6*. Wasn't it IE7 that "broke the web" in the first place? So, if the primary "breaker of the web" is being used as the default solution -- how is anything actually being fixed? Please, I beg of you, O Mighty Intarwebz, tell me what I'm missing on this particular aspect of the solution. There has to be a piece to this puzzle that I don't grasp and if someone would bother to explain *that*, then I might be in favor of this idea.

I understand that cutting edge developers, standardistas and brilliant guys like [Jeremy Keith][5] want IE8 or IE[new] to be the default. I understand why they want it and my gut wants it, too. I also understand the argument of why it is beneficial to select an older engine as the default for instances of sites where no target meta has been included. I don't disagree with the logic in any of these arguments -- either side. However, I do argue with the logic that states that IE7 is the proper choice in this particular problem. How does it help fix the number of sites that are being *developed today with IE6 as the browser testing environment*? (Think non-profit, faith based, local schools, et al.)

Please understand that **I work for a non-profit**. Go look at the [table based site][6] I manage because there is no money in the budget to redo the site sans tables. The table based structure exists because of a CMS that I can't alter. I am personally and painfully aware that cutting edge is not the norm everywhere you turn. I really am thinking of those people Jeffrey listed in all my rambling thoughts on this subject. This proposed solution does not add up, from what I can see.

IE6 and all the sites built to "work" in it, intentionally via hacks, or unintentionally due to ignorance, is still the issue we are dealing with here and I don't see that going away any time soon.

Let's say that you build your smokin' hot IE8 shiny awesomeness using all the cutting edge tech available at the time. Let's say that you even set the meta to target IE8 in order to get all the benefits of said awesomeness. That site will still be including hacks and comments and work-arounds for the **visitors of your site that use IE6 as their browser**. Sure, IE7 is getting some traction (finally!) but there is still a whole helluva lot of IE6 and a smattering of IE5.5 out there - so says the website's stats of the non-profit where I work. Is there a proposal in the works that guarantees that those old browsers will finally go away so that we, the knowledgeable, can build sites without hacks for IE6, target the latest browser version tested and move on?

It appears to me that IE7 being the default renderer for sites that do not use a meta declaration only works IF IE7 is the oldest browser alive in the Microsoft stable of browsers. Is there a proposal in the works that addresses this issue?

#### Other articles on this blog pertaining to this subject:

*   [The Bruhaha of the Meta Declaration][7]
*   [More on the Meta][8]

 [1]: http://www.alistapart.com/articles/beyonddoctype "Aaron Gustafson's article on A List Apart."
 [2]: http://www.zeldman.com/2008/01/22/in-defense-of-version-targeting/#comment-29366 "The Second Grade Teacher Defense"
 [3]: http://www.alistapart.com/ "A List Apart"
 [4]: http://blogs.msdn.com/ie/archive/2008/01/21/compatibility-and-ie8.aspx "Compatibility and IE8"
 [5]: http://adactio.com/journal/1402/ "Jeremy Keith's Article: Broken"
 [6]: http://www.vfc-oh.org/cms/site/841df35d572b686e/index.html "Voices for Ohio's Children"
 [7]: http://shallowthoughts.org/2008/01/22/the-bruhaha-of-the-meta-declaration/
 [8]: http://shallowthoughts.org/2008/01/24/more-on-the-meta/