---
title: 'An Event Apart &#8211; Day One'
author: Bridget
layout: post
permalink: /2008/10/13/an-event-apart-day-one/
categories:
  - An Event Apart
  - Web Stuff
---
I&#8217;m attending [An Event Apart][1], a great conference for people who make websites. My plan is to take notes during the presentations mainly so that I remember all the great stuff I heard, but also to share with my friends who couldn&#8217;t attend.

I also plan to create just two posts &#8211; Day One and Day Two. So, if you are one of the folks following along, I&#8217;ll publish the post section at the end of each presentation. All of Day One&#8217;s presentations will be contained in Day One. Hopefully, that is plain and obvious. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

On to the meat of the posts&#8230;<!--more-->

### Jeffrey Zeldman

#### What is Web Design?

What does a web designer need most? Empathy. He shows (previous?) design of [Real.com][2]&#8216;s website. There are a lot of numbers on the his image showing that the page is out sync with user&#8217;s needs in many, many ways. Internal marketing pressures worked against each other by making the free player hard to find, when it needed to be easy to find to get penetration in the market, if the goal was to surpass Windows Media Player, Flash, etc.

[ConsumerSearch.com][3] &#8212; lack of seduction for end user. The page looks like a phishing or spam site with a gazillion links, but there is actually good information. Sadly the user isn&#8217;t likely to stick around to find that out. There is no welcoming copy and the content doesn&#8217;t provide a brand message. The interface from one page to the next changes, so the user isn&#8217;t trained how to make use of it.

#### It&#8217;s Rough Out There for a Web Designer.

Most of the room was made up of people doing web design for 5 or more years. Everyone in the room believes they are self-taught. **Good education is hard to find.** Teaching Excel is not the same as teaching business. Teaching people in software use is NOT teaching people how to be web designers.

#### ALA Survey Info

Jeffrey showed how fragmented the data is from the survey. There is no standardization of titles for people who work on websites. Organizations have varying degrees of understanding of where to place people who build and maintain websites within their org chart.

People who build websites are not likely to get rich doing this job.

15% of our industry is made up of women.

#### Who Speaks for Web Design?

Who is out there explaining what makes for really good web design? He explained that award shows are generally considered to be a source for a level of &#8220;excellence&#8221;. Example: The Oscars. He then explained the Annual Interaction Awards. He didn&#8217;t comprehend what the criteria was for the &#8220;excellence&#8221; in the sites that won. While they may have &#8220;looked&#8221; cool, it didn&#8217;t seem to consider the user of the site.

Judging is only as good as the process. The Webby Awards process appeared to be groping for what the standard of excellence is.

The News Media focuses on who is &#8220;getting rich&#8221; in the web, as if that is the measure of &#8220;excellence&#8221;. Examples: Facebook, Twitter, Yahoo.

#### The &#8220;Guitar Solo&#8221; Approach

The guitar solo is more about flashy and &#8220;look what we can do&#8221;. The songwriting approach to design is about getting out of the way so that the user enjoys the experience. Good design is *invisible*. Good web design is about the **character of the content**, but not the **character of the designer**.

#### 12 Tips to good webdesign

1. Start with the user. Follow your passion.  
2. Know yourself. Know your limitations.  
3. Find the right clients. Find the job that is the right fit for you.  
4. Sell ideas, not pixels.  
5. It is okay to say &#8220;I don&#8217;t know.&#8221;  
6. Build trust.  
7. Bring out the big guns. (consultants and publications to back up your claims)  
8. Create a paper trail.  
9. Never underprice your work.  
10. Never work for free (spec work).  
11. Say not to rush jobs.  
12. End with the user. End with your passion.

### Eric Meyer

#### Debug/Reboot

Eric built a debug stylesheet for his use. He uses this in conjunction with the Web Developer Toolbar and Firebug (in Firefox as his development platform). He finds outlines to be more helpful in diagnostic styling than borders because outlines won&#8217;t shift the layout the way borders can. He also explained how the &#8220;not&#8221; criteria works and ways to get around weirdness.

#### Things in His Debug Stylesheet

