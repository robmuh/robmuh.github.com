---
layout: post
title: CoffeeScript Before JavaScript
subtitle: For education at least. Hear me out.
---

Many programmers dismiss CoffeeScript for different reasons, but
what if CoffeeScript turns out to be the best way to learn (and
teach) JavaScript for beginners &mdash; especially for those as
young as seven.

## No Really

Don't roll your eyes yet. Hear me out. 

I started web development in the 90s and coded Perl, shell, Java
and C most of my life. I dabbled in JavaScript when it came out and
like everyone else hated Python and PHP when they came out.

Things have changed.

Call it aged wisdom or something but I see JavaScript and Python
for what they are way beyond their syntax now. I also spend every
waking moment helping others *learn* to program instead of simply
programming. Where I once hated significant white-space I now
embrace it every chance I get. The logic that Code.org, Berkeley and the
rest of the *computational literacy* crowd follows
&mdash; nay touts &mdash; goes like this:

> The most important thing is for those learning to code to not get
> discouraged and frustrated early on so they don't prematurely abandon
> it. Therefore, the less concern for syntax and typos a certain
> approach has the better.

I share [George Saines'](http://blog.codecombat.com/3-reasons-why-computational-literacy-is-ruining-coding-education)
feelings on this position. In short, we need to get those learning
to code actually typing code as soon as possible and begin from
there. This is where CoffeeScript comes in. Here is a simple example
first in CoffeeScript and then in the well-formed JavaScript it
produces:

    do -> 
      weekDays = ['sun','mon','tue','wed','thu','fri','sat']
      order = {'sun':0,'mon':1,'tue':2,'wed':3,'thu':4,'fri':5,'sat':6}
      weekDay = (new Date()).getDay()
      today = weekDays[weekDay]
      times = document.querySelectorAll('.time')
      pnode = times[0].parentNode
      count = times.length
      lnode = times[count-1].nextSibling
      if today isnt 'sun'
        for time in times
          day = time.classList[1]
          break if day is today
          pnode.insertBefore(time,lnode);

Or this:

    (function() {
      var count, day, lnode, order, pnode, time, times, today, weekDay, weekDays, _i, _len, _results;
      weekDays = ['sun', 'mon', 'tue', 'wed', 'thu', 'fri', 'sat'];
      order = {
        'sun': 0,
        'mon': 1,
        'tue': 2,
        'wed': 3,
        'thu': 4,
        'fri': 5,
        'sat': 6
      };
      weekDay = (new Date()).getDay();
      today = weekDays[weekDay];
      times = document.querySelectorAll('.time');
      pnode = times[0].parentNode;
      count = times.length;
      lnode = times[count - 1].nextSibling;
      if (today !== 'sun') {
        _results = [];
        for (_i = 0, _len = times.length; _i < _len; _i++) {
          time = times[_i];
          day = time.classList[1];
          if (day === today) {
            break;
          }
          _results.push(pnode.insertBefore(time, lnode));
        }
        return _results;
      }
    })();

Now I know there are more clever ways to do this probably. This is
simply an example illustrating several principles combined with
some DOM manipulation to illustrate. But care to explain a
self-executing anonymous function to a 7-year-old?  I didn't think
so. How about `do` instead?  What about the very common and simple
`for day in weekdays` construct?  Compare that to the equivalent
for loop with its localized `var i` definition.

CoffeeScript is easier for beginners to learn and for good reason,
ironically it also *safer* for them to learn. 

## They Still Learn JavaScript, Just Better

When the time comes they are ready to see the JavaScript produced
and study the individual equivalents and what they mean. As their
programming skills grow they will have more and more exposure to
the post-processed code, its style and proper syntax. This is simply
the best way to learn rather than having every single JavaScript
Wart and best practiced spelled out in class or by reading a book.
Students are encouraged to think, "what would the CoffeeScript
compiler do".

It is true that learning CoffeeScript first defers learning actual
JavaScript. Some might even argue that this prevents students from
learning proper JavaScript eventually. I think that is false. If
anything it encourages them not to repeatedly shoot themselves in
the foot with JavaScript problems and bad practices they may not
be aware of.  Soon they will understand what is happening in clear
terms and be able to converse in either and be better programmers
for it in the end.

## Whitespace IS Significant

How would you teach a child? Would you teach them that indenting
really doesn't matter? Boy I hope not.  Would you encourage them
to write spaghetti? Probably not. Whitespace simply *does* matter.
These are the very reasons Python is taking over the education world
as the first *real* language to learn and why it is the default
language for CodeCombat.com and SkilStak as well. This acknowledges
the need to keep things the least frustrating for those starting
out while keeping it real.

This is the exact same reason that learning the preprocessors Jade
and Stylus are *better* than learning actual HTML and CSS for
beginners. It follows for CoffeeScript as well. Not only do students
learn the tools and workflows modern professionals prefer for their
simplicity and speed of development, but they learn the actual code
better as well.

## Clarity Beats Cleverness

Stop telling yourself that it doesn't. You may say you want your
curly freedom but you curse the developers that abuse it and you
know it.  Usually they are the worst programmers you will ever
encounter.  Every memory I have of any programmer who didn't use
proper style, or any style, or who filled code with actual tab
characters AND 4-space indents and then picked horrible variable
names has *always* turned out to royally suck as a programmer in
general. Maybe it is the Swiss in me, but bad style *ruins* code.
Obfuscation competitions are fun anomalies but are built on a bad
premise, that making code that others can't understand somehow makes
you smarter than them.  That's just bullshit.

That said, I have heard the other extreme applied to torpedo use
of regular expressions based on that premise, but that is going too
far.  Even 7-year-olds can and should learn regular expressions
eventually.

## Can a 7-Year-Old Learn This

As Einstein said, "If you can't explain it to a six year old, you don't
understand it yourself." This is the true measure. In my world this translates to, "can you teach it
to a 7-year-old."

There is something innate in every young person I've run across
that has something to prove to themselves and everyone else, build
their own computer, type faster than their parents, code something
most everyone else around them doesn't understand. Whatever it is,
it seems to subside once that person has mastered the challenge
enough for it to become mundane. Like loud v.s. classical music it
seems tastes shift from showy to beauty, efficiency, and clarity; to well
thought-out, practical ideas and innovation.

## Stay Flexible

As someone responsible for the learning direction of so many this
all reminds me to stay flexible, adaptive, and open-minded as a
technology teacher, something students also need to learn as well.
Hey, I came to accept, even love JavaScript even after *experiencing*
it in the 90s so there is that.  I'm sure so many educators will
think I have lost my mind, but I have observed applying the following
progression tree to work in my classroom and that really suffices
for me:

    Code.org -> CodeCombat -> Python -> Jade -> HTML
                                     -> Stylus -> CSS
                                     -> CoffeeScript -> JavaScript
                                     -> Java -> Android
                                             -> MC Spigot
                                             -> MC Forge
                                             -> MIT BattleCode
                                     -> Swift -> iOS
                                     -> GameMaker (GML)
                                     -> Bash
                                     -> C

I would love to hear others' thoughts on this but it is nearly
impossible to even find *anyone* teaching any of this in a physical
setting &mdash; least of all the public school system. If you do, please
leave a comment or email me. I'd love to meet you.
