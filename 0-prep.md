---
title: 0-Prep
nav: true
---

# Workshop Prep

To get ready for this workshop, please create a free [GitHub account](https://github.com/join){:target="_blank"} if you do not have one already.
That is all you really need! 

This workshop introduces GitHub Pages using GitHub's web interface, demonstrating several ways to create gh-pages without using Jekyll locally.
Basic familiarity with the GitHub web interface and HTML will be helpful. 
For quick introductions check out GitHub's [Hello World guide](https://guides.github.com/activities/hello-world/){:target="_blank"} and w3schools [HTML Tutorial](https://www.w3schools.com/html/default.asp){:target="_blank"}.

# Optional Prep *[optional!]*

For more advanced uses of GitHub Pages and Jekyll you will want a text editor, Git, Ruby, and Jekyll installed on your computer.
The instructions below will set up your local development environment and provide a bit of background.

## Text Editor

When working with code you should have a good text editor.
Word processors such as MS Word can not be used to create or edit code.
Windows Notepad does not handle UTF-8 encoding or UNIX line endings that are standard for cross platform applications. 
For basic editing, Windows [Notepad++](https://notepad-plus-plus.org/), Mac TextEdit, or Linux Gedit are sufficient.
However, a more complete code editor will be helpful for managing Jekyll projects.

Open-source cross platform suggestions:

- [Visual Studio Code](https://code.visualstudio.com/)
- [Atom](https://atom.io/)

## Install Git

[Git](https://git-scm.com/) is a [free](https://www.gnu.org/philosophy/free-sw.en.html), [distributed](https://en.wikipedia.org/wiki/Distributed_version_control) version control system, a piece of software on your computer. 
[GitHub](https://github.com/) is a Git repository hosting service, a place to store and sync your work in the cloud.
Your GitHub Pages projects will be under Git version control, so you need the software on your machine. 

Installing it is pretty straightforward:

- **Windows:** install [Git for Windows](https://git-for-windows.github.io/){:target="_blank"} using the default options, except when setup asks you to choose the default editor used by Git, select "Use the Nano editor by default". This will give you Git, Git Bash, and Git GUI. Git Bash is a great terminal that lets you use UNIX style commands and utilities on Windows.
- **Mac:** check if Git is already installed by opening terminal and typing `git --version`. If you do not have it, your system will often prompt you to install "Xcode Command Line Tools"--follow the prompt as this package is necessary for Ruby as well. Alternatively, type `xcode-select --install` to start the process. If you want a newer version, download the official [Mac git installer](https://git-scm.com/downloads){:target="_blank"} or use Homebrew.
- **Linux:** install from your distribution's software center or package manager (for Ubuntu `sudo apt install git`).

If you are interested in using a visual GUI application integrated with GitHub, Windows and Mac users should also install [GitHub Desktop](https://desktop.github.com/){:target="_blank"} using the default options.
You can install GitHub Desktop in addition to other versions of Git.

There are other [GUI apps available](https://git-scm.com/downloads/guis){:target="_blank"} for managing and visualizing Git repositories, including Linux options.

## Install Ruby

[Ruby](https://www.ruby-lang.org/en/){:target="_blank"} is a fairly young and developing programming language with some unique features. 
To use Jekyll, *you do not need to know anything about Ruby*, but if you are curious, check out [Ruby in 20 minutes](https://www.ruby-lang.org/en/documentation/quickstart/){:target="_blank"}.

Frustratingly, different versions have many dependency and incompatibility problems.
Because of these issues, many use Ruby Managers, such as [RVM](http://rvm.io/){:target="_blank"}, to install and switch between versions.
However, if you are just interested in working with Jekyll, using an installer for your OS should be sufficient.
Jekyll requires a Ruby version > 2.2.5.

- **Windows:** Use [RubyInstaller for Windows](https://rubyinstaller.org/){:target="_blank"}. 
    - First, [download](https://rubyinstaller.org/downloads/){:target="_blank"} the suggested stable version "WITH DEVKIT" (as of this writing, Ruby+Devkit 2.5.X (x64)) and double click to install. Use the install defaults, but make sure "Add Ruby executables to your PATH" is checked. On the final step, ensure the box to start the MSYS2 DevKit is checked.
    - Second, the installer will open a terminal window with options to install MSYS2 DevKit components. Choose option 3, "MSYS2 and MINGW development toolchain", or simply press ENTER to install all the necessary dependencies. The installer will proceed through a bunch of steps outputting a bunch of text in the terminal window--*eventually*, this will conclude and you should see a message with success in it. If the window doesn't close, press Enter again or manually close it. (The installer can be restarted by typing `ridk install` into a command prompt)
- **Mac:** OS X has a version of Ruby installed by default. Check the version with `ruby -v`. If it is > 2.2.5 you can use the system Ruby. 
    - A newer version can be installed using [Homebrew](https://brew.sh/){:target="_blank"}, `brew install ruby`, or a manager such as [rbenv](https://github.com/rbenv/rbenv){:target="_blank"}. Check the official Jekyll [Mac install docs](https://jekyllrb.com/docs/installation/macos/){:target="_blank"} for tips. 
    - Ensure you have Xcode Command Line Tools, if not use `xcode-select --install` to start the installer.
- **Linux:** Even though the version will not be the most up-to-date, the simplest method is to use your distro's repositories. For example on Ubuntu, `sudo apt install ruby-full`. Check `ruby -v` to make sure the repository version is > 2.2.5. See the official Jekyll [Ubuntu install docs](https://jekyllrb.com/docs/installation/ubuntu/){:target="_blank"} for more details.
    - For a more up-to-date version, use a manager such as [RVM](http://rvm.io/){:target="_blank"} ([Ubuntu tips](https://evanwill.github.io/_drafts/notes/ruby-notes.html){:target="_blank"})
    - You will also need some build tools (Make and GCC), on Ubuntu get them with `sudo apt install build-essential`.

## Install Jekyll

> Note: Jekyll does not officially support Windows, however it is cross platform and works fine (they just don’t officially write windows documentation or check for bugs). 
> There is a [Jekyll on Windows](https://jekyllrb.com/docs/installation/windows/) page, but it can be out of date and inaccurate.

Jekyll is a Gem, a software package installed via Ruby's management system called RubyGems (similar to Python's Pip). 
Open a terminal and type:

`gem install jekyll bundler`

This will take a minute as Gem installs all the dependencies and builds extensions (on Windows it may appear as if nothing is happening, but be patient!). 

> Note: Linux users may need to `sudo`, to avoid this install Ruby using [RVM](http://rvm.io/) or add a gem install directory to `.bashrc`.
> On Windows, if `gem` returns an error about secure connections, it may be necessary to update to a newer version of RubyGems as some versions have out of date SSL certificates.
> Manually install the newer version by downloading the [RubyGems zip package](https://rubygems.org/pages/download#formats).
> Unzip the package, then run `ruby setup.rb` in the directory.