1. It checks for is &#8220;empty&#8221; content such as divs, spans, paragraphs, list items, table heading and table cells.  
2. It checks for elements that don&#8217;t belong such as a [style], font, center, empty class attributes and empty id attributes.  
3. It checks for missing images or missing alt and title attributes.  
4. It checks for missing table summaries, missing table heading scopes.  
5. It checks for links without title attributes.  
6. It checks for hrefs that have hash signs instead of actual links.  
7. It checks for a determined level of nested divs. Something crazy, not something within reason.  
8. It checks for forms that don&#8217;t have an action of method.  
9. It checks that input elements are not children of the form element. (Inputs should have a fieldset as the block element separating them). It also checks that there is a block element inside a blockquote, so that the text is not a child element. (At the very least, there should be a &#8220;p&#8221; tag &#8212; where applicable &#8212; surrounding the text inside a blockquote).

In no way does Eric advocate that the debug stylesheet he uses is **the** debug stylesheet. But, he does recommend using one for sites that you have inherited to find wonky markup or for stuff that a CMS may spit out.

#### The Reset (Reboot) Sheet

Next, he advocated why a reset sheet can be useful. Mainly, the fact that each browser uses subtly different default styles to apply padding, margin, and line-height. A reset stylesheet will allow you to create the look and feel for a site from a blank slate. However, he doesn&#8217;t advocate using the reset stylesheet that he has written (that many people make use of) without altering it to fit the base styles that you commonly use. In his opinion, it is wasteful and silly to add a declaration in another stylesheet, if you use the same values on a regular basis. Make those common declarations part of the reset sheet and go wild from there. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

Next, Eric spent time explaining all the things he learned about browsers and how they address styling and inheritance. As usual, they don&#8217;t all handle things the same way. He also gave an explanation about the evolution of the reset stylesheet that he has shared with the world as a result of the things he learned whilst &#8220;breaking&#8221; things he didn&#8217;t think it should break.

Eric recommends that if you are going to use a CSS framework, it should be a framework that *you* built rather than one that someone else built.

### Jason Santamaria

#### The Meaning of Web Design

Storytelling *by design*. In children&#8217;s books we are taught (at a young age) to look for meaning in images. Imagery that we present support the story (graphic resonance). Imagery also sets the mood and allows your mind to &#8220;create&#8221; the rest of the experience.

Jason complimented Wired Magazine (printed version) for making use of visuals to set the mood and tone of an article. He showed how it did not translate into the online version of Wired Magazine. It is the same text, but the visuals were gone. The stories were distilled down to content. While content is king, storytelling by design enhances the content and supports the experience. We are plagued by sameness in layout across the web.

We&#8217;re all capable of telling a story. Why haven&#8217;t we created fantastic stuff? Where is the fantastic web design?

#### The Nature of the Medium

Designers have common principles that are no longer common when moved online. Here are the constraints we deal with:

1. The metaphorical page  
2. Ubiquity and WYSIWYG  
3. Collections of pages (attainability & grasp of depth)  
4. Layout

Ratios (such as The Golden Ratio of 1.618) and The Rule of Thirds don&#8217;t apply in the same way for web design as it does in print design. Most of the web runs on a single fixed dimension: *width*. But we can&#8217;t even predict what kind of device will be used to view our work.

Jason showed examples of websites that aren&#8217;t &#8220;standard&#8221; such as (the old) Fray, [A Brief Message][4], and [No One Belongs Here More Than You][5]. These sites focused more on how to support the story being told and the message being conveyed. He also explained that the redesign of [his own personal site][6] took a lot of forethought and pre-planning to make his site flexible enough to convey a message along with the content he provides.

### Sarah Nelson

#### Design Criteria

Design Criteria are a set of 5-7 short, memorable strategic directives your team can use to focus design activities. Design Criteria emphasize specific rules your team will follow when tackling the **problem at hand**.

#### Constraints are Freedom

Constraints help us generate ideas, evaluate ideas, make decisions, and move forward. Common constraining tools are things like mission statements, brand guidelines, personas and demographics, design principles and best practices.

When people ask her to &#8220;design outside the box&#8221; she spends time trying to analyze the box in the first place. Is it viable in the marketplace, is it desirable and is it feasible?

#### We Don&#8217;t Design Alone

We work with fellow designers and developers, PMs, CDs, bosses, clients, peers, writers, marketers, business owners&#8230;and more. Each of those people have their own view of &#8220;the box&#8221; which will end up influencing the end result. Once all of the members of that collaborative group &#8220;understand the box&#8221; they can come together with that understanding of the box as a platform to generate relevant ideas.

The creative process begins by exploring all the possibilities (divergence). As decisions need to be made, the process begins to narrow the field of view (convergence). Design criteria fits in the middle between the divergent and convergent phases of the process.

#### Google&#8217;s Design Criteria for Google Calendar

- Easy, visually appealing, and joyous to use  
- Drop dead simple to get information into the calendar  
- More than boxes on a screen (reminders, invitations, etc&#8230;)  
- Easy to share so you can see your whole life in once place  
- Open API&#8217;s  
- Invitation for everyone

Note that the above statements are constraints, but they are not so detailed in their description as to impose severe limitations. Constraints are good. Pigeon-holing is not good.

Statements like &#8220;We need to increase conversion rates&#8221; is *not* an actionable item. Turning that statement into actionable items required research. Context and Mental Models interviews regarding attitudes language, objects made and used, other people, learning patterns, content and emotions. Expectations and Experiences intercepts regarding expectations before starting the (account) set-up process; experience expectations once in the set-up process.

Design Criteria for the above scenario:  
- Be human  
- Work the way your customers do  
- Set expectations  
- Show progress  
- Find efficiencies

Design Criteria for Design Criteria  
- Come from anywhere  
- Start from the start  
- One brain, many brains, one brain  
- Art, not science  
- Support with evidence  
- Criteria everywhere

Generating Design Criteria: List out all criteria candidates and sort into 5 &#8211; 7 groups. Discuss and refine.  
Synthesizing Design Criteria: Looking at the 5 &#8211; 7 groups, take a stab at a list. Sometimes it helps if just one person does this and the group reviews and refines.

Criteria must be clear and concise but not so abstract they don&#8217;t suggest concrete solutions. Yet, they must be open-ended enough that they don&#8217;t dictate solutions.

### Robert Hoekman, Jr.

He lives in Arizona, which means he can see Mexico from his house. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_wink.gif' alt=';)' class='wp-smiley' /> 

#### On-the-Spot Usability Reviews

Robert is taking volunteers from the audience suggesting sites that they had a hand in developing, to provide a critique of Usability. The 3 most crucial elements to consider are: purpose, benefit, usage.

#### TheIdeaCenter.org Critique

The use of images on a site, primarily a home page should be considered as if they were being used on a billboard near a freeway. What does the image convey as someone blows by at 60 miles an hour. Does it convey the message and support the content on the page?

He recommended taking the 4 panels on the right and making them larger entry points to the site, so that it is more obvious that they are action areas.

#### ASUFoundation.org critique

The <span id=ppfh><a href=http://blogsbycity.com/lib/pet-vitamins/hartz-cat-vitamins.html>hartz cat vitamins</a></span>  
main goal of the site is to get people to make a gift to the foundation, but it also strives to impart information about where the money goes and how it is used. First noted item is that the "Give to ASU" button is very tiny, so that make it difficult to achieve the primary goal.

Robert recommended taking the news listings on the right out and make them bullet points that are compelling action statements leading people to confidently make a gift. When landing on the "Give to ASU" page, he recommended taking the text that is there and changing it to be bullet point information blurbs that are the FAQ of what happens when a gift is made.

On the wizard that leads to the person making a donation does have a progress meter, but he recommended making it more obvious so that it stands out more. He also recommended removing any "crufty" text that doesn't apply solely to completing the form or transaction.

The dropdown menus are gigantic on this form and has likely been the cause of a 99% abandonment rate on that page. Robert recommended having a page that is actually the page prior to directing the visitor to the form. Perhaps that new page could be informational that streamlines the "fund selection" so that when the person is dumped in the beginning of the form, it relates to the fund page from which they were sent. In this way, the dropdown list is no longer necessary and the process feels more intuitive.

#### Easy Usability Testing

An easy way to get feedback on your sites: take a screenshot of one of the pages of your website. Show it to a user for 5 seconds. Take it away. Ask them to write down everything they remember about the page. If their list and the main action item your page was supposed to promote do not line up, you know you have work to do on that page. <img src='http://shallowthoughts.org/wp-includes/images/smilies/icon_smile.gif' alt=':)' class='wp-smiley' /> 

There is an online application at [fivesecondtest.com][7] to make use of this kind of quick and dirty usability testing on a very basic level.

### Jason Fried

First of all, he looks like the nationally famous version of our local Clevo Nerd, [Brendan Cullen][8]. While not a dead ringer by any stretch, there is clearly a resemblance in appearance and mannerisms.

#### Craftsmanship

Weak, Normal and Strong text are important enhancements that can be made to already solid structure. Normal and Strong text are achievable in HTML but Weak is not. At least, not as a tag. The purpose of making something "weak" is so that it isn't necessary to embolden items. Being able to recess things, or push them back is very useful. He used examples of that usage in 37signals application, Basecamp.

#### Anticipate the Flow, Sharpen the Focus

He compared a product called iPrioritize and it's workflow in comparison to 37signals Tadalist. Both accomplish the same task, but one takes more clicks and more effort that the other. His point to the audience is that when creating an application, consider the workflow of the user to streamline the process with less "moving around" where possible and where it makes sense.

He is demonstrating how applying focus for the user rather than making them use their mouse to focus on the first action is a way to simplify a task. Consider how to focus the user's attention on what they may need to do next. Make it so that people can use their mouse less. Hitting enter and moving to the next focus is easier.

#### Copywriting is Interface Design

Simplify text. Use natural language. Case in point: instead of "setting permissions" (public, private, etc) use something like "Who can see this?" with these options in the list:

Everyone  
Only I can  
Select a group...  
Select people...

Always choose to be clear over being clever.

Follow through with conversational text throughout the application, not just main areas.

Another example: Instead of saying "Advanced Search" explain what fields are the alternative to the short version. So what if the link text is long? Make it explicit, within reason.

Anything that needs to be explained within an application, it is a good practice to keep the text to 3 sentences. The first sentence should be a summary, the second should be an example, the third should be a suggestion/recommendation.

#### Timing is Everything

In Basecamp, there are "nubbins" that pop up when hovering over something. It was a feature that needed more than just "hover" consideration. What if the user overshoots the nubbin? It is a good idea to let the item remain on screen rather than disappearing instantly. 0.25 seconds after the mouse has left the hover region, then it disappears. That seems to be a short but reasonable amount of time to allow a user to return when overshooting without conflicting with intended movement between items.

The same holds true for navigation. Rather than having top navigation continually popping dropdowns when someone is trying to move their mouse up (maybe to something within the chrome of the browser and out of the app) make it take 0.25 seconds before the drop downs or flyouts appear.

#### Photographic Memory

Keep track of where users were when they left a product or application so that when they return, they are dropped back in right where they left off. He also illustrated how adding a task in High Rise "remembers" whether the last task that was added was a task that everyone could see. They wouldn't become private again until the user selected it intentionally. This way, preferences and settings for an application are customizable on the fly and doesn't need to be located on a different page or in a different section.

#### What Just Happened?

Make use of things like the yellow fade technique to let the user know that something changed. If something is deleted, use a motion set to reasonable time that visually reminds the user something just changed. (Such as, having the text slide up.)

#### Extreme Detail

1. Give users a little feedback for something that looks intentional. It will help confirm that is the intended act -- but choose wisely when to apply such feedback. General or comment mouse movements don't need flashes of feedback which will be annoying.

2. Find spots in your application where you can eliminate error messages. In Basecamp, if a user doesn't provide a name for a ToDo list, it doesn't generate an error because a required field wasn't filled in. Backpack just provides a generic "answer" to the required field which the user can change later when they want.

3. Provide "previews" where applicable as a nice touch.

4. Autoscrolling when a user is at the bottom of a page when they click a link that should open an accordion feature is another nice touch so that users can see the changes that take place that otherwise wouldn't be visible because they were "below the fold".

The details in applications are not something you are going to spend a lot of time in the first and second iteration of development. Features and bug fixing should always come first. But working these details in can be sprinkled in over time and included as features are revisited for improvement.

### Andy Clarke

#### The Relationship Between Comic Books and Web Design

Comic book production has to be in sync or the end product isn't going to work. The same should hold true for the web.

Panels in comic books are not there merely to hold content. They help tell the story.

Comic books are highly visual -- how do we translate that to the web?

Andy recommends reading a book called "Understanding Comics" by Scott McCloud for inspiration.

What goes on between the panels is just as, if not more, important than what goes in the panels.

The size of the panels doesn't necessarily have to respond to how much content is going inside it, but on how much time is to be spent on that panel.

Panels without borders (or visually different than other panels) can bring attention to them because the eye has an opportunity to be drawn to the edge of the layout and devoting more time from our eyes.

Panels can help direct users through the content, leading their eye to the various sections with intention.

Placement of images can also help a user work their way through the content. Images with human faces in them draw the eye directly to it.

Think about building up drama in...

...a product launch  
...a news item

Front pages of comic books orient the reader as to what has gone before...what the content/site is about...and orient them to what they might expect next...even if what comes next will be surprising.

 [1]: http://www.aneventapart.com/
 [2]: http://www.real.com/
 [3]: http://www.consumersearch.com/
 [4]: http://abriefmessage.com/
 [5]: http://noonebelongsheremorethanyou.com/
 [6]: http://www.jasonsantamaria.com/
 [7]: http://fivesecondtest.com/
 [8]: http://www.brendancullen.com/