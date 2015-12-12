---
layout: post
title:  "Updating Content"
date:   2015-12-04 12:00:00
---
<span class="image featured"><img src="/images/updating.jpg" alt=""></span>

What's in a Post?
---------------------

A post is simple a Markdown file that is saved in your _posts folder with the following conventions:

1. <strong>Title:</strong> Jekyll requires blog post files to be named according to the following format: <strong>YEAR-MONTH-DAY-title.MARKUP</strong>, where YEAR is a four-digit number, MONTH and DAY are both two-digit numbers, TITLE is the title you wish to give your post, and MARKDOWN is the desired file extension.
2. <strong>Front Matter: </strong> At the top of every post, the post must include the following front matter set between triple-dashed lines:  layout, title, and date. Other data, such a a permalink, category, or tags, can also be posted.

An example of a title would be: <br>
2015-12-31-new-years-eve-is-awesome.md

An example of the blog's front matter would be: 

\---<br>
layout: post<br>
title:  "Updating Content"<br>
date:   2015-12-04 12:00:00<br>
\---<br>


After those lines...anything goes! Write into your post file as you want to, incorporating any Markdown formatting syntax as desired! As a clue, all of the pages discussing the topics in this presentation are all created as individual posts!

Markdown is one one of many supported file types. Posts can also be written in Textile, HAML, CoffeeScript, and <a href = "http://jekyllrb.com/docs/plugins/#converters-1">many others.</a>

Post Drafts
=====================

As noted when discussing the basic file structure of a Jekyll site, there is the possibility of using drafts for your posts. A draft is simply a post without a date in the front matter. This allows you to work on a post without publishing it yet. 

Jekyll does not automatically create this folder for you, but it's easy enough to make a new folder labeled _drafts and save any work-in-progress posts there. This option allows you to preview your site with your draft posts by using the <strong>jekyll serve</strong> command (or <strong> jekyll build --drafts</strong>).

Any drafts will have it's modification time used as the value for it's date, allowing you to see the draft in its current state without having to first publish it.

Post Benefits
=====================

This method of using markdown files to write up posts allows for you to write your desired content offline and then publish them as you will. It also is much easier to manage a folder full of text-based files on your own computer rather than some of the much-more intricate blogging sites that require all files to be saved online. You can also quickly tweak the layout of your entire blog by updating the _layouts files. Everything is neatly organized and laid out!

Jekyll will automatically display posts by order of the most recent, and the naming convention allows for you to find posts easily by either the date or the post title. It really is a convientent system.

What's in a Page?
---------------------

Other than posts, another way to display content is in a Page. A page is an HTML file, usually created and saved in the site's root folder. You can also create an individual folder in the root directory for each additional page you wish to create, though it creates a longer naming convention.

A page will require the same <strong>Front Matter</strong> as a post, with the note of a date being not required. Pages can be incorporated into the site just as any HTML document would, and will be processed accordingly by Jekyll.

In the Jekyll’s vision, pages should be used for general information pages, like index, abouts, or links pages. Posts are more useful for handling the web content as a blog where a new item (post) gets published by adding a new page under a predictable structure


