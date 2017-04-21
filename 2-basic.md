---
layout: default
title: 2-Basic
---

# GitHub Pages Basics

Any GitHub repository can have a site by activating gh-pages in the settings and selecting a source branch.
Additionally, each user and organization can have one root site by creating a repository called `username.github.io` (replace username with your actual username!).
The site will automatically appear in the github.io domain following this pattern: `https://username.github.io/repositoryname/`

Let's look at the basic ways to use it!

# Static HTML

Any static web document can be served up from your repository. 
If you add a `index.html` and activate gh-pages, you are ready to go! 

Demo: 

1. Create a new repository: 
    - Click the + sign in the upper right and select *New repository*. 
    - Give the repository a nice name, check the *Initialize this repository with a README* option, and click the *Create* button.
2. Create a new `index.html` file:
    - Click the *Create new file* button on the repository page.
    - Name the file `index.html`.
    - Write some HTML in the web editor! For example:

      ```
      <html>
          <body>
              <h1>Hello World!</h1>
              <p>gh-pages rock!</p>
          </body>
      </html>
      ```
    - Scroll to the bottom, add a message, and click *Commit new file*. (You just used Git!)
3. Activate gh-pages:
    - Click on the repository's *Settings* tab.
    - Scroll down to the *GitHub Pages* options.
    - Click *Source*, select *Master branch*, and click *Save*. 
    - Wait for a minute for gh-pages to build. The live link will appear in the options.

> All Markdown files in the repo will also be rendered to HTML using the default GitHub theme.

# Automatic Theme Chooser

The Theme Chooser is a fully automated option to create a stock page for a repository using a Jekyll theme. 
It converts [Markdown](https://daringfireball.net/projects/markdown/) files into site pages using the selected theme layout (Markdown basics are on the [Reference page](5-reference.html)).
This is a handy way to convert a README into a slightly more attractive project home page--in seconds!  

Demo: 

1. Create a new repository:
    - Click the + sign in the upper right and select *New repository*. 
    - Give the repository a nice name, check the *Initialize this repository with a README* option, and click the *Create* button.
2. Edit the `README.md` file:
    - From the repository's main page, click on the `README.md` name to open the file's page.
    - Click on the *Edit* (pencil icon) button at the top right of the file content.
    - Edit the content in the web editor. For example:

      ```
      # Hello World! 

      This is a great new site.
      p.s. gh-pages rock!
      ```
    - Scroll to the bottom, add a message, and click *Commit changes*. (You just did a `git commit -m "..."`!) 
3. Activate gh-pages:
    - Click on the repository's *Settings* tab.
    - Scroll down to the *GitHub Pages* options.
    - Click *Choose theme*.
    - Click on the theme thumbnails to get a preview, then click the *Select* button. 
    - Wait for a minute for gh-pages to build. The live link will appear in the options.
4. Add an image:
    - From the repository's main page, click *Upload files* button.
    - Drag & drop a small image file, add a commit message, and click *Commit changes*.
    - Edit the `README.md` file, adding the image to the Markdown like: `![alt text](filename.jpg)`. Also add a link to an About page, like: `[About](about.md)`. Commit changes!
5. Add an About page:
    - From the repository's main page, click the *Create new file* button.
    - Name the file `about.md`.
    - At the top of the file add YAML Front Matter (a sign to Jekyll to process the file). Add some content and a link back to the README. For example:

      ```
      ---
      title: About
      ---

      # About this project

      In a word: **Awesome!**

      See the [Home page](README.md)
      ```
    - Commit the changes, wait for a minute for the site to rebuild.

> If you want to clean up after these tests, repositories can be deleted from the Settings tab.
> Scroll way down to the bottom *Danger Zone* and click *Delete this repository*.
> 
> Another incredibly quick way to share content and documentation is to use the built in wiki feature of a GitHub repository. 
> Just click the Wiki tab and start editing.
