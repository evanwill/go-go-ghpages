---
layout: default
title: 0-Prep
---

# Workshop Prep

To get ready for this workshop, please create a free [GitHub account](https://github.com/join) if you do not have one already.
Basic familiarity with the GitHub web interface and Git will be helpful. 
If you have time, check out GitHub's [Hello World guide](https://guides.github.com/activities/hello-world/) and [Try Git](https://try.github.io/).

# Local Jekyll Setup [optional]

The workshop will introduce several ways to create gh-pages without using Jekyll locally. 
However, if you would like to do development with Jekyll on your laptop, it is necessary to install Git, Ruby, and Jekyll.

## Install Git

[Git](https://git-scm.com/) is a [free](https://www.gnu.org/philosophy/free-sw.en.html), [distributed](https://en.wikipedia.org/wiki/Distributed_version_control) version control system. [GitHub](https://github.com/) is a Git repository hosting service, a place to store and sync your work in the cloud--your Jekyll and GitHub Pages projects will be under Git version control, so you need the software on your machine. 

- Windows: install [Git for Windows](https://git-for-windows.github.io/) using the default options. This will give you Git, Git Bash, and Git GUI. Git Bash is a great terminal that lets you use UNIX style commands on Windows.
- Mac: check if Git is already installed by opening terminal and typing `git --version`. If you do not have it, download the official [Mac installer](https://git-scm.com/downloads).
- Linux: install from your distribution's software center or package manager (for Ubuntu `sudo apt-get install git`).

If you are interested in using a visual GUI application integrated with GitHub, Windows and Mac users should also install [GitHub Desktop](https://desktop.github.com/) using the default options.
You can install GitHub Desktop in addition to other versions of Git.

There are other [GUI apps available](https://git-scm.com/downloads/guis) for managing and visualizing Git repositories, including Linux options.

## Install Ruby

[Ruby](https://www.ruby-lang.org/en/) is a fairly young and developing programming language with some unique features. 
To use Jekyll, you do not need to know anything about Ruby, but if you are curious, check out [Ruby in 20 minutes](https://www.ruby-lang.org/en/documentation/quickstart/).
Frustratingly, different versions have many dependency and incompatibility problems.
Because of these issues, many use Ruby Managers, such as [RVM](http://rvm.io/), to switch between versions.
However, if you are just interested in working with Jekyll, using an installer for your OS should be sufficient.

- Windows: Use [RubyInstaller for Windows](https://rubyinstaller.org/). 
    - First, [download](https://rubyinstaller.org/downloads/) the most recent 32-bit version and double click to install. Use the install defaults, but make sure “Add Ruby executables to your PATH” is checked. 
    - Second, from the same [download page](https://rubyinstaller.org/downloads/), download the Development Kit for the Ruby version you installed. Double click the DevKit file to extract, saving it to a permanent location, such as `C:\rubyDevKit`. Then open the directory in a terminal and run the commands `ruby dk.rb init` and `ruby dk.rb install`.
- Mac: Use [Homebrew](https://brew.sh/), `brew install ruby`
- Linux: Even though the version will not be the most up-to-date, use your distro's repositories. For example on Ubuntu, `sudo apt install ruby-full`. Make sure your version is > 2.0. You will also need the build tools Make and GCC, on Ubuntu get them with `sudo apt install build-essential`.

## Install Jekyll

> Note: Jekyll does not officially support Windows, however it is cross platform (they just don’t officially write windows documentation or check for bugs). 
> There is a [Jekyll on Windows](https://jekyllrb.com/docs/windows/#installation) page, but it is out of date and inaccurate.

Jekyll is a Gem, a software package installed via Ruby's management system called RubyGems (similar to Python's Pip). 
Open a terminal and type:
`gem install jekyll bundler`

Note: Linux users may need to `sudo`.
This might take a minute as Gem installs all the dependencies. 

> On Windows, if `gem` returns an error about secure connections, it may be necessary to update to a newer version of RubyGems as some versions have out of date SSL certificates.
> Manually install the newer version by downloading the [RubyGems zip package](https://rubygems.org/pages/download#formats).
> Unzip the package, then run `ruby setup.rb` in the directory.

# Text Editor

When working with code you should have a good text editor.
Windows notepad does not handle UTF-8 encoding or UNIX line endings that are standard for most cross platform applications. 
For basic editing, Windows [Notepad++](https://notepad-plus-plus.org/), Mac TextEdit, or Linux Gedit are sufficient.
However, a more complete code editor will be helpful for managing Jekyll projects.

Open-source cross platform suggestions:
- [Visual Studio Code](https://code.visualstudio.com/)
- [Atom](https://atom.io/)
