---
layout: post
title: Learn Python and Java on the Desktop, JavaScript in the Browser
---

JavaScript, Java, and Python top the list of first real programming
languages. As expected there are many sites for learning JavaScript
within a web browser and there are few for learning real Java, a heavier,
compiled language usually requiring Eclipse or IntelliJ. Python, however,
suffers from a schism of sorts between those that try to invent ways of
running Python in the web browser using JavaScript (think codeacademy.com
and Skulpt) and those that run Python on the server and send the
results back to the web browser (think groklearning.com, checkio.org,
sphere-research.com). It's no surprise that learning JavaScript in the
browser and Python and Java on the desktop works out best in the long
run for education.

Note to the established developers: yes I'm over-generalizing and
simplifying a bit to make this easier to grok for others.

Comparing programming languages is holy ground for many but running a
school that teaches programming requires it. 

### JavaScript

JavaScript is fundamental. You are almost required to learn it these
days, which is quite a change from the 90s. JavaScript is executed in
just about every web page you view. Node has brought JavaScript solidly
into the back end domain of other languages such as Java, Python,
and Perl. Because of this (and JavaScript's event-model paradigm) it
has gained the attention of the brightest minds on Earth working to
optimize the V8 engine that runs it. A solid well-funded community has
formed around it. It is the language taught by code.org and KhanAcademy
in a creative, graphics-centric way. 

### Java

Java, not to be confused with JavaScript of course, is another big
language used in education and for good reason, it's ubiquity outweighs
it's warts as the first *heavy* language you should learn, but not as a
first language. It is currently the language of the AP Computer Science
exam and the main secondary language taught at MIT (after Python). Java
is the *only* language most new students know by name when they enroll
at SkilStak because of Minecraft. Writing anything to do with Minecraft
(mods, plugins) involves Java. There are also a lot of other fun options
when learning Java such as Robocode and Battlecode. These days Java is
rarely found in the web browser. Java is also a traditional, strict
object-oriented language which makes Python a great introduction to
eventually learning and coding in Java as well.

### Python

Python has surfaced as the winner of a decade-long battle for prominence
on the server-side or 'back end' domain as a *scripting* language. It
appears ultimately 'one best way' has won over 'more than one way'
which differentiated Python's roots as a language developed by an
engineer (who now works at Google) from those of Perl developed by
a linguist.

During it's long life several Python engines have been created to
accomplish different things, all with their own subtle (and sometimes
annoying) differences. Among these are the 'in browser' Python interpreter
engines that weigh up to 300KB, don't support much of anything you
would actually use Python for, and when they do support graphics and
such use a completely different implementation than every other Python
interpreter. This is important to those teaching Python out there
because it means that things like `turtle` and `tkinter` just are not
available despite the very clever replacements for them in JavaScript
implementations. At first everything seems amazing, then you start to
slowly hit the bugs and limitations of that implementation and wish you
had just stuck with Python on the desktop and server-side.

### In-Browser Python Suffers from No Support

Anything designed to run Python in the browser will always remain
an educator's toy. Python is *never* run in the browser to do any real
work, which explains why the engines created to allow Python to run in
a browser will never enjoy the support of a real community.

A good example of this is codeacademy.com, an otherwise great way to
learn HTML, CSS and the like, but don't learn Python there. Kids get so
sad when I tell them they have bugs in their Python 3 code in class after
diligently using codecademy to learn Python 2.7. I actually discourage
anyone from learning Python there. Thankfully there are alternatives.

By the way, a little sleuthing in the open source repos reveals that the
author of the Emscripten-compiled, in-browser, version of Python used at
codecademy moved to Facebook some years back and codecademy hasn't done
anything new with Python since, perhaps just a coincidence, but if not,
then a great example of why no one learning or teaching should invest
heavily in any in-browser Python implementation for their material.

### But what about graphics?

I had to be reminded that kids really, really, really love visual feedback
during their programming. While we have a great time creating text-only
games in Python things like the amazing studio.code.org mesmerized these
guys to the point of almost of being catatonic while working on them.
Naturally that meant adding more visual interest to their
learning-to-code work.

The greatest discovery at SkilStak in the last two months was having
students port their JavaScript stuff from studio.code.org to the Python
they know and love running in IDLE on their desktops thanks to the
brilliance of those who decided to put `turtle` and `tkinter` into
every distribution of Python. This single fact makes the conversion
from JavaScript graphics in studio.code.org to IDLE a breeze. When
students take what they know and love and actually type in the Python
equivalent they seem overwhelmed with accomplishment.

Khan Academy is another JavaScript-based place to learn programming
and uses ProcessingJS library, an amazing tool for making all sorts of
creative visual stuff, but Processing is technically it's own language
even though it looks a lot like Java. Moving from Processing, which is
more of a language than an API, to Java makes some sense, but not really
to Python. There is the `pyprocessing` project and some other Skulpt-based
processing ports but they fizzle out and suffer from lack of support.

However, Python's Kivy contains a lot of similarities to Processing
and is also a darling of the graphics arts world boasting full
multi-touch and cross-platform support, which Processing currently
does not have. In other words, perhaps a KhanAcademy-to-Kivy path
could work, but the studio.code.org -> turtle -> tkinter -> PyGame ->
Kivy seems a smoother path.

### So no web sites for learning Python?

I didn't say that. Sites like the amazing
[groklearning.com](http://groklearning.com) and [checkio.org](checkio.org)
have streamlined the client-server-client Python code pipeline so much it
is almost undetectable that it is not real-time.  They have even managed
to deal with `while True:` attempts to break their servers. To me these
are the next best ways to learning Python from actually using IDLE or
the command line itself. (I try to forget other heaver IDEs for Python
development actually exist.)
