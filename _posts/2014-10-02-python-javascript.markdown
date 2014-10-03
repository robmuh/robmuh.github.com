---
layout: post
title: Porting Code.org JavaScript to Python
subtitle: One way to expand studio.code.org into written Python code
---

The activities at [studio.code.org](http://studio.code.org) do an amazing
job introducing computational thinking, algorithms and the rest to coders
as young as four. But what do you do when you are done with them? Port
them from JavaScript to Python of course.

Some of my students and I at [SkilStak](http://skilstak.com) were working
through some of the 'Artist' activities clicking on 'Show Code' as usual
when it occurred to me the JavaScript code for these is nearly 
identical to the Python turtle module. Turtle approaches to
teaching programming have been around almost as long as programming so
it wasn't that surprising.

"Let's port that," I said. So we fired up Python, which we normally use
for Battleship, BridgeKeeper, Magic8Ball and all our other raw Python
coding in class, but so far not a lot of graphics. After a `from turtle
import Turtle` and a `muddy = Turtle()` we could make muddy do all sorts
of equivalent things using inspired from the ported JavaScript code, which
some would even include in the Python code at the top in a long comment.

As for using the `turtle` module I decided to keep things Pythonic instead
of using the uglier `from turtle import *` which almost every single book
and tutorial uses even though it is just plain 'ol bad practice. A few
lines later we had spirograph (an old reference I know) stuff happening
on our screens and the class was deeply engaged in making their creations
all the better, including writing their own `random_color()` (with proper
American spelling of 'color'):

```
from random import random
def random_color():
    return (random(),random(),random())
```

*I could not contain my excitement.*

This porting activity addressed so many things that I still felt were
missing and even made me shy away from things like
[Scratch](http://robmuh.com/scratch-misses-itch) and even turtle
graphics programming in general. Since GameMaker, for example, is also
very graphical and can be used to make actual games eventually more
capably that just pure Python.

Here's the major reasons, (which maybe I'll elaborate on later):

* **Really** writing code, not just dragging blocks around
* Getting exposure to two essential languages at once (Python,
  JavaScript)
* Maintaining their 'green dot' work by committing to GitHub
* Integrates on-the-web and on-the-desktop coding activities
* Launch point into graphics programming starting with Python `turtle`

The overwhelming evidence from my personal experience with this students
is that they *love* Python graphics programming and want to do a lot
more of it. Reminded me of when I wrote a basic missile-command game in
Basic on the Atari after doing a simpler DnD character generator in text
before.

### From Blockly to Kivy, A Solid Learning Path

The best part of all is that there is now a solid educational path
from moving blocks around with Blockly ultimately to cross-platform
applications development with Kivy or even SDL2. It looks something
like this:

1. Introduce Blockly through studio.code.org (also Scratch/Snap!)
1. Port JavaScript from studio.code.org to Python `turtle`
1. Expand and play with Python `turtle`
1. Expanding from `turtle` to `tkinter` (on which `turtle` is built)
1. Supplement with Python Image Processing Library
1. Introduce PyGame (built on industry SDL standard)
1. Expand from PyGame to Kivy (partially built on PyGame and SDL)
1. Expand from PyGame to raw Python SDL development 
1. Expand from Python SDL to raw C++ SDL development

I haven't figured out a good way to introduce Java programming in this
progressive path. So far we just do that separately after they have
completed the `tkinter` stuff and other non-graphic lessons involving
traditional object-oriented programming (primarily Battleship).

I'm also looking at adding the ProcessingJS stuff from KhanAcademy the
the can-be-ported-to-python activities.

### Working with the studio.code.org contributors

The more porting we have been doing in classes the more I realized with
a little structure and organization this code could really help others
wanting to offer more to students after completing studio.code.org
activities. I played around with how to organize everything and
remembered that all of code for studio.code.org is available on
[github.com/code-dot-org](http://github.com/code-dot.org). Around that
time I also wondered how to add port activities for the Maze and Farmer
sections that don't directly map to Artist/Turtle stuff.  I thought we
could easily add something to make them also port directly. Something
as simple as what to name such a Python library was not immediately
obvious. So I decided to ask.

I found the studio.code.org team in their chat room a met them a little
in their chat room the other day. They were overwhelming supportive of
the idea and full of encouragement. We arrived on the name
`codestudio` for the Python module and decided to have it model pretty
closely the actual activities from the site, including references like
`s1level1`. This way a simple one line import can setup whatever
activity even if all it is doing is mapping snake-case versions of the
same JavaScript functions to their `turtle` equivalents. The goal
seems to be to have everything simplified in one import line:

```
from codestudio import Artist
```

Or even more simply when referring directly to an activity:

``` 
from codestudio.s1level2 import *
```

And yes I do not like using `*` here but this is the easiest way to
maintain the procedural feel of the initial studio.code.org
activities until they are introduced to OO concepts gradually later.

### No code checking

Initially the objects moving and interacting on the grid will be the
success criteria with timeouts and such modeled after the same in the
JavaScript code base. So no direct syntax checking or 'lines of code'
counting for now.

### More later ...

Still a lot to do here, but the immediate benefit is that SkilStak
(and everyone else hopefully) will get a framework to easily and
directly take studio.code.org activities directly into running Python
environments (assuming schools get over the hurdle of allowing Python
to be installed on their computers).
