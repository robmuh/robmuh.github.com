---
layout: post
title: GitHub Python Module Project Organization
subtitle: Have your cruft and eat it too, wait, what?
---

It's not rocket science, but some of you might still not know to just
make a `yourmod-project` repo and a `yourmod` repo and just make the
second a submodule of the first.

One of the long standing debates in the packaging world is just how much
packaging to put around the actual stuff you are packaging. On the one side
you have those that may believe in testing but hate burying their working,
useful code in a heavy package making it almost possible to find. On the
other you have those that not only bury their working code but have
generators, macros and so much cruft that you can't actually see what the
code does or even looks like in source form without some level of build
staging or compilation.

I'm happy to share one method that I recently stumbled upon having caught
up on the PyPA stuff. Last time I got into Python packaging distutils2
was still the apparent direction, which has since been denied by the
powers that be. But I digress &hellip;

### Just Make a Submodule, Duh

This is gonna sound ridiculously obvious to a lot of you out there, but it
is worth sharing for the others:

`
cd codestudio-project;
git submodule add git@github.com:skilstak/codestudio.git
`

That was all it took to separate what can otherwise be cloned simply
as a directory (and therefore Python module) from all the unit testing,
distro stuff, docs and extra stuff that a user of the module would likely
not care about. The result looks like
[this](http://github.com/skilstak/codestudio-project).
