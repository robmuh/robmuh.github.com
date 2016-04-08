---
layout: post
title: Bower, Yet Another Unnecessary Package Manager
---

Bower is a well-intentioned waste of time and distraction from the real
challenges of package management. Plus it promotes bad web app development
practices. Let's focus on meeting web app challenges with NPM instead. 

I haven't been using bower for long, but after streamlining my web app
and library workflow recently I realized what a fat waste of energy it
is. The biggest reason NOT to use bower is that you have to manage two
package managers in your project. This is just stupid.

Then I actually submitted my first simple package to both systems. Why?
Honestly at this point I don't know. Maybe because I wanted to see it work
for the first time. I wish I had not registered to bower and that is the
last time I will. I'd encourage you also to not use bower and focus
your energy in getting a kick-ass library or app into NPM instead.

If you are not using grunt or gulp to build your web app --- including
unit testing, compression, vendor prefix adds, jshint, automatic
versioning, etc. --- then you are doing it wrong. I certainly am not going
to encourage you by making my shit available to you in bower form. Hell,
you will probably just move it out of the horribly named bower_components
as soon as you get it and stuff it statically in your `src` when you do
finally get a clue and start building properly using `gulp` (or `grunt`).
At that point the whole reason for package management will have been
defeated. No, it is better for all of us for you to get into the habit
of linking in or dynamically sourcing from `node_modules` where it
safely lives and can be updated properly.


### But bower isn't directly linked to any 


* Bower fractures the package management issue diverting resources
* Bower is fundamentally dependent on node and git (and github)
* We already have git-based package management in NPM
* Bower is broken
* NPM has a robust, official company associated with it, with support
* Bower is failing
* Good web app creation means consolidating and compressing
* NPM needs our help
