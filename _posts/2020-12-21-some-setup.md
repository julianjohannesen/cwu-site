---
categories: [jekyll, learning, howto]
date:   2018-12-21 09:45:00 -0500
excerpt_separator: <!--more-->
layout: post
permalink: date
published: true
tags: [setup, config]
title:  "Some Setup"
---

The first things I did after installing the project was add all of the folders I'll need later - _pages, _includes, assets, _sass, and _data. These folders aren't included in the base install, because you don't need them unless you plan to customize your blog and add new pages and functionality. If you're fuzzy on what any of those directories do, the [Jekyll documentation](https://jekyllrb.com/docs/) is pretty good. Look at the "Content" section in the sidebar on the right.

(Most of those folders _are_ included in the Minima theme's folder, which lives in the /usr/share/rvm/gems/ruby-2.5.1/gems/minima-2.5.0 directory. That confused me at first. Why put all of the folders and files that are actually generating the site in some hard to reach place? The reason for putting everything in the Minima theme folder, is to make sure that you get the benefit of any updates to the Minima theme. You could just copy all of those folders and files to your project directory, but then any updates to the Minima gem wouldn't have any effect on your site. BTW, the command to show where the Minima theme folder is is: 'bundle show minima') 

I also spent some time looking at the config.yml file and going over some of the default settings that don't show up in the base install. The base install ha a pretty slim config file. It doesn't even include some of the config options that come with Minima, like the head_pages setting. head_pages allows you to set which pages you want to appear in Minima's navigation menu and the order you want them to be in. The About page is included by default (this is also the only page, other than the home page, that appears in the root directory), but you can include the names of any additional pages you want to appear in the menu at the top right of your site. I don't plan to use this feature, because in order to use it, you need to place your pages in the root directory and not in the _pages directory.

I looked at the "front matter" settings in the welcome post too. You don't have to include anything in a post or page's front matter, other than the 3 dashes, but there are some useful settings available, like categories and tags, and permalink and publication settings.