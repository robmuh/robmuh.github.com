---
layout: post
title: Jade, Stylus, and PrePros
subtitle: An Easier Way to Learn Web Development
---

It may seem backward, but teaching [Jade](http://jade-lang.com) and
[Stylus](http://learnboost.github.io/stylus/) before teaching HTML and
CSS is a natural compliment to learning Python as a first language and
actually easier for students to grok. The instant gratification and
smooth interface of [PrePros](http://prepros.io) make any student want
to write the code to make the magic transitions happen before their eyes.

# Simple is Easier to Learn

The same reason that Python makes such a great first programming language
Jade and Stylus make focusing on the concept and tags much easier &mdash;
particularly for young students. The significant whitespace cleans the
syntax and teaches good style habits, which you will appreciate if you
have spent any time reading about the philosophy behind code.org and
Blockly. You may have been convinced removing as many distractions from
learning the quirks of typed-syntax to focus on core concepts has value.
Learning Jade and Stylus first carries that same value. Surely it does
not insulate the student from learning proper syntax and being able to
eventually type language constructs correctly, but the initial impression
is gentler. HTML and CSS Syntax is not kind to the very young. Jade and
Stylus follow on this idea and when adding PrePros you can see immediately
the resulting HTML formatted perfectly in the Chrome source inspector.

# Sweet Spot Between Raw and Build Workflow

I used to start teaching HTML and CSS with raw HTML to those just
starting and command-line npm-based boiler-plate for everyone else.
Using a graphic tool like PrePros fits nicely between these two
approaches.

At first editing raw HTML on GitHub seems like a good way to quickly
get students started with web development because it does not require
the extra steps necessary to clone a repo and can be done entirely
from their web browser using the GitHub editor. Once GitHub Pages
picks up their web site saves (commits) are instantly visible giving
them immediate feedback that would take much more setup to accomplish
using a clone, update, commit, push approach. Soon, however, students
and teachers hit the limitations of not being able to include local
images and such that are addressed by doing development locally.
At that point one begins to wonder if it would have been better to
simply start out that way.

On the other hand those doing more involved web development with
Node require setting up a command-line build workflow including
live-reload of some kind. There have been many approaches to
simplifying this including [Yoeman](http://yeoman.io), which I
loathe, to any number of boilerplates for [Grunt](http://gruntjs.com)
and [Gulp](http://gulpjs.com) and finally just plain
[NPM](http://blog.keithcirkel.co.uk/how-to-use-npm-as-a-build-tool/), which
makes so much sense. I even started my [own](http://kwand.io) a few
years back but abandoned it when I realized even the brightest
students have a hard time groking it all.

The great thing about a tool like CodeKit or PrePros is that students
can do their development locally with even more ease than with
GitHub Pages and still maintain that process when they add in a
build workflow such as one based on NPM.

# Blog Without an Engine

The Jade + Stylus + PrePros combo makes creating a blog on GitHub not only
remarkably easy, but very educational. While I haven't converted this blog
from GitHub pages yet it is just a matter of time. This combination allows
immediate previewing of blog posts and other web pages and a simple `git
commit` and `git push` posts the final version without any dependency on
GitHub pages or any other blogging engine for that matter. Blogging can be
a great way to promote web development skills using these industry
standard preprocessor formats and fosters less dependence on any particular
blogging system.
