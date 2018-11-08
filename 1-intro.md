---
title: 1-Intro
nav: true
---

# Introduction to GitHub Pages

[GitHub](https://github.com/){:target="_blank"} is a cloud [Git](https://git-scm.com/){:target="_blank"} repository hosting service, with benefits!
It provides a handy web interface for managing, editing, and collaborating on Git repositories.
Originally designed to manage large open-source software projects, its use has expanded to many other types of organizations and individuals, with over 30 million users.
Public repositories are free--private repositories are available on a subscription pricing model.

{% include figure.html file="octojekyll.png" alt="github octocat" width="45%" %}

One amazingly useful GitHub feature is [GitHub Pages](https://pages.github.com/){:target="_blank"}.
It provides free static web hosting from any repository with a simple *click of a button*.
GH-Pages is intended to host relatively simple sites for your GitHub portfolio, project, or documentation.

> There are *soft* limits and guidelines for gh-pages usage: sites should be < 1GB, use < 100GB bandwidth per month, and make < 10 builds per hour.
> If your site exceeds these quotas, GitHub will send you a notice asking you to modify the repository.
> All content must follow the [community guidelines](https://help.github.com/articles/github-community-guidelines/){:target="_blank"}, e.g. no violence, obscene sex, or illegal stuff.

Because using hosting through GH-Pages is free and builds valuable transferable skills, this is a great option for teaching and learning.
Users have the opportunity to become creators and participants in global digital culture, developing critical digital literacy about the fabric of the web.

Many organizations are using GitHub to collaboratively create and publish public websites. 
For example:

- [Programming Historian](http://programminghistorian.org/){:target="_blank"}
- [Software Carpentry](https://software-carpentry.org/){:target="_blank"}, [Data Carpentry](http://www.datacarpentry.org/){:target="_blank"}
- this site!

> Note: gh-pages features and setup have changed over time, so tutorials and documentation more than six months old are probably inaccurate.

## Static Web

Unlike [WordPress](https://wordpress.com/){:target="_blank"} or [Drupal](https://www.drupal.org/){:target="_blank"}, gh-pages is not a content management system or dynamic web application.
There is no database, server side language / processing, or admin interface.
This is known as a [static web](https://en.wikipedia.org/wiki/Static_web_page){:target="_blank"} host. 
HTML, CSS, and JS stored in the repository are served to the user without dynamic changes.

In the olden days static web was the norm, but database driven dynamic web sites have dominated the last decade.
Dynamic web applications enable features such as live comments, user authentication, and personalized streams. 
However, this functionality requires complex server-side infrastructure and processing.

> `view-source:` one fascinating aspect of the web is that everyone must share code to participate. 
> Right click on any web page and select "View page source" to see the code that is being rendered by the browser.
> Right click on any element in the page and select "Inspect" or "Inspect Element" to open your browser's built in developer tools.
> This is a great way to learn about HTML and to understand how others created the sites you use.

Despite their limitations static sites are experiencing a [new boom](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/){:target="_blank"}, because they offer some significant advantages:
- much faster performance (caching, low bandwidth, no processing time).
- low hosting requirements (simple web servers, no dependencies).
- no security vulnerabilities.
- easy version control.

To make development easier, hundreds of static site generators have sprung onto the scene (see lists at [StaticGen](https://www.staticgen.com/){:target="_blank"} and [Static Site Generators](https://staticsitegenerators.net/){:target="_blank"}).
Static generators bundle together a stack of web development tools which are used to transform a directory of source code into a deployable web site.

[Jekyll](https://jekyllrb.com/){:target="_blank"} is one of the most popular and actively developed, in part because of its integration with gh-pages.
*More on that later...*

> Static Site Generators typically feature: command line interface; builtin development server; simplified markup based content; web templating language; CSS preprocessor; file-based data options; plugin extensibility. 
