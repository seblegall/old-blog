---
layout: post
title: "As a developer in 2016, you need to learn Emacs (or Vi)"
description: "How to improve your productivity writing code and force yourself to think twice."
header-img: "img/emacs.png"
date: 2016-05-21 19:00:00
author: Sébastien Le Gall
category: developer-tips
tags: [emacs, vi]
---

*How to improve your productivity writing code and force yourself to think twice.*

This post is not another Emacs vs Vi troll. My point is to explain why (deeply) learning to use a low level text editor is one of the first things any software engineer should do. I have personally chose Emacs because I found common shortcuts easier to memorize. As you will see later, it doesn't matter which one of those editors you like to use, as long as you have learned to use it.

Editors like Emacs may seems old but they have been thought to be productive tools. Shortcuts are optimized with your hands place on the keyboard and the most used key. They let you do your work as quickly as you can think about it but still, they force you to think about what you're doing. Not only they let you learn how to be more productive, they make you understand what you do instead of writing code with crappy CRLF.

## Master your working environment.

I often meet developers working on a software or a web application development trying to master the programming language and the framework they use. This is a good idea, for sure. It let you being more productive with time. But, at some point, programming a new feature in your development environment is not enough to get things done. More effective and more comfortable you become with the software code, more features you should be able to design, code, and make run into production. And yet, most of the time, this doesn't go as well as you expected. There could be thousands of management and technical reasons which explain why you don't succeed at getting things done. Obviously, if your company culture is that only one of the lead developers is in charge of pushing new features into production, your possible improvement is limited *(And you probably should think about quitting you job)*. However, most of the time, this is not the reason why you can't push the feature you just get reviewed and validated into production. Most of the time, you just don't want to work *(or people don't want you to work..)* on the production environment because you don't master it.

So, as (not) expected, mastering your working environment doesn't mean mastering MS Windows. It means, however, mastering your VCS, mastering the deployment tools you use, mastering the server configuration (such as Apache or Nginx), mastering the programming language configuration, mastering Linux configuration and the Linux logging system.

As you probably know, all those tools configuration is made trough text files you need to edit directly on the server. At this point, no chance to open any of the graphical text editors you use everyday. Here is where comes Emacs (or Vi).

![Emacs](http://tuhdo.github.io/static/helm_projectile.gif)

<!--more-->

I will make it clear. If you want to master your work environment, you need to master Emacs or Vi. Any configuration operation on your Vagrant, Docker, Linux server or any element of your working environment will require to open a text file and edit it. Most of the time, even commit a change will require that you edit your commit message using a non-graphical text editor.

If you want to get things done, learn how to use Emacs or Vi.

## Improve your ability to make meaningful impacts

As a software engineer, making a meaningful impact depends on your ability to think about scalable solutions, find smart ways to fix issues in less time, make the software code base as maintainable as possible, etc. For sure, finding smart solutions require more use of your brain than your keyboard or mouse. That's my point.
Non-graphical text editor such as Nano, Emacs and Vi have been developed in the 70's. That was before the trackballs and mouse became popular, so at this time all actions had to be done with only the keyboard and, since, this non-mouse philosophy has been kept so that even today, Emacs and Vi doesn't require a mouse, **at all**. And this is a good thing !

Think about it. How many time goes your hand from the keyboard to the mouse or trackpad in one day? 1000 times? Each time you get your hands off the keyboard and put it on your mouse of keyboard you need to focus on where your pointer is and then, when finished, you still need to put each hands on your keyboard. Those action probably takes half a second each. So, lets say, it takes a whole second each time you need to use your mouse and get back to your keyboard. It means 1000 seconds per days (16 minutes), 333 minutes per months (5 hours), and 2 days and a half per year spent to get your hands off the keyboard and put them at the right place.

As a programmer, this is a time you should spent using your brain to make a meaningful impact instead of using it to find this *f~cking* pointer on your screen. Learning Emacs means learning dozen of shortcuts to do anything you want like search and replace, moving the cursor to the next line of function, go to a specific line, place the cursor at the end of the file, etc. Learning Emacs will force you to use your keyboard instead of using your mouse/trackpad. After some days, you will find yourself more productive and comfortable with your keyboard. Soon, you won't want to use your mouse anymore and you will force you to learn all the common shortcut of your favorite graphical editor.

## Think twice.

Not convinced about winning 2 days and a half per year? There is much more.

Using recent graphical text editors and IDEs is a good idea. I personally use quite often Atom and PhpStorm. It offers me features such as easy navigation between functions, classes and unit tests, VCS integration, markdown preview, etc. And even if editors like Emacs and Vi can offer you such features, most of the time you'll need to spend countless hours to configure the plugins required. What isn't a good idea, however, is to get your mouse to use all those features. The best example I found to make my point is the *tree view* that most graphical editors provides.

Viewing your file system as a tree on the left side of your code can be an interesting feature as long as you don't know what you're looking for. But, most of the time, people use that tree to open any file of their project. And by *any* I mean, even when they know what they are looking for. So, each time those developers (most of my co-workers) need to see a piece of code located in an another file than the one currently open, they get their mouse, read the tree view, click on the folders, read the file names and click on the file they need. Does it look familiar to you? It mean that even if you used your brain to think about which file contains the piece of code you'd like to see, you still need to read all your tree and find this file although you already know what you're looking for. This is non-sens for me.

Emacs and Vi don't comes with *tree view* tools. Instead, you need to use shortcuts and commands to open a new file or buffer. Most of the time, those editors provide an auto-complete function on file name so that you just have to type a few characters and press *tab*. Anyway, having to type the beginning of the file you'd like to open requires you to think about it and stay focus on what you're looking for instead of being distract by your mouse and your tree view panel. This is a good thing and, again, after a few days using project management tools such as [Projectile](https://github.com/bbatsov/projectile), you won't want to use your tree view panel. (Adding a shortcut to toggle the tree view in Atom was the first thing I do after install)

Once again, think about it. How many time it takes to find a file, navigating trough the tree? Maybe 5 second. Maybe 10. It often depends on if the file is near the one you're currently editing. How many files do you open per day? 10? 20?. Lets say 15. At the end of the day, you passed 2 minutes looking for something you already knows how it's called and where it is. At the end of the year it's 10 hours.

Instead of loosing your time by looking for files you already know were they are, take a break and start learning Emacs.

## Try it, love it

I could write about opening large files such as dump or log that Sublime and Atome aren't able to open without crashing. I could write about memory leaks caused by web-view editors. I could too, write about micro-optimization you can't do with any of those modern editors but may let you incredibly improve your productivity (I often use a rest client plugin for Emacs, for example).

But, the best thing you could do is to try it and you will soon love it.

Emacs and Vi can be used on multiple platforms such as Windows, Mac OS and Linux.

* Find your version on the [Emacs website](https://www.gnu.org/software/emacs/).
* Watch some [EmacsRocks](http://emacsrocks.com/) videos to get started.
* Add some plugins using the [Melpa package manager](https://melpa.org/#/).
* Learn [shortcuts](https://www.shortcutworld.com/en/linux/Emacs_23.2.1.html) to be more productive

And, feel free to clone [my personal configuration](https://github.com/seblegall/emacs-symfony2) for web programming on my Github account.
