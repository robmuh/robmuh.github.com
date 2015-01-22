---
layout: post
title: No One Uses Python IDLE
subtitle: so stop using it to teach Python
---

Professional Python developers use anything but IDLE so why should
*anyone* else. "It runs on Windows" and "it does function completion"
are no longer sufficient to convince me since no professional cares
about these things. Tkinter graphics isn't even a reason since it
does not require Python to be edited in IDLE. Don't teach or learn
Python on Windows. Learn it on a Bash command line like the pros
use or, if you must, use a *real* editor.

## But everybody's doing it (in education)

This is another forehead-slapping moment for me. For some reason I
keep discovering things that I adopted when teaching that some how
I felt I had to do to be in step with others teaching the same
things. Python IDLE is one of those things. It comes with Python.
It is on the desktop on Raspberry Pi. It supports graphics. Yep,
at first it seems to be the right thing to use.

It's not.

In the many years I have been programming, even before I was coding
Python in my Perl days, I have never once seen Python IDLE used in
any professional way. Yet for some reason I felt I had to use it
to teach kids programming. Wrong.

Python IDLE falls into the 'unnecessarily babying them' category
along with the nano editor, which I'll rant about in a separate
blog post. 

## "What if they are not ready to use an editor?"

Then they shouldn't be using IDLE either. This is what
[code.org](http://code.org) and [codecombat.com](http://codecombat.com)
are for.

## "But it has Tkinter graphics"

No it doesn't. Python for Windows comes with it. IDLE doesn't provide
it.  Tkinter is largely a useless interface to teach (no anti-aliasing,
no GPU acceleration, etc.) but if you choose to spend any time
teaching or learning it you still don't need IDLE. You can use vim,
Notepad++, Sublime, Atom, Brackets, even Eclipse if you are that
much of a masochist. You don't lose Tk just for not using IDLE.

## You don't have time to waste

Educators that teach students using Python IDLE are actually slowing
them down.  The pace of technology advance parallels the pace of
just-in-time learning required to keep up with that pace. Those who
learn Python using IDLE develop work patterns that have to be
overcome later. IDLE promotes a two window development work style
with the coder switching between code and the shell windows. Yes
you can run the code from F5 once you configure auto save but if
the code has any kind of input prompt the coder will have to switch
to the shell to enter it. This is not intuitive for young programmers
who often end up in the wrong window slightly confused largely because the
windows look the same. No amount of it-looks-like-a-rattle-snake-rattle
mnemonic devices seem to overcome it.

Another issue is when students double-click on their Python program and it
runs and ends. They have to be trained to right click it and open it with
another editor. This double-clicking to run is actually a more useful
workflow to teach because it reinforces how their code could actually be
used on their computer. A better workflow to teach is to have the code open
in a real editor of some kind, and another window with either the file
explorer or a true shell, even Windows, where they run the program.

At first it seems like having IDLE up is more efficient during development
than saving and rerunning it but if anything it is as efficient while
emphasizing the way code will actually be used. Which reminds me &hellip;

## Python IDLE has no support for ANSI terminal colors

Never underestimate the power of terminal color. Ever watch a kid
spend an hour obsessed with crafting a Minecraft MOTD just so it
has color? I have seen dramatic changes in interest from students
just from a solarized Linux terminal running syntax-highlighted
vim. Somehow it makes programming orders of magnitude more fun and
most professionals agree. Python IDLE doesn't have it. Sure you can
change your colors and such but you cannot produce amazing text
adventures that output ANSI color that you can see.  What's worse
the IDLE shell trying to apply Python syntax highlighting to your
text adventure with creative ASCII art making the whole thing look
like crap. Using Python from Bash almost always &mdash; even on
Windows &mdash; ensures you will have color possibilities that will
tantalize coders to create amazing uses for them &mdash; in text.

## Might as well change operating systems while you are at it

Once you throw out IDLE and Python for graphics you have nothing
stopping you from using Bash command line for all your Python
development, which reinforces more essential technical skill in the
process. Moving all our coding that does not focus on native front-end
app development or games to a centralized Linux server has been the
best decision we have made as a school. Every second is more relevant,
more meaningful, and for the right-type of student, more fun.

## "Not everyone likes the command line"

Well they should. The command line is where real work gets done.
It is the reason Mac is the goto choice for most developers. IDLE
is not. I have observed over and over again that students not only
step-up to the challenge of command line, they *love* it, even
prefer it once they have learned the basics. Personally I think it
is parents and teachers that are more scared of it than they are.
