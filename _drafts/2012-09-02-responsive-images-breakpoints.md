---
title: Responsive Images Breakpoints
author: Bridget
layout: post
permalink: /2012/09/02/responsive-images-breakpoints/
categories:
  - Web Stuff
---
### Responsive Images Breakpoints

Yes, I’m way behind in my reading. Don’t judge me.

I finally got around to reading Jason Grigsby’s excellent post on [Cloud Four][1] which is already about 10 days old. I found myself about to submit a really long comment when I realized I’d essentially written a blog post of my own. So, instead of saying what I want to say over there, I’m saying it over here.

<!--more-->Jason muses:

> For a few months now, I’ve been puzzling over the question of how to pick responsive images breakpoints.

### Here is my reply

Maybe it’s just me who thinks this shouldn’t be *our* (web devs) problem to solve. In cases like this, when there are so many factors to consider, it is very easy to fall into the trap of micromanaging the design.

I’m not suggesting that we should ignore the problem. I just think we could be barking up the wrong tree. Several times now, it has been suggested that in the uncertain future of high density vs. standard density screens coupled with unknown/always changing bandwidth & latency: a new image format is needed. I accept that something like that will be slow in coming to fruition. I understand we still have to *do something* to bridge the gap in the meantime. Perhaps what we need to accept is some level of imperfection for now, looking toward a brighter tomorrow when a less complicated solution comes along. (Which might not be [a new image format][2] at all, who knows?)

Responsive Design has done a world of good to move web designers and developers, myself included, into accepting that fixed-width sites are not really the right design solution for the web because it’s not a fixed-width medium. (It never was!) It only took us 15 or so years to accept that fact even though [others tried to tell us][3]. Yes, I’m using a broad brush to paint, but I’m referring to our industry as a whole, not any particular group or individual.

Of course we want the sites and apps we build to look as good as they possibly can. However, given that **there is no true unifying factor** on which to base our designs and implementations, maybe the shift in thinking needs to be ours yet again – a willingness to give up *control*.

As an industry, we built fixed-width sites in a fluid medium because we had *more control* over the end result. We are currently facing the exact same problem. We are in a sea of devices that don’t make it easy for us to control the end result, but we are still fighting like hell to try by coming up with some very intricate solutions around images.

Do I want images to appear blurry on a high density device? Not really, but the bandwidth/latency considerations make it much more difficult for me, the developer, to determine which is the best image to fit the bill at the time it is being requested by the device. Until the browser can help solve that conundrum in some way, I’m banging my head looking at all sorts of articles and math that is way over my head – and I used to be good at math – to try to solve something I can’t really solve.

### I cannot control every aspect of the output

I can wrangle a lot of things as the tools get more sophisticated, but am I able to understand when it is right to put in a little more effort to achieve a great result vs. micromanaging that which cannot be controlled?

Just as John Allsopp quoted in his Dao of Web Design article on A List Apart:

> The Sage “…accepts the ebb and flow of things,
> 
> Nurtures them, but does not own them,”
> 
> Tao Te Ching; 2 Abstraction

I think the above quote applies aptly to our current attempts to solve how images look across the variety of devices &#8211; high density or otherwise. Read (or reread) his article, especially the portion under the heading “Controlling Web Pages.” Resolution density issues were actually a thing designers tried to control back in 2000. 12 years and some months after that article we’re at it again! Consider, too, that Ethan Marcotte was inspired by **that very article** when he uncovered the secret of Responsive Design.

I know that history repeating itself is a fact of human existence. But I also dream of a day when we can learn from the past.

### Bridget, what’s your point?

In all of this rambling, the point of my post today is about finding that happy medium in which to develop websites and apps:

Do what you can reasonably do to make something beautiful, but be willing to let go of that which takes more effort and/or overhead than is *reasonable* to accomplish it. This notion is not so different from giving up the notion of struggling to make every browser look the same. It’s also pretty close to the serenity prayer:

> Grant me the serenity to accept the things I cannot change,
> 
> The courage to change the things I can,
> 
> And the wisdom to know the difference.

**Wisdom to know the difference** &#8211; that’s the clincher for me. That’s the part that is almost always unclear.

 [1]: http://blog.cloudfour.com/how-do-you-pick-responsive-images-breakpoints/
 [2]: http://blog.cloudfour.com/what-a-holy-grail-image-format-would-mean-for-the-browsers-lookahead-pre-parser/ "another post by Jason"
 [3]: http://www.alistapart.com/articles/dao/