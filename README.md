Land Registry Digital Service Website
========================

Documentation for the Land Registry Alpha digital service: http://www.landregistryconcept.co.uk

    $ make init
    $ make
    $ open http://0.0.0.0:4000/

# Uses
*[Jekyll](http://jekyllrb.com/) for templating and static page generation.
*[Bootstrap](http://getbootstrap.com/) for layouts and styling.
*[Font Awesome](http://fontawesome.io/) for visual decoration.
*[JQuery](http://jquery.com/) only because Bootstrap JS requires it :-(

# To add a new page

To add a new page to the site, place a ```.html```, ```.markdown```, ```.md``` or ```.textile``` file in the root directory.

Each page must start with a Front Matter block in the following format:
```
---
layout: default
title: Manifesto
permalink: /manifesto/
---
```

For consistent page formatting, use the ```default``` layout for static pages.

Your new page content will be place inside the ```<body>```, within a ```<div class="container">``` to support responsive web design, so please be mindful of that when designing pages and refer to the [Bootstrap CSS documentation](http://getbootstrap.com/css/).

All pages in the root directory will automatically be added to the navigation bar.

# To add a new blog post

Create a new branch in GitHub for your blog post, do not push directly to master, this is so that a pull request can be raised and reviewed for your blog post before going live.

Place a ```.html```, ```.markdown```, ```.md``` or ```.textile``` file in the ```_posts``` directory with the following naming convention: ```YEAR-MONTH-DAY-title.extension''', for example ```2014-11-21-My-new-blog-title.md```

Each post must start with a Front Matter block in the following format:
```
---
layout: post
title:  "Welcome to Jekyll!"
date:   2014-11-19 15:51:18
categories: jekyll update
author: Jekyll
meta: Example blog post
---
```

For consistent post formatting, use the ```post``` layout for blog posts.
The ```title```, ```date``` and ```categories``` form part of the permalink for the post, for examplethe above Front Matter would generate the following URL: ```mywebsite.com/jekyll/update/2014/11/19/welcome-to-jekyll/'''.
The ```author``` and ```meta``` are also used on the site to provide additional information and should be used.
