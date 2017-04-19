---
layout: default
title: 1-Intro
---

# Introduction to GitHub Pages

[GitHub](https://github.com/) is a cloud [Git](https://git-scm.com/) repository hosting service, with benefits!
It provides a handy web interface for managing, editing, and collaborating on remote Git repositories.
Originally designed to manage large open-source software projects, its use has expanded to many other types of organizations and individuals, with over 20 million users.
Accounts are free for public repositories--private repositories are available on a subscription pricing model.

{% include image.html file="octocat.jpg" alt="github octocat" width="45%" %}

One amazingly useful GitHub feature is [GitHub Pages](https://guides.github.com/features/pages/).
It provides free static web hosting from any repository.
Gh-pages is intended to host relatively simple sites for your GitHub portfolio, project, or documentation.
Because it is free and a valuable transferable skill, this is a great option for teaching and learning.

Many organizations are using GitHub to collaboratively create and publish public websites. 
For example: 
- [Programming Historian](http://programminghistorian.org/)
- [Software Carpentry](https://software-carpentry.org/), [Data Carpentry](http://www.datacarpentry.org/)
- this site!

> Note: gh-pages features and setup have recently changed, so tutorials and documentation more than six months old are probably inaccurate.
> There are *soft* limits and guidelines for gh-pages usage: sites should be < 1GB, use < 100GB bandwidth per month, and make < 10 builds per hour.
> If your site exceeds these quotas, GitHub will send you a notice asking you to modify the repository.
> All content must follow the [community guidelines](https://help.github.com/articles/github-community-guidelines/), e.g. no violence, obscene sex, or illegal stuff.

## Static Web

Unlike [WordPress](https://wordpress.com/) or [Drupal](https://www.drupal.org/), gh-pages is not a content management system or dynamic web application.
There is no database, server side language / processing, or admin interface.
This is known as a [static web](https://en.wikipedia.org/wiki/Static_web_page) host. 
HTML, CSS, and JS stored in the repository are served to the user without dynamic changes.

In the olden days static web was the norm, but database driven dynamic web sites have dominated the last decade.
Dynamic web applications enable features such as live comments, user authentication, and personalized streams. 
However, this functionality requires complex server-side infrastructure and processing.

Despite their limitations static sites are experiencing a [new boom](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/), because they offer some significant advantages:
- much faster performance (caching, low bandwidth, no processing time).
- low hosting requirements (simple web servers, no dependencies).
- no security vulnerabilities.
- easy version control.

To make development easier, hundreds of static site generators have sprung onto the scene (see lists at [StaticGen](https://www.staticgen.com/) and [Static Site Generators](https://staticsitegenerators.net/)).
Static generators bundle together a stack of web development tools which are used to transform a directory of source code into a deployable web site.
[Jekyll](https://jekyllrb.com/) is one of the most popular and actively developed, in part because of its integration with gh-pages.

> Static Site Generators typically feature: command line interface; builtin development server; simplified markup based content; web templating language; CSS preprocessor; file-based data options; plugin extensibility. 
