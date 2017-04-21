---
layout: default
title: 3-Jekyll
---

# GitHub Jekyll Project

[Jekyll](https://jekyllrb.com/) is a static site generator originally focused on creating simple blogs from plain text files.
It has developed into a fully featured generator used on all types of web projects from tiny to huge.
Gh-pages uses a Jekyll build service to generate all static web content.
The basic demos presented so far don't actually use any Jekyll features.
However, a full fledged Jekyll project can be created with just a few files in a repository.

> Note: file names starting with an underscore `_` are special files to Jekyll. 
> Be sure to include them correctly!

Demo using the [Minima](https://github.com/jekyll/minima) theme:

1. Create a new repository: 
    - Click the + sign in the upper right and select *New repository*. 
    - Give the repository a nice name, check the *Initialize this repository with a README* option, and click the *Create* button.
2. Create a `_config.yml` file to setup your Jekyll project (check the example [config](https://github.com/jekyll/minima/blob/master/_config.yml) for all the options):
    - Click the *Create new file* button on the repository page.
    - Name the file `_config.yml`.
    - Add the basic YAML fields required by Jekyll:

      ```
      # basic options
      title: Your awesome title
      author: GitHub User
      email: your-email@domain.com
      description: A wonderful site
      twitter_username: jekyllrb
      github_username:  jekyll

      # Build settings
      markdown: kramdown
      theme: minima
      ```

    Be careful with indentation, YAML likes exactly 2 spaces.
3. Create a `about.md` file for the About page.
    - From the repository's main page, click the *Create new file* button.
    - Name the file `about.md`.
    - At the top of the file add YAML Front Matter. Add some content. For example:

      ```
      ---
      layout: page
      title: About
      ---

      This is an about page about this awesome site.
      Hope you love it!

      Reasons:
      - its great.
      - its a test.

      ## Other thoughts

      This is great.
      ```
    - Commit the changes.
3. Activate gh-pages:
    - Click on the repository's *Settings* tab.
    - Scroll down to the *GitHub Pages* options.
    - Click *Source*, select *Master branch*, and click *Save*. 
    - Wait for a minute for gh-pages to build. The live link will appear in the options.
4. Add a blog post:
    - From the repository's main page, click the *Create new file* button.
    - Create a new directory by typing `_posts/`. The name field will update.
    - Name the file `2017-04-18-first-post.md` (post filenames must start with a date, use `-` to replace spaces).
    - Add YAML Front Matter and some content, for example,
        
      `````
      ---
      layout: post
      title: A Great First Post
      ---

      This is it!
      What a wonderful post!
      `````
    - Commit the changes, wait a minute for gh-pages to rebuild the site.

## Congrats! 

You have a Jekyll blog!

Any markdown files added to the `_post` directory with the correct filename convention will become blog post on your site. 
Markdown files added to the root directory will be come pages and show up in the navigation.

Read the [Minima](https://github.com/jekyll/minima) documentation to learn about the customization options--or just look at how the repository is set up for an example. 
If you put any file in the same place as the theme's structure, your version will replace it. 

Thanks Octocat!

{% include image.html file="octocat.jpg" alt="github octocat" width="45%" %}

> If you want to collaborate on the blog, add other GitHub users in the *Settings* tab. Look for *Collaborators* on the left side menu.
> You can keep track of the project using the *Issues* or *Projects* features.
