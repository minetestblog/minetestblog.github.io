---
layout: page
title: About
permalink: /about/
published: true
---

<div class="page" markdown="1">

{% capture page_subtitle %}
<img
    class="me"
    alt="{{ author.name }}"
    src="{{ site.author.photo | relative_url }}"
    srcset="{{ site.author.photo2x | relative_url }} 2x"
/>
{% endcapture %}

{% include page/title.html title=page.title subtitle=page_subtitle %}

## Welcome to The Minetest Blog!

We post updates about once per month (subject to change) to let you know whats new with Minetest. We cover everything about Minetest, from engine development, to mod and game progress, to servers and community events. Even minetest related artwork can have a place here. Posts are subdivided by general topic.

## Contributing posts

Are you working with minetest? We'd love to know what's new with you! If you have gomething great to share, please make an issue on the [github issue tracker] (https://github.com/minetestblog/minetestblog.github.io/issues) or alternatively, on the mirrored [gitlab issue tracker] (https://gitlab.com/mistere123.coding/minetestblog.github.io/-/issues) if you cannot use github.

## Submission Guidelines

We ask that you follow these guidelines when making issues to submit post content:

Required:
* In the issue, format the issue title like: ` [content] content description`. Replace `content description` with a very brief title/description of your submission.
* Include who is working on the project
* Include a brief description. Keep it short. Links to further details are encouraged.
* Do not post about extremely trivial updates. Actually share project status updates, news or something new. While shills are allowed/encouraged to a degree, you need a good excuse to shill your project. No "hey check out my project that I made last year". New projects, major updates, and events are all good "excuses".
* No NSFW content or projects allowed.

Highly recommended:
* a single screenshot or gif that *effectively* communicates your message. The screenshot may or may not be included in the final post depending on: how important your update is deemed to be by the editors, and how well the screenshot adds to understanding the message. Don't expect to have a screenshot of minetest-game included in a post about a background api update, for example. 
* include who took the screenshot.

IMPORTANT:
The blog editors will consider the content submitted for each post. They will build the upcoming post using the content provided. The issues for each content submission will be closed when the content is included in the upcoming post, or when the post occurs. You submission will not be included if it doesn't meet the basic requirements. The editors may choose to respond to the issue to give you a chance to fix any problems. Regardless, at each post release, all outstanding content submission issues will be closed to make way for the next release. Please only submit content for current updates.


## Cover screenshot
Each post should have a cover screenshot that will be the background for the title. We may also include a "minetest at its best" screenshot, showing players having fun, 

Please make submissions each month for these!
When you make the issue on Github, format the title like: `[Screenshot] `
Include who took the screenshot, and any descriptive caption you think fits well.

## Licensing

READ THIS!!

All submissions should be *your* work (you wrote the words or took the screenshot), or you should have explicit permission from the owner. 

Unless you specify otherwise, you agree to release your submissions (your words and your screenshots) under the CC0 license. Attribution will not be required, though in-text or in-caption attribution will often be made.

While you are free to specify another license for your post submission, We ask that you do so clearly at the top of the submission issue, and please understand that the editors may choose to exclude submissions that take too much effort/post space to properly attribute.



</div>
