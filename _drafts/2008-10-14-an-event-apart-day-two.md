---
title: 'An Event Apart &#8211; Day Two'
author: Bridget
layout: post
permalink: /2008/10/14/an-event-apart-day-two/
categories:
  - An Event Apart
  - Web Stuff
---
I’m attending An Event Apart, a great conference for people who make websites. My plan is to take notes during the presentations mainly so that I remember all the great stuff I heard, but also to share with my friends who couldn’t attend.

I also plan to create just two posts &#8211; Day One and Day Two. So, if you are one of the folks following along, I’ll publish the post section at the end of each presentation. All of Day One’s presentations will be contained in Day One, while Day Two will be in a post dedicated to day two. Hopefully, that is plain and obvious. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

On to the meat of the posts…<!--more-->

### Eric Meyer

Eric was at yesterday&#8217;s after party longer than the rest of his Cleveland pals, so we have no idea how much time he actually had to prepare for today&#8217;s presentation which is a live code workshop. This presentation is based on user submitted questions from yesterday, so it isn&#8217;t like he can fake it! Good luck, Eric. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

#### Stratom.com

Stratom.com has a <span id=uyjb><a href=http://blogsbycity.com/lib/pet-vitamins/vitamins-for-dogs-skin.html>vitamins for dogs skin</a></span>  
few superfluous divs and a touch of span-itis in the menu, but overall it isn't horrendous. Eric is happy that no one submitted a table based site to be reviewed today because 3 or 4 years ago they would have still been on the radar.

There are some classes with names that are lacking like "style21" and there were still some align="left"s and there was a div with a bunch of empty paragraph tags. His main beef with the site regardless of these other items is the div that surrounds the menu which is an unordered list. He pointed out that that div didn't "do" anything so it was unnecessary. The ul would be the containing element.

He also suggested that there are sites that will create a header div that has the h1 to hold the logo, a few links and a search box. He explained that you could put the h1 and the links inside the form that the search box will be in. Think smart about what container type elements are already on hand and make good use of them instead. Divs are not a requirement. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

#### McKesson.com

McKesson is designed in pixel-based text which would have once been a criticism point, but with the advent of page zoom and the impending death of IE6 it isn't a big deal anymore. 

Some of the class names were not helpful, such as {p class="p"}. He was actually impressed that they had extended their brand in their file extension. He noted that there was a missing background-color declaration in the body, so he changed it to lime in the user stylesheet to show how sad it looks in the hands of others. 

If you are going to set your text in pixels, he recommends setting that in the body and then use percentages on headings and other elements. That way, scaling is still used and should there ever need to be a change in the base, there is only one line to alter instead of many places to be hunted down and changed.

He praised them for putting background images on the list item, but wondered why they weren't set on the anchor in order to allow the bullet image to also extend the region that is to be clicked.

#### Delta.com

There are style attributes placed in the html markup and he recommends stopping that. This site has divs everywhere. Tons of them. Especially when you get to the section that is a complex form. He wondered why it wasn't in a table. For accessibility reasons, putting some th's with scopes might make the form easier to use for visitors who employ speaking browsers.

#### TabletHotels.com

The sidebar links do not belong in paragraphs. They are list items. He also didn't understand why the footer was a paragraph separated with lots and lots of spans. Perhaps it should have been a series of lists or even a table, but it wasn't intuitive in a paragraph.

### Rob Weychert

#### Design Lessons in Chess

Rob read two books on chess: Pandolfini's Ultimate Guide to Chess (Bruce Pandolfini) and How life Imitates Chess (Gary Kasparaov). What he found interesting is that he found concepts in those two books that resonated with him as a designer.

#### Correlations

Chronology: 3 parts in both chess and in web design to succeed (hopefully).

1. Opening - Information Architecture  
2. Middle Game - Visual Design  
3. End Game - Build

#### Opponent as User, Client, and Colleague

In chess, the strategy is that you want to lead your opponent to the end that you desire. You make moves in order to limit their options so that they do what you want them to do. This is much the same way we build a site. We try to lead the user through the path we desire to the end of our choosing (conversion).

There is a back and forth interaction during the process of design much like there is in the back and forth of a chess game. In chess, you want to play opponents that challenge you because it will improve your game. The same holds true for clients because if we don't, we don't improve as designers.

#### Content is King

In chess, winning or losing is based on what happens to the king. If the king is captured, the game ends. Often times, in a strategy for a game, the strategy will become the focus and lose sight of what will happen to the king. In design, we can often get so focused on things like incorporating AJAX-y goodness, that we forget to make support, guard and protect the content (king).

#### Know Your History and Think Ahead

While content is king, context can provide meaning, cohesion, and support information delivery. Researching what will support the content in context in the best way possible takes effort, just like understanding your opponent's skills, playstyle and mindset.

In chess, expert players can view a board and think many moves ahead. What makes designer's stand out in the industry are those who can think ahead. Designer's who don't think ahead about what a site's needs may be will ultimately fail their client's.

#### Don't Get Too Attached

Novice chess players recognize how powerful the queen is, but will get distracted trying to protect her and leave their king unprotected. Better chess players consider looking for a better move when they find a good one. As designer's we should do the same. Stopping at your first good idea isn't smart. Consider other options.

#### The Journey is as Important as the Goal

Success is based on some sort of failure. It's a process of elimination. With attempts at greatness, you find out what didn't work and remember that in the next project.

### Dan Cederholm

Implementing Design. Bulletproof A-Z

#### Craftsmanship

When something is well-crafted, it reflects that a human was behind the design.

Bulletproofiness (my term, not his) consists of:  
Flexibility  
Adaptable to multiple scenarios  
Adding detail without complexity

A. **Anchor links with meta information**: typical modules encapsulate a list of links with some numbers on the right. Making the whole line clickable rather than just the link text. Link text could become longer than expected (likewise, the number) so what works better? Absolute positioning? or Floats? (The answer is floating).

B. **Border-radius**: Even though it isn't a property that can be used across the board, it can be implemented as we wait for the CSS3 spec. A good ideas is to put those kinds of properties into their own stylesheet (he calls his "enriched.css"). While Firefox 2 doesn't do rounded corners well, if the contrast is low enough, you can get away with it.

C. **Color Transparency with RGBa**: This sets the opacity value for background-color only). This is easily implementable by declaring background color in the standard way and then overriding it with RGBa for browsers that recognize it.

D. **Do Websites Need to Look Exactly the Same in Every Browser**: The answer is no.  
**Decision Makers Who Get It**: it's great to be able to work with people who understand that not every browser will do the same thing. Understand that this is in regard to tiny visual enhancements that don't affect the layout.

E. **Easy Clearing of Floats**: Dan uses clearfix often, but discovered that the class name can be offputting to clients, so he changed the name. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

F. **Frameworks**: Dan writes his own. The fixes are there, the reset may be there, and stubs for the things that are commonly found from project to project.

G. **Gridlasticness**: Grid layouts using EMs. Em-based layouts force you to ensure flexibility. Setting a base of 62.5% makes the math easier, but don't set the widths on the same element that you set the font-sizes. Be sure to set a max-width of 100% for elastic layouts to ensure a horizontal scroll bar will not appear.

H. **Horizontal Grid? Sure. Vertical Grid. Sort of.** Break out some of the modules into classed groups in order to realign the tops to create the appearance of a vertical grid.

I. **IE8 Still Refuses to Resize Text in Pixels**: WTF? Does page-zoom affect this? Since the text size tools are still there, we have to think about this.

J. **J-Query**: At it's core, Jquery is one file and is very "css-like".

K. **Kitty**: Just because. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

L. **.last**: Making use of a last class for presentation changes can be accomplished using Jquery.

P. **Parallax**: It's a fun treat for those who stumble upon it. Not everyone will see it, but it's a nice touch. Position the background with a negative percentage to get such an effect of movement.

T. **Today's Macbook Event**: Duh.

U. **Ur (your) Stats**: Your stats dictate when you can drop support for any older user-agents. Global aggregated stats are not helpful in any real sense.

### Cameron Moll

As a designer, a key skill is the ability to influence and draw people in.

Few things build trust better than results. Do good work, thoroughly and promptly.

Relationships between designers and developers is critical. Projects go better when there is continual communication between these two groups.

Great communication skills create the shortest distance between an initial idea and a successful user experience.

There are times when it is useful to remove "hi fidelity" from comps to keep the conversation and communication focused on features for the stakeholders. Grayscale wireframes can aid in keeping the focus of attention on functionality over how pretty it is in the end.

Cameron recommends holding annual design review and weekly design reviews. Along with that, provide in house workshops to increase and maintain quality in staff skillsets.

### Curt Cloninger

Curt is going to explain to the audience how the arts&crafts movement of the 1800s applies to modern webdesign. At a time when there were not designers operating letter presses, but rather "jobbers," William Morris emerged to bring order to graphic design. William Morris was initially a wallpaper and textile pattern designer. His mantra was to remain true to the medium upon which you are working.

#### Stay True to Nature and Materials

You need not replicate nature, but allow it to inspire you and influence your work. Curt suggested that the "natural medium" in which we work is typography (as opposed to pixels). We need not simulate a physical material like brushed metal and shiny glass.

Typography as material:

Push CSS typography. letter spacing and font-size can vary the appearance of type and create a kind of influence. Oversized text = easy to use (according to feel).

Behavior as material: It should like it does what it does. Interstitial animation is a narrative of progression through a site.

Insincere objects, such as scrollbars that might lead one to believe you will reach the bottom of the page in an expected amount of time, but pop up higher unexpectedly are not intuitive and are not true to something in nature, like using a stick to measure something.

#### Value Utility. Value Beauty.

Not everything has to be useful. It's ok to have something just because it's beautiful. While modernism is often championed in web design, people enjoy beauty. Why not inject beauty into a site to get people to hang around more? People are attracted to beautiful things. Just remember that adding that touch of beauty needs to be integrated into the design, not just tacked on without a cohesiveness to the rest of the design. Example: Cameron Moll and his use of frilly bits or the ornamentation that enhances A List Apart and An Event Apart's sites. That's beauty that doesn't "serve a function" but doesn't appear "tacked on."

### Jeff Veen

Our job as designers is to find a story in the data and assign different visual cues to each dimension of the data. This will provide tangible context that might not be easily grasped. Remove everything that isn't telling the story.

We also have to let go of control of the artifacts of how the data will be viewed, as the user has control over what device will consume the content. It's also beneficial to provide various tools to allow the users to find their own story (or preference of a story) in which to display the data.

Provide filters to enable clarity. Enable tools that allow users to scale down the scope of the data presented to access the story they are interested in.

### A Panel Apart

**How do you handle clients who will not hire a copywriter and insist on writing the content themselves?**  
Happy Cog has copywriters on staff, in house, and they "include" it in tandem with the Information Architecture process (if you need to "hide" the costs) in billing. He then suggests scaling back in other areas, where possible.