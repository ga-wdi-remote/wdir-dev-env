---
title: Installation
type: Walkthrough
duration: 1hr
creator:
  name: Colin Hart
  campus: WDIR
competencies: Course Prep
---

# Installation

## Lesson Objectives

- install `homebrew` and `brew cask`
- install `Node` w/ brew
- install `Spectacles` w/ brew cask
- uninstall and install `Atom` w/ brew cask
- Verify git is installed


## Installing Homebrew
#### What is Homebrew?

Brew is a piece of software that runs in the Terminal. The Homebrew commands can be run from any directory on your computer. Using the Homebrew command `brew` you can install other pieces of software, frequently referred to as packages, or in Homebrew parlance, casks/taps.

We'll use it install all kinds of things throughout WDI: from Git and Node to Ruby and Rails.


#### To install homebrew

Here is the link to the [homebrew documentation](http://brew.sh/), which explains what Homebrew is, how to use it, and how to install it.

You should start to get into the habit of always reading the documentation for any tool, package, or language we use in class. It will be overwhelming at first and you might only understand a small percentage of what you're reading. But developing this habit early, is essential for your success in the class and your success as a developer.


According to the documentation, we simply have to paste the following command into our Terminal and then restart.

> When we say **"Run this command,"** it means type or paste the command into the terminal and hit enter."

1. Run this command in the Terminal

  ```bash
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  ```

  ![](.md_resources/brew_install.gif)

2. Restart your Terminal

3. To test that brew successfully installed we need to try and run the base command. If you run `$ brew` in the Terminal you should see what looks like a manual page. This is ubiquitous for most Terminal applications.

  run these commands in bash:

  ```bash
  $ brew update
  $ brew upgrade
  ```

If brew is used to install packages you might guess what our next step is... We're going to install a package!

We're going install Node using brew. We're going to learn a lot about Node over the next two months.

1. Run the following command from any directory:

  ```bash
  brew install node 7.0.0
  ```

## Installing Brew Cask
#### What is brew cask?

Where Homebrew lets us install packages and tools for the Terminal and other low level processes, brew cask let's us install Apps. Things like Chrome, Atom or Sublime Text, Spectacle, Slack and so on!


#### to install brew cask

According the [documentation](https://caskroom.github.io/) we need to run the following command in our terminal and then restart.

1. Run this command in the Terminal

  ```bash
  $ brew tap caskroom/cask
  ```

2. Restart your terminal.

Now you'll be able to install regular applications like Chrome using the command `$ brew cask install`

You should already have Atom installed but I'm going to ask you to uninstall it by dragging the application to the trash and emptying it. Then we're going to install Atom using brew cask.

```bash
$ brew cask install atom
```

Why did we do that? Because we installed using brew cask, it created a command in our terminal so if we run the command `atom` and we give it a file or directory name/path it will open it in Atom.

Let's test it out.

### Set up Spectacles

We're going to install one more application using brew cask. It's an App called Spectacles—[documentation](https://github.com/eczarny/spectacle)—which is going to make organizing your screen much simpler!

1. install spectacle using `brew cask`
  ```bash
  $ brew cask install spectacle
  ```

2. Open up your System Preferences

  Click the padlock in the bottom left corner so you can make changes and then check the box next to Spectacle to allow the app to control your computer.

  Spectacle gives you the ability to move your windows around quickly so you're not wasting time dragging your mouse around
  ![](.md_resources/specs.gif)

### Install Hyper

Finally, we're going to install a Terminal Emulator called Hyper.

1. install hyper using `brew cask`

  ```
  $ brew cask install hyper
  ```


### Why Hyper

The big reason is that later in the course you'll need to have many... MANY... different windows open in both terminal and in Chrome and Hyper has some nice features for splitting your Terminal window without the need for new tabs and so forth.  
