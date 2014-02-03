---
layout: post
title: Web Accessibility Over Design
subtitle: To Underline or Not to Underline
---

Web accessibility often gets thrown out because of someone's design
requirements or artistic sensibilities. Why? What is your goal? To look
good for the majority or be functional for everyone.

**TL;DR:** Follow [webaim.org][]'s recommendations when creating your web
sites and apps unless you *know* no one with any sight impairment will
ever want to use it.

![Put a damn line underneath][]

I've never met [Jen Myers][] but I like her already. That's her calling out all of
us that put design over function, something we web and mobile developers
all need to remember --- especially as current or aspiring instructional
designers.

### Don't be me.

I've been away from web design for a while (since my
[90s Teleport and Nike days][]) but I've kept up enough to know [bad design](http://robmuh.me)
when I see it &hellip; or at least I think so. &hellip; OK, OK, what the
hell do I know about design? I'm just a coder after all, right? Let's
just say my design-muggle eyes know [really bad design][shittysite] when I
see it. (I'm curious, how long did it take for that site to load for
you? For me, on a screaming machine it still takes a full two
seconds.) Still I forgot something we all should remember.



Recently I grabbed a nice [Jekyll][] template from GitHub during the
[GitHub Automatic Pages][] creation (as I recommend to my students as
well). Later when Jen tweeted this I thought, "Oh God, I hope it wasn't
because she visited my site." I was so embarrassed to realize that,
although I just earned my [Online Instructor Certificate][], which
included an entire unit dedicated to web accessibility, that I had quickly
picked a cool template that missed one of the easiest things to catch:

**My links were not distinguishable to those with visual impairments.**

I knew better and fixed that immediately.

### "Put a damn line underneath"

&hellip; to use Jen's words. It really isn't that hard. In fact, it
is the default unless you turn it off:

{% highlight css %}
a {
  text-decoration: none;
}
{% endhighlight %}

Removing these isn't that hard. And if you don't particularly like how
the underline text decoration looks, use a border instead:

{% highlight css %}
a {
  border-bottom: 1px solid;
  text-decoration: none;
}
{% endhighlight %}

### But what about just making them bold?

I thought about this a lot and tested. I don't believe bold alone covers
it and from my reading of [webaim.org][]. That's not really a solution
the visually impaired agree with.

However, I did give in with blog excerpts where the `H3` header is
linked but I also added a 'More&hellip;' continuation at the end of
the excerpt that is underlined, colored, slightly bolder and inverts
on focus and hover, which reminds me.

### Hover is not enough, add focus as well

This was new to me. Read about it on [webaim.org][] and understand it.
A lot of people use tab to get to your links and your cool inverse
hover event will not trigger without adding the focus event.

### Why so many links?

While we are on this, why are there so many links on your site anyway? Can
you imagine navigating sites like [this, (my favorite example of a bad site)][shittysite]
with just tab? Thank God for the mobile-first,
responsive design movement and the HTML5 that enables it so
wonderfully.

### Does everyone need accessibility in their site?

I'm open to feedback on this one. At first it feels like a no. But
still why not go ahead and make it accessible anyway? You should have
a really good case for it.

For example, I have a client currently who is putting his instructional
golf videos online and into an app. At first it almost seems like
vision accessibility should not be an issue since golfers will generally
be able to see well, it's a big part of the sport. But there are obviously
color-blind golfers. So yes, he needs accessibility as well. In his
case, however, visual accessibility comes through mobile-first design
elements and not necessarily underlines.

### Remember

I don't want to believe there are designers out there that knowingly
ignore those with visual impairments but there are definitely a lot
of us who forget to think about it. Now that have been reminded we will we remember?

[90s Teleport and Nike days]: http://linkedin.com/in/robmuh
[GitHub Automatic Pages]: http://pages.github.com/
[Jekyll]: http://jekyllrb.com
[Jen Myers]: http://twitter.com/antiheroine
[Online Instructor Certificate]: http://www.rccc.edu/distance/internet-courses/
[Put a damn line underneath]: /images/put_a_damn_line_underneath.png
[webaim.org]: http://webaim.org
[shittysite]: http://lakenorman.com
