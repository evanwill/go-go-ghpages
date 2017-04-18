---
layout: default
title: 0-Prep
---

# Prep and Installation

To get ready for this workshop, please create a free [GitHub account](https://github.com/join) if you do not have one already.
Basic familiarity with the GitHub web interface and Git will be helpful. 
Check out GitHub's [hello world guide](https://guides.github.com/activities/hello-world/) and [Try Git](https://try.github.io/).

# Local Jekyll Setup

The workshop will introduce several ways to create gh-pages without using Jekyll locally. 
However, if you would like to do development with Jekyll on your laptop, it is necessary to install Git, Ruby, and Jekyll.

## Install Git

- Windows: install [Git for Windows](https://git-for-windows.github.io/) using the default options. This will give you Git, Git Bash, and Git GUI. Git Bash is a great terminal that lets you use UNIX style commands on Windows.
- Mac: check if Git is already installed by opening terminal and typing `git --version`. If you do not have it, download the official [Mac installer](https://git-scm.com/downloads).
- Linux: install from your distribution's software center or package manager (for Ubuntu `sudo apt-get install git`).

If you are interested in using a visual GUI application integrated with GitHub, Windows and Mac users should also install [GitHub Desktop](https://desktop.github.com/) using the default options.
You can install GitHub Desktop in addition to other versions of Git.

There are other [GUI apps available](https://git-scm.com/downloads/guis) for managing and visualizing Git repositories, including Linux options.

## Install Ruby

Ruby is a fairly young and developing language with some unique features. 
To use Jekyll, you do not need to know anything about Ruby, but if you are curious, check out [Ruby in 20 minutes](https://www.ruby-lang.org/en/documentation/quickstart/).
Frustratingly, different versions have many dependency and incompatibility problems.
Because of these issues, many use Ruby Managers, such as [RVM](http://rvm.io/), to switch between versions.
However, if you are just interested in working with Jekyll, using an installer for your system should be sufficient.

- Windows: Use [RubyInstaller for Windows](https://rubyinstaller.org/). 
    - First, [download](https://rubyinstaller.org/downloads/) the most recent 32-bit version and double click to install. Use the install defaults, but make sure “Add Ruby executables to your PATH” is checked. 
    - Second, from the same [download page](https://rubyinstaller.org/downloads/), download the Development Kit for the Ruby version you installed. Double click the DevKit file to extract, saving it to a permanent location, such as `C:\rubyDevKit`. Then open the directory in a terminal and run the commands `ruby dk.rb init` and `ruby dk.rb install`.
- Mac: Use [Homebrew](https://brew.sh/), `brew install ruby`
- Linux: Even though the version will not be the most up-to-date, use your distro's repositories. For example on Ubuntu, `sudo apt-get install ruby-full`. Make sure your version is > 2.0

## Install Jekyll

Jekyll is a Ruby Gem, a software package installed via Ruby's management system. 
Open a terminal and type:
`gem install jekyll bundler`

Linux users may need to `sudo`. This might take a minute as it installs all the dependencies. 
ruby install problems on windows, ruby installer rubygems is not update, which causes SSL errors, cant download anything. manually install newer version of rubygems.
download zip from
https://rubygems.org/pages/download#formats
unzip, then run `ruby setup.rb`
