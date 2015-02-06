Land Registry Digital Service Website
========================
[![Build Status](https://travis-ci.org/LandRegistry/landregistry.github.io.svg?branch=htmlproof-travis)](https://travis-ci.org/LandRegistry/landregistry.github.io)

Overview for the Land Registry digital service teams: http://www.landregistryconcept.co.uk

    $ make init
    $ make
    $ open http://0.0.0.0:4000/

# Uses
* [Jekyll](http://jekyllrb.com/) for templating and static page generation.
* [Bootstrap](http://getbootstrap.com/) for layouts and styling.
* [Font Awesome](http://fontawesome.io/) for visual decoration.
* [JQuery](http://jquery.com/) only because Bootstrap JS requires it :-(

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
