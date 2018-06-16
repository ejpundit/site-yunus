---
layout: blog
title: 'created with netlify cms :-)'
date: 2018-03-04T21:00:57.557Z
draft: false
---
# live editing

yeah, now I'm writing a new blog with netlify cms.
The documentation in netlify cms is good.
Just add an admin folder under static with two file

* index.html to include the cms
* config.yml to configure the cms

To configure netlify cms without making my hugo site know about it, there is this cool feature _Script Injection_ as part of the post deploy step. With this feature an the needed JavaScript snippets can be injected into the `head`-section on every page of the site.
