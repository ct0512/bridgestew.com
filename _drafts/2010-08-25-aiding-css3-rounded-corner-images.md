---
title: Aiding CSS3 Rounded Corner Images
author: Bridget
layout: article
permalink: /2010/08/25/aiding-css3-rounded-corner-images/
categories:
  - Uncategorized
---
Tim Van Damme wrote a very helpful [tip for adding CSS3 rounded corners on images][1]. To get the rounded corner effect, Tim placed an additional element around the img tag &mdash; in this case a <samp>p</samp> tag. To that <samp>p</samp> tag, he applied an inline style to set the background-image to be the same as the image being displayed on the page. Then he wrote some CSS3 magic using border-radius to round the corners. Not every image you come across will need this solution, but if you read what he wrote first, you might see why this strategy would come in handy.

The issue that arises for me comes when handing the site off to a client who will be adding images later. Depending on their skill level, they may or may not be savvy enough to add markup around an image to make this effect work. So, I&#8217;ve opted to add that element automagically using jQuery. All the caveats that go along with other javascript solutions apply here.

In my scenario, there is already a <samp>div</samp> with <samp>class=&#8221;figure&#8221;</samp> containing the image that is to have its corners rounded along with some additional text. In fact there are multiple <samp>div</samp>&#8216;s with <samp>class=&#8221;figure&#8221;</samp> on the page. So, this snippet of jQuery finds the images inside each of those <samp>div</samp>s and applies the additional markup to them:

<pre><code lang="javascript">$(document).ready(function() {

// find images inside the divs with the class of
// "figure" - and for each of them do some stuff

  $('.figure img').each(function() {

// store the src attribute for the img because we
// need it in the next bit

  var imgSrc = $(this).attr('src');

// wrap the image in a p tag and use the src
// attribute we stored earlier in the inline style
// on the p tag

  $(this).wrap('&lt;p style="background-image:url('
  +imgSrc+ ');"/&gt;');
  });
});</code>
</pre>

That&#8217;s all there is to it. Now each of the images will have the p tag with the inline style added to them, in order to make use of Tim&#8217;s delightful solution.

 [1]: http://maxvoltar.com/archive/rounded-corners-on-images-css-only