---
layout: post
title: Teach Kivy Before Processing?
subtitle: Yes.
---

Recently I've had to choose which method of graphics programming to
teach first at [SkilStak Coding Arts](http://skilstak.com). I've
narrowed it down to [Kivy](http://kivy.org) and
[Processing](http://processing.org). Processing is a visualization
language targeted mostly at artists with a great JavaScript port and
is used by [khanacademy.com](http://khanacademy.com) to teach programming
but suffers from lack of cross-platform support and multi-touch
functions. Kivy is Python with its own markup and full cross-platform,
multi-touch support for apps on all devices but isn't really as accessible
to beginners. Both are darlings of the creative world. The question
for a lot of folks teaching programming is, "Which one should I teach
first?" I've decided on Kivy. Here's why.

### Kivy has More General Usefulness

Kivy was conceived to make amazing, cross-platform, high-performing,
multi-touch apps on any mobile device or computer.  Processing
was specifically targeted at artists and those focusing on data
visualization. While this makes Processing particular good at being a
'digital sketchbook' for artists, this specialization limits its scope
&mdash; especially to the broad interests of students here. If I were
just teaching art I might have chosen Processing instead.

### Kivy is More Open

Kivy does have its own optional widget markup language to accompany the
Python, but at its core it is Python. Processing is its own language at
its core and although it looks like Java it isn't.  ProcessingJS has
created more openness for this but is not supported anywhere but in a
web browser. Kivy's Python and markup are supported on all devices even
if they cannot be run from within the browser. At this stage at which
students are introduced to this level of graphics programming we have
already departed from the web browser and therefore Kivy fits better.
Web development is obviously very important, but it is a specialized
branch to be added after the core trunk of programming skills has been
achieved.

### Multi-touch is King

I personally feel the move to mobile-centric apps will eventually favor
frameworks that specifically target cross-platform, multi-touch, native
apps, which is exactly what Kivy is. Eventually front-end alternatives
using web technology (like PhoneGap) will give way to the raw power of
native apps. This is the fundamental reason Facebook, for example, stopped
using a PhoneGap-ish version of its mobile messenger and went native.

One of the main reasons to go native is multi-touch. As touch continues to
displaces the mouse as the preferred interface frameworks and apps that
support it natively will grow in adoption. Multi-touch is Kivy's great
strength. Kivy was conceived and written by the Python core multi-touch
team. They live for multi-touch above everything else.

Teaching kids Kivy prepares them well for the device-centric, multi-touch
world they live in now and to come. This is a core requirement as
important &mdash; if not slightly more so &mdash; than web development.

### Kivy Fits the Education Path Better

Everyone here starts on studio.code.org. Then they port the JavaScript
from 'Show Code' to Python's `turtle` module, which in turn leads to
`tkinter` broader graphic possibilities and then to `pygame` and
ultimately to Kivy, which is built partially on `pygame`. This
progression feels natural where it matters most: the transition from
dragging blocks to typing code. Python has a more forgiving and
understandable syntax than JavaScript for this yet the students are
exposed to a little JavaScript syntax as well in the process &mdash;
particularly loops, functions and such.

Python provides quite a bit of graphics programming possibilities included
in every Python installation with `turtle` and `tkinter`. When we reach
the `pygame` point in the learning curve we have to start installing
extra stuff. At that point, however, students should be very well
versed in programming and ready to learn how to integrate other tools
and libraries. Installing Kivy is within easy reach after that. These
steps also include important branch points for introducing deeper game
and OpenGL development with SDL2 and Pyglet.

The path using Processing does not enjoy the same granularity in
steps. The steps filled by Python `turtle` and `tkinter` are absent. You
go from coding in the browser, to having to download and install the
Processing app and using that, which no longer uses the JavaScript used
in Khan Academy but the Processing language, which claims to be a subset
of Java, but for educational purposes could confuse students when they
do actually do Java. It is neither the JavaScript they learned at Khan
Academy nor Java. This puts Processing in the GameMaker Studio category,
useful and great, but specialized and secondary. Those highly creative
students can always add on Processing starting with Khan Academy along
with the other material.

### What About GameMaker Studio?

We do use the propietary GameMaker Studio but it has taken a secondary
place much like Unity3D. Learning GML is no longer in the main path here
but is still very valid for students with specific projects to make 2D
games. This is because GameMaker Studio is a real tool used by real game
developers to publish games. But while GameMaker is great for creating
games it is horrible for making any other type of mobile apps &mdash;
particularly those involving multi-touch (which was the very reason we
purchased multi-touch laptops at the school that GameMaker Studio does
not support, Kivy does).

### Kivy Tops the Trunk Before Branching Out

Part of building a curriculum has involved deciding what is a core part
of the main trunk and what is a specialization branch. At SkilStak Kivy
is the last thing everyone learns before branching out growing into
their preferred specialization (front-end development, 2D and 3D game
development, system administration, Java development, data visualization
art, etc.)
