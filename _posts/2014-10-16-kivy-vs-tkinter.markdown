---
layout: post
title: Kivy v.s. Tkinter
subtitle: Tinker in Tkinter. Develop in Kivy.
---

While I predict [Kivy](http://kivy.org) will enjoy a meteoric rise in
attention as the world continues to adopt and prefer voice and multi-touch
interfaces over carpel-tunnel-inducing alternatives there are still
plenty of solid reasons to learn at least some of the well-established
Tk framework and the Python tkinter that goes with it &mdash; especially
for rapid data visualization.

[Here's](http://www.techwars.io/fight/kivy/tkinter/) one fun comparison
that does show searches for Kivy are on the rise as does [this
one](http://www.techwars.io/fight/pygame/kivy/) comparing Kivy to Pygame,
upon which Kivy is partially built.

### Tkinter Comes with Python, Kivy Does Not

While the Kivy team has really streamlined the installation process,
you still are required to download Kivy and set it up in addition
to downloading and getting Python to work. With tkinter you get that
for free.

Yep, thanks to ActiveState the Python you download automatically includes
everything you need to use `tkinter` with just an `import tkinter`. This is
phenomenally good for students, scientists and everyone else that want
something quick and easy to use for games and other visualizations. It also
means that you can save your Python code to GitHub or send it in email as
text and have others run it simply by downloading and installing Python,
a two or three click operation. There is no compilation or special extra
steps required, which is what Kivy, Pygame and others require.

### Both are Easy, About Same Docs

They both take about the same amount of time to learn and understand. Both
have great books out about them and both face some documentation
challenges.

The plethora of old/bad documentation for tkinter
makes it a little hard to know where to start. [Modern
Tkinter](http://www.amazon.com/Modern-Tkinter-Busy-Python-Developers-ebook/dp/B0071QDNLO)
is as good a place to start as any since Mark emphasizes
`ttk`, the new and improved widgets library. Plus you have the
extra burden of translating a lot of documentation (like that at
[tkdocs](http://tkdocs.com)) into Python since Tk/TCL was written with
many dynamic language implementations in mind. This is a good and bad
thing. It means you can transfer that knowledge to other languages
but also means you have to wade through more words to get you to your
finish line.

Kivy suffers from being so new, well at least new to those adopting it,
that finding any documentation is still challenging.

### Both Support Python 3

Kivy still has something to work out on the Mac as of this writing, but
Python 3 is otherwise supported by both.

### Don't forget ttk!

You really have to just add one line:

```python
from tkinter import tkk
```

This gets you all the new and improved widgets.


### Under the Hood(s)

Kivy has a cool and rather complicated engine that will make the
best of what it finds, OpenGL, DirectX, or fall backs. I understand
it is also partially built on Pygame although you can't use the
Pygame elements directly. This means that Kivy, like Pygame, is
leveraging the wildly popular and standard [Simple DirectMedia Layer
(SDL2)](https://www.libsdl.org/) for it's rendering. This very important
as SDL2 emerges the apparent leader in cross-platform graphic development
libraries. It also means that if you need extra power later you can
leverage SDL directly.

The tkinter module is built atop Tk/TCL of course, which was created to be
built upon by other dynamic languages, and depends on the specific
implementation for the operating system it is on. While it is possible to
use the native widgets of the operating system it is running on, it is not
always obvious. This has given Tk something of a bad name in the land of GUI
apps, but you can see it reliably in any movie where a fictional or
scientific application has quickly been created to chart tornadoes or
aliens.

In other words, when you want a really 'baked' application go through the
slight bit of extra work to do it in Kivy. When you want a very quick
visualization or GUI app maybe you just need tkinter. Tinker in tkinter.
Develop in Kivy.

### Kivy Can 3D, Tkinter Can't

If you visualizations or games might one day be better in 3D then maybe
start with Kivy first.

### Kivy Can Multi-Touch, Tkinter Can't

Kivy was built by the Python multi-touch team. Tkinter was conceived long
before multi-touch was a glint in someone's eye.

### What about the web?

Building canvas-style visualizations and games is certainly quickly doable
on the web &mdash; especially with tools like [phaser.io](http://phaser.io)
but very often you want an app that doesn't require a web browser or will be
running on hardware directly, such as robotics. There are a lot of problems
that have already been solved with Python modules as well that need
a visualization layer. In these cases it makes more sense to use
a Python-based approach such as Kivy or tkinter.

### Why not JavaScript?

Everyone should learn JavaScript. Everyone. It is the most important,
most ubiquitous, and fastest growing language currently. JavaScript is
executed billions of times a day in places that include not just the
web anymore. But JavaScript still falls behind Python for significant
applications &mdash; especially those involving numeric and scientific
computation and visualization.

WebGL and HTML5 canvas certainly have raised JavaScript closer to the ranks
of Python for numerical analysis and science in general. But as of today
Python pretty clearly dominates in this realm being the darling of the
scientific and number-crunching set for rapid applications where visualizing
the data quickly is the most important requirement over how attractive the
interface itself is.

### Why not Java?

Java is just too heavy for most small to mid-sized applications. There are
plenty of reasons to use it &mdash; and it is the next language after Python
and JavaScript that we learn at &mdash; [SkilStak](http://skilstak.com) but
if you are comparing Kivy and tkinter you have already decided to stick with
a faster, lighter language.
