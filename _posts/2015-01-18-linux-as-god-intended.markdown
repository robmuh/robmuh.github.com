---
layout: post
title: Linux as God Intended
subtitle: for multiple users
---

Linux came from Unix which came from a need for powerful, collaborative,
platform for hundreds, even thousands of individual users and nothing
but a text terminal interface. Guess what, it still excels at it
and it is exactly what any nano-school needs.

I [ranted hard](http://robs.io/use-linux) for using Linux over
windows and even Mac but I've changed my mind on some things based on
observations that have changed some of my core thinking about teaching
programming primarily to kids, some as young as seven.

## Once again I recommend Macs to anyone that asks

I wrote a [page about why](http://robs.io/buyers-guide). I also
have one on my desktop, again. It seems like a fickle phase with
me between that and Linux. I have a Linux laptop and an iMac Desktop
workstation.

## How young is too young for Linux and vim on a terminal? 

Age is irrelevant. I have 10-year-olds busting out code in vim from
a Solarized [Putty Tray](https://puttytray.goeswhere.com/) and
loving every second of it. My nano-school wall now has a 12 foot
mural of vim shortcuts. If they can type like they do on
the Minecraft terminal then they are ready for Linux, even vim. 

[By the way I ripped nano off our server after finally concluding
all you need are three main commands in vim to be just as easy:
Esc, 'i', and 'ZZ'. This is because insert mode supports all the
arrow navigation the youngest coder would find intuitive. Plus I
have vim so customized they see clearly where they are, what line
they are on and more.]

## Linux + Putty Tray + WinSCP = Light-Weight Coding Bliss

A lot of my students get really bored at home or at their main
school, public or private. Creating a set of tools that are just
customized copies of [Putty Tray](https://puttytray.goeswhere.com/)
(for ssh terminal access) and [WinSCP](http://winscp.net/eng/index.php)
(for drop-dead easy file transfers) and putting them on a USB stick
means they have nearly instant access to all their SkilStak work
from anywhere, anytime. This escape into coding at SkilStak is just
the type of disruptive subversion I absolutely love. Kids learning
despite the school system.

As great as *Desktop on a Stick* and *Server on a Stick* have been
they are too big for this sort of instant access. They are ideal
for full Linux training in which case we are breaking the system
or reconfiguring it in ways that would need to be snapped back.

## Better Storage and Backup

GitHub has corrupted a few GameMaker games when students get confused
and get locked in a merge conflict &mdash; particularly because
GameMaker uses text XML files. Plus GitHub saves of GameMaker or
any code are automatically public and not all students want their
work public (I know they could get private repos for free, but it's
a hassle.)

Unity games are usually so large they can't even be stored on
GameMaker.

## Collaboration

Students at SkilStak have used Minecraft somewhat to get that sense
of community even though only 4-8 or them are ever at the school
at the same time. Logging into a multi-user Linux school server is
proving to accomplish that same thing. I've renamed 'finger' to
'poke' and encouraged them to use Mutt mail, .project and .plan
files and all the other 1970s Unix goodness. It's almost like a
game itself and they love it, all of them.

## Code Review

Not only can I log into the server and help anyone stuck on a coding
problem but so can *every other student*. This is huge. No fancy
need to post to Gist or Github or Reddit or, god-forbid, some sort
of bulky LMS. Instant feedback from peers and friends on the same
system they are using to run the code. You just cannot beat that.

I can even automate calculation of when each student was on the
server, even how many lines of code they wrote and give them SkilBux
based on their activity with much more precision than would ever
be possible writing some complicated interface to the GitHub API.

I can even automate git commits for those young kids that want them,
but they really don't need them. Everything is backed up in .snap
daily and onto other disks regularly as well. Git is now command
line, also as God intended. No more building dependency on GitHub's
pretty little windows GUI that may or may not work on any given
day. I've simplified the git commit steps with a 'save' alias. Now four
little letters make these kids joyful for how much simpler everything is,
and yes I'm still talking about the command-line.

## The Future is on the Command Line

I've recently read more than one futurist predict more and more
developers will move to the command line for its raw power &mdash;
especially as it becomes more approachable and the standard for
packaged software installation. I agree with these predications and
getting students comfortable with the command-line is fundamental
from a very early age. Minecraft has eased this wonderfully for
those that have the real version and have learned to type and use
the Minecraft command line, which is modeled in part after the Linux
command line.

## Why aren't more doing this?

Some please explain to me why other schools are not introducing
Linux command-line skills earlier to students? It seems everyone
learns them in college but that is far too late. I suppose the main
reason is schools do not have the know-how and human resources to
dedicate to such a thing, or do they? This seems like a great thing
for the Instructional Technologist and media people to setup, but
then again, they are dealing with teachers who can't use the command
line themselves *sigh*. Never mind. I answered my own question.
