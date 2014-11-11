---
layout: post
title: Python for Platform, Node for Network
subtitle: Picking the Right Tool for the Job
---

Python's core strengths are for platform engineering particularly large
applications. Node.js shines for network-centric components.

I'm gonna take flack over this from the seasoned developers out there
but if that moniker describes you consider how you would explain these
two languages to someone who had never heard of them and specifically
how to use each and for what. Here is a summary of how I've observed
how these languages are generally used.

An Example
==========
At SkilStak Coding Arts this week we welcome the birth of two new baby Lego
Mindstorm EV3s and a bunch of Raspberry Pis to keep them company. While
we researched all the fun things we can code and learn with them, which
is just astounding, we uncovered dozens of ways to make them do what
you want in about every major programming language that exists, even
Bash scripts. This begs the question, "What language should we program
them in?"

Python for Platform
===================
I see the title **Platform Engineer** pop up a lot in casual perusing of
job postings these days (to keep up on what companies are looking for
so we can teach relevant stuff). Turns out this is just another way of
saying uber-coder-who-loves-backend-systems-development. These guys and
gals spend their days immersed in complicated software with thousands
of lines of code, test suites, data analysis, etc. Python is likely the
lightest of the languages they get to use. More often everything is in
Java, C, C# or some other enterprise-ish language.

Python for platform engineering and other large-scale systems development
seems solidly and prolifically used in that space and has been for years.
I remember one rather large corporate Intranet search engine offering in
the 90s that cost thousands and was entirely in Python, not Java. In fact,
more and more you see Python replacing and supplementing Java &mdash;
especially in the enterprise space. Having done a lot more Python in the
last four years I must confess I wish I had been able to use Python 3
for the massive enterprise applications I got to build while at IBM. I
used Perl and Ruby instead. (Don't even ask about my experience trying
to do them in PHP at first to be a 'team player', that memory-leaking,
not-a-language, developer-team-in-fighting, piece of filth.)

Python is also the darling among scientists and number crunchers for
many reasons but I can't help thinking this is mostly because it can be
extended so easily in C and embedded into so much, like Lua. It has so
many data visualization options that anytime you see a legitimate movie
with science-types charting Tornadoes or staring at mass-spectrometers
you are likely looking at a Python program running on Linux.

While Django, Pyramid/Pylons, Flask and the rest have been major players
in the web framework space for years (and still are) I submit they are
not Python's major domain or strength. For one, it wasn't until recently
that they supported Python3. Many of them still don't support asyncio,
which seems like Python playing catch-up after the popularity of nginx
and node took off (for good reason). Python web development still,
for the most part, seems to have the WSGI cruft as well. A lot of create
sites web sites and apps run on Python, but I suggest a strong look at Node
for anything network related.

Node for Network
================
Node was built with the network in mind &mdash; and not just the
web. At the core it uses the same model the wildly popular nginx does,
an asynchronous, event-driven, low-ram-using powerhouse. But even more
significantly it empowers developers to largely do away with the bulk and
cruft of other web components, such as the server itself in many cases. In
fact, with additions like Koa you have access to the efficiency and power
of low level network operations allowing you to create protocols below
HTTP in the same way. These powerful advances have got Python playing
catch-up in a big way. Python has bolted on `asyncio` but it wasn't built
around an optimized engine that used it from the start.

Node is also in JavaScript so connecting it the front-end just feels
less hack-ish. Node was born to talk to front ends and other network
components.

Node can be used for platform engineering, but it has a long way to go to
catch up with Python in that space. Most notably Node lacks the same level
of maturity that Python does in the enterprise space. There are fewer test
suites and a few major flaws, such as the NPM naming issue. Relatively
speaking, very few enterprise architects or scientists would trust Node as
their core development language currently and probably for good reason.
Last year Walmart uncovered a subtle but important memory leak in the
Node core. It was corrected and pushed the language further along in
enterprise adoption, but it's important to remember just how new Node
is. Sometimes old is better.

Right Tool
==========
So as CTO of this enterprise of one here at SkilStak I've decided our
architecture will use generally use Python for platform and Node for
network. In terms of our little EV3s this means when we ssh into our
EV's brains we code Python and Bash scripts in them so they remember
them even when off the network, but when we want to control them over
WIFI or Bluetooth we use Node to handle the protocol connections and
such. 

Will we still learn network programming in Python? Absolutely, probably
by creating a `tkinter` app to control the robots first, then a `kivy`
app later to do the same. Kivy quickly gives students a beautiful app
they can run on any device to control their robot locally over the
network once they have written the network protocol code to talk to it,
which is a huge learning opportunity I can't wait to introduce.

We will use Node to create SPAs that are accessible from anyplace on the
Internet by anyone perhaps even giving them a playground that is on a web
cam so others can 'drive' them from home. Node let's us both handle the
webapp commands and connect easily to the EVs over the network.
