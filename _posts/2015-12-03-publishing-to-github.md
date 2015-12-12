---
layout: post
title:  "Publishing to Github"
date:   2015-12-03 14:36:23
---

<span class="image featured"><img src="/images/publishing.jpg" alt=""></span>

Why Github?
---------------------

As stated in the history section, Jekyll was written by one of Github's co-founders. So it is no surprise that any Jekyll website can be easily and freely hosted on Github using Github Pages on it's <strong>github.io</strong> domain.

If it's so easy and so free, then why not?

User and Organizations
=====================

In order to display content for user and organizational pages, there must be a be a special GitHub repository dedicated to only the GitHub Pages files. This repository <strong>must</strong> be named after the account name. 

Use this presentation as an example:

* -- username: dSouthard
* -- repository name: dsouthard.github.com
* -- Github Page: dSouthard.github.io


Content from the master branch of your repository will be used to build and publish the GitHub Pages site, so your desired published Jekyll <strong>must</strong> be stored there.

Project Pages
=====================

Project Pages are kept in the same repository as the project they are for, except that the website content is stored in a specially named <strong>gh-pages</strong> branch. The content of this branch will be rendered using Jekyll, and the output will become available under a subpath of the user pages subdomain, such as username.github.io/project

This is the same method used in my previous presentations, where my desired presentation was always pushed to the <strong>gh-pages</strong> branch.
