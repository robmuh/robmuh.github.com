---
layout: post
title: Good Developers Use Linux
subtitle: Personal Reflections on an Undeniable Truth
---

I'm finishing up a VMware Ubuntu Linux Desktop on a Stick image for
[SkilStak Coding Arts](skilstak.com) with one goal in mind. Marginalize
Windows &mdash; and even Macs &mdash; in my students' minds.

Here's the reality. I've met and worked with a lot of respectable,
intelligent developers out there over some 25 years, but the ones that
are head and shoulders above their peers &mdash; not just the rock stars,
not even the masters: the code geniuses who quietly and decidedly blow
away their peers in performance, aptitude, and raw skill &mdash; all
use Linux as their primary desktop. Among them those that use vim turn
out to be even more intelligent and capable. These folks can leverage
any operating system foisted on them, but they excel using Linux. In
fact, if you **don't** use Linux on your desktop when you first
encounter one of these types, many of them will almost palpably dismiss
your mediocrity in subtle, but distinguishable ways. The reverse is
also true, if you do use Linux as your desktop the masses incorrectly
attribute more acumen than you actually possess to you.

### Why do the best coders pick Linux?

Bash. Why Bash? Because command-line. Why command-line? Because power,
raw, scriptable, i-don't-need-no-stinking-gui power, which is also why
they prefer vim as their primary editor.

### Why does anyone use Windows at all?

Windows is the cheapest, expandable purchase and a lot of software
offerings &mdash; including most big-name games &mdash; won't run
on anything else. This is why I personally picked Windows as our main
operating system at SkilStak. Games run best on Windows and if they don't
you can upgrade components of your system, you can't on a Mac. As much
as Steam has leveled the playing field, there are still tons of games
that will not run on Linux or Mac.

More importantly, however, some important game development engines
and frameworks won't run on anything but Windows (Gamemaker Studio,
Cryengine, etc.). So you go with Windows if your company teaches
programming through game development and gives out gaming-time reward
sessions for programming achievements (via SkilBux) as incentive. Often
the games kids want to play together during a camp are not those that
will run on anything but Windows.

Also most students have Windows already available to them &mdash;
especially if it is their first computer and their parents are stretching
to justify the cost.

### Gamemaker Studio == Main Reason @skilstak

I've done a lot of research on the topic and Gamemaker Studio is still
the best all-around, serious game development tool that both a 7-year-old
can use as well as a professional or amateur indy developer. It has
its quirks to be sure, but enjoys a solid place in the industry &mdash;
for now &mdash; especially for real 2D game development.  At SkilStak
we make a point of helping students learn real tools as much as possible
rather than just-for-education toys whenever possible.  When considering a
tool the first questions are "Can a seven-year-old use this?" followed by
"Can students use this in the real world?" or "Can this be used to make
something I can upload to any app store?"  This is where Gamemaker Studio
stands out even if it is a Windows-only thing. It does, however, create
games for all platforms (much better than Corona SDK does, for example).

### The Mac Conundrum 

Macs are great computers and arguably the first pick by all developers
I've met with the money to buy one (and all the software to make it
actually do what they need). This is particularly true in the mobile and
web application space, particularly since you can't even develop apps
for Mac unless you have one (and you can still develop for Windows and
Android from a Mac but the reverse is not true).

The game development world these days also seems to support Macs. Unity3D
will run on it. Blender and the rest of the 3D modeling apps.  Source,
Unreal and other engines support Mac as well as Windows (CryEngine3
will not, however.) You can even buy Fusion and run Gamemaker Studio on
a Mac without a problem. So even though there is always a little note 'on a
Mac you have to take these additional setup steps' Macs seem capable of
supporting a wide range of development &mdash; for the money.

Macs are expensive. They say you get what you pay for, but I don't buy
it, literally (although we do have them so we can develop for iOS). You
can get twice the resources &mdash; and a touch screen &mdash; in a
'Windows' machine.

**Wha? No Touch?**

While I have not cared enough to research it. It has always perplexed
me that arguably the company that introduced touch to the mainstream
has not put touch on their desktops and laptops yet. I have heard some
posit that this was because it would "cut into their iPad" sales,
which if true, is utterly ridiculous. But what is to stop them? Apple
made the brain-dead decision to turn the mouse upside down. Steve Jobs
admitted he stole the mouse design from Xerox, thankfully. Maybe their affair
with the mouse is keeping those touch screens down. Maybe all those
elite artists cannot imagine the dank fingerprints on their screens
messing up their 4k resolution displays.

Whatever the reason, this is why truly elite developers will go with
Ubuntu and a touch screen instead of Mac. I can say that since moving
to this combination my coding efficiency has never been higher.

**Touchpads Suck**

They always have. But to a mobile developer with a laptop it was the next
best thing. No carpal-tunnel-inducing mouse required. But God help you if
you don't turn that insidious touch pad off during a 90 wpm code session.

**Touch Screens Rule**

Enter the touch screen and software that supports it (like Ubuntu).
Now you can leave off that touchpad (although it can easily be turned
on if your desktop apps ever glitch, which unfortunately they still
do, \*uh hummm, cough, Chrome\*). This combination is ideal for those
that develop on a laptop since their fingers are a short distance away
from the screen and no resyncing of mouse to brain to screen has to
take place.

**Package Management**

The main reason most developers will always go Linux &mdash;
particularly a flavor of Debian like Ubuntu &mdash; is because of
package management. Macs have homebrew but this is really not close to
the use and control *apt* will get you on Debian.

### One Solution

Increasingly I read of really good developers separating their
selection of primary computer from their main work environment. One
calls her Mac a 'glorified ssh terminal' because most development is
happening in the cloud and not directly on the systems attached to
the developer's lap. Even if not having Internet access is an
unmentionable sin to the mobile developer community, it does happen,
and it's not always all that efficient.

So why not make your 'glorified ssh terminal' a bit bigger and use
a Linux VM that models most of your cloud operating systems. You can
still use it to connect to your cloud VMs for sure, but you also get
the advantages of full-blown Linux at your disposal, touch and all if
you like, as well as a full environment to do all aspects of that
development.

And you can take snapshot backups of your VM anytime and use them as
backups or share them.

This is where SkilStak Desktop on a Stick came from (following on Server
on a Stick). Rather than decide which version of Frankenstein's monster
you want to make out of your Windows machine to make it grunt like Linux
(putty, ConEmu, git-scm, cygwin, msysgit, GitHub git-shell) you can
actually have Linux on every Windows system (or Macs if you want to
fork the $80 for each copy of Fusion).

This makes updating every student system simply a matter of
distributing the zip with the free VMware player and your updated
image to all student PCs. Then just add an icon to boot it up with
a default login. Once they go full-screen they will never even know
they are on a Windows machine, unless they need to be.

There are a lot of virtual machine offerings, VirtualBox and VMware
seem to lead them and even if you do pay a hundred dollars or so for
a commercial offering, that is money spent on having several computers
at your disposal instead of just one. For example, I can run the main
VMware Professional application on both my Ubuntu and Windows machines
for commercial development and creation of educational images for the
same cost and can always use VMware Player anywhere else I might need
to run them.

More on use of Desktop on a Stick later ...
