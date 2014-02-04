---
layout: post
title: The Static Web Returns
subtitle: All of this has happened before and it is happening again
---

The '90s standard of static web content is returning and for good
reason. Mashable services covering every dynamic component a web site
could ever really want have combined with the absolute client-side power
of HTML5, CSS3, and modern Javascript to leave the humble page itself
standing single and static.

### Grunge, brit-rock, alpha JavaScript and the first static web


Nirvana in on the Walkman, laser-discs the size of vinyl albums tied to
our Apple Macintosh IIfx boxes, writing emails in Eudora, searching the
Internet with [Gopher][] or for books [telneting][] to library terminals,
fingering our friends on university BSD machines, aw yes, those were the
days.
![GopherImg][]
I will never forget the day I saw my first web page. I FTPed (or
Gophered) NCSA browser and saw my first HTML of the campus. Then
I opened a page with an image on it that took four minutes to load and
I thought I was going to faint it was so cool. All the possibilities
opened in a way that must have for Thomas Edison when he saw the
first working light bulb. I grabbed random strangers in the university
hallway and said, "You HAVE to see this!"
![Mosaic][]
Those were the days of static web pages. Modems forced an unhealthy
obsession with optimizing web pages. The idea of connecting web
content to anything dynamic was a dream.

Then came CGI, the Common Gateway Interface, and anyone with Perl skills
instantly became a web god --- especially if you could make web pages
render data from flat file databases like Xbase, CSV, and such.

**Get off my lawn!**

OK, I couldn't resist.

Eventually we learned to talk to mostly Oracle databases, if you had
the money to work with one. There was no Open Source database
offering. Having a dynamic site generated from content in a database
was the coolest thing most could imagine. And as for speed, well, it
took so long to even load the content the DB and dynamic latency was
not an issue --- at all.

### The dark ages of bloated Java and PHP frameworks

I have to say I'm rather glad I was doing Linux system administration
and system development and other interesting stuff during the dawn of
dynamic web frameworks. ASP turned my stomach so much I couldn't even look
at it (still does). In fact, it was one major reason I left web
development in general for stuff more deeply buried.

Frameworks, then and now, seemed largely like an unforgivable waste of
resources to me. More and more people wanted to create systems that
required caching database calls and other complex, unnecessary tricks when
just creating a system that organized that data and created static
resources, static pages and files, would have been fine. There were
definitely legitimate uses of server-side dynamics, but everyone
wanted it just because it was cool.

Browsers that were warring and unable to do even consistent things
with JavaScript complicated it. Web developers took refuge in doing
things on the server-side where at least they had a certain degree of
control. Devs would send relatively simple, but commonly supported
HTML and the magic would happen server-side, which meant more dynamic
web page requests on the back end.

The shitty, web-driven language PHP was born around this time. It was
carelessly thrown together and grew with no supervision into a bloated
piece of [crap][] that even the original authors won't claim anymore. I
made the mistake of being a team player and using PHP for a rudimentary
back-end data processing queue only to uncover the horrendous memory-leaks
of a piece of shit conceived and designed to never have to run but a few
seconds in a web server request. I imagine a lot of that is still unfixed
and people refuse to work on it. Yeah, now THERE is a language we should
build our entire web-o-sphere on --- *shakes head* --- which is exactly
what happened with Wordpress, Drupal, Joomla and the rest of the PHP-based
butt-ugly frameworks. Why on Earth so many brilliant, talented, people are
waisting their skills on that shit is beyond me. I just won't. And I won't
teach it either. PHP and all the frameworks built on it are BAD for the
Internet.

### Browsers grew. Peace was made. The web got faster.

Maybe the Mayans were right. Yep. It seems the world has awoke to many
important improvements and the web world is among them. The following
factors have combined to obliterate the dark ages of bloated, dynamic
frameworks:

* Mobile first development began to dominate
* HTML5/CSS3 came out and was welcomed
* JavaScript got fast, really fast
* SQLLite and NoSQL databases emerged
* git and GitHub saw mass adoption
* Static web site frameworks (Jekyll)
* People just got sick of [horrible][] sites

Mobile devices proved slower than their desktop counter-parts, which
got developers concerned about speed again.

### Mashable services and client-side power leave static standing

But clearly the leading reason for this reemergence boils down to:

1. The proliferation of Mashable services
1. The increase in cross-browser, client-side power

Almost instantly the need for WordPress plugins vanished. Once these
plugins were essential to anyone that wanted a shopping cart, comments,
advertising and more. But not just plugins have taken the hit, entire
frameworks are falling decrepitly by the wayside such as Joomla, Drupal,
and Django. We just don't need them anymore.

Show me a Wordpress plugin for something someone *really* needs and
I'll show you an embeddable service that already does the same thing.

### Keep is simple ...

The burden of proof has clearly shifted. Developers now have to prove
there is a need for dynamic elements instead of assuming they will be
there from the start.

But some still haven't learned.

Some web developers have taken the power of JavaScript too far
suggesting that the entire web, HTML, CSS and all the rest should be
replaced with pure JavaScipt and a very fat, smart web browser, (well,
to be fair, as fat as the modern browsers already are). These guys
might be well intentioned but what they suggest would obliterate the
resurgence of the static web which is not only speeding everything up,
but also opening web development back up to the simple masses as was
originally intended.


### Static blogging ain't just for blogging

Tools like [Jekyll][], which [Obama][] used in his campaign, demonstrate
the sheer power and simplicity of the static site paradigm. Even though
Jekyll started as static blogging engine from what I can tell from the
first blog posts to GitHub it certainly has grown into much more.

As if returning to the static web were not retro enough, [Sublime][],
[vim][] and [Markdown][] have returned us all to an age when word
processing is done on a terminal and not a bloated, ugly word
processor. Just like before we markup special emphasis as easily as we
type other words and live with it appearing in-line, then we tweak the
presentation of the whole hot mess with CSS beyond our dreams back
then. No more, "Oh, was that an H2, damn I missed it" like you get
with incompatible Microsoft Word docs.

### You can always add dynamic later

Mobile and cloud seem to have shaped server-side functionality into
manageable, granular bits of event drive functionality couched in
events. It's no surprise to me (and others) that [node][] is taking
off so quickly because of it. It seems the modern static web is in
love with the ripped server-side power tools (notice I did
not say *framework* and yes I'm wearing [skinny jeans][]) like node bring to the party.

Thank you static web for putting the fun back into writing and web
development. I owe you a beer. Now will you dance on the table? (Oh
God, who invited tables.)

[Gopher]: http://en.wikipedia.org/wiki/Gopher_(protocol)
[GopherImg]: /images/archie-gopher2.png
[Jekyll]: /images/jekyll.png
[Markdown]: https://help.github.com/articles/github-flavored-markdown
[Mosaic]: /images/mosaic.jpg
[Obama]: http://kylerush.net/blog/meet-the-obama-campaigns-250-million-fundraising-platform/
[Sublime]: http://www.sublimetext.com/
[crap]: http://blog.ircmaxell.com/2013/09/rambling-on-internals.html
[horrible]: http://lakenorman.com
[node]: http://nodejs.org 
[skinny jeans]: https://twitter.com/noahlz/status/365519263236235266
[telneting]: http://en.wikipedia.org/wiki/Telnet
[vim]: http:///vim.org
