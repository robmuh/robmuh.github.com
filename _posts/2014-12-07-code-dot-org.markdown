---
layout: post
title: Code.org - Introduction to Computer Science
subtitle: Things to Know and Some to Avoid
---

Want to avoid students nearly in tears from the otherwise great
code.org puzzles? Make sure you understand the following before
embarking on your own code.org experience or requiring it of your
students.

**You might bookmark this page. I am updating it with new information
regularly as I run into it.**

The [Introduction to Computer Science](http://studio.code.org/s/1)
is the first block in every students stack here at [SkilStak Coding
Arts](http://skilstak.com). It is so fantastic and fundamental I
created a [Python version](http://github.com/skilstak/code-dot-org-python)
of every puzzle to build student skills with typed programming challenges
using the same tools and methods professional programmers do. I
really do believe in the code.org approach and applaud everyone
involved in bringing this amazing resource to the world.

However, I have witnessed student after student struggle with the
same things as they complete the challenges, some nearly in tears
from the frustration. Here's how to avoid them.

# Complete ALL of Every Exercise Yourself First

I am glad I did. I have encountered other educators who not only
did not know how to program at all themselves, but had not completed
even one challenge in the code.org set they assigned to their
classes. I simply can't understand this at all. I realize public-school
educators are particularly overworked and underpaid but I find it
really hard to accept any excuses for not actually doing the work
themselves first. Students who detect this are particularly unforgiving
&mdash; especially when they begin to struggle themselves.

# Instructions Not in View

On many default web browser windows the instructions for the puzzle, which
contain the essentials hints are truncated at the bottom of the screen. Few
students actually read that same text when it pops up in the modal window at
the beginning of the puzzle and then don't realize it is down there.
Getting students to actually read instructions is hard enough without them
not even seeing them at the bottom left of the page.

# Videos Not in View

Videos are even more hidden on the bottom left and students frequently
click it off and go on missing critical information.

# Unplugged Videos Mixed with Instructional Videos

Here's a funny dialog that happened last week:

"Hey which one are you on?"

"There's some weather man explaining something."

The weather man was Bill Gates explaining 'if' statements about taking your
jacket out in the rain.

*Know Thy Audience*

The biggest instructional design flaw in the system as far as I'm
concerned is mixing the unplugged videos with real-content videos:

* Unplugged videos talk to teachers not students
* Students cannot distinguish between core content videos and unplugged
* Many classes will not be doing the unplugged activities
* Students become bored by the unplugged videos and skip them
* Students form the bad habit of skipping videos
* Students miss important videos about core concepts from skipping

I had a hard time myself knowing when I could skip videos.  The
entire series should have eliminated the parts that speak directly
to teachers and focused solely on establishing a dialog with the
student completing the challenges.

The first time Kiki or one of the other educators begins using
educator vocabulary and speaking with a tone as if talking to other
teachers you **lose** the student and the trust of the student later
that you will not bore them with teacher stuff. Students should not be
expected to make this distinction themselves.

One way around this is to have fun with the personalities of the
actors, which are memorable. I'll say something like, "We like Kiki,
but you can always skip her." Or, "Brini's my favorite. I think I
have a crush on her because she skateboards. Make sure you listen
to her talk about functions." Or, "Listen to Bill Gates the weather
man!" The kids laugh and remember the faces of those they need to
remember since these are at least consistent.

# Students Can't Hear or Understand the Videos

Beyond the problem of mixed video audiences you have the normal
challenges of video content more-or-less being required and a
classroom of distractions to deal with.

Even in my small nano-school with four students maximum at a time
the volume and excitement levels can make it hard for anyone to
focus. You don't have to be a 25-year veteran programmer to know
computational thinking demands an intense level of focus. Code.org
is no exception. Do whatever you can to reduce noise and allow each
student to feel encouraged by their peers around them, but also
clearly isolated themselves from them when they choose to solve
their code.org problems. This is particularly important if a
high-percentage of your students are ADHD, ADD, or on the Autism
spectrum (as are at least 20% of our small student body).

We went ahead and purchased [Studio Beats
headphones](http://www.amazon.com/Beats-Over-Ear-Headphone-Discontinued-Manufacturer/dp/B008CS5T76)
for our small school despite the cost for the following reasons:

* The kids **love** them
* They have great sound
* They isolate external sound
* They are famous for rough use and have replaceable/washable parts

They were expensive, but a much better investment than the $2
headphones I've been forced to use at some college media centers.

# Blockly: Not Enough Room

This is the first of the Blockly annoyances where Blockly actually
fails at its core mission of removing the syntactic and other
distractions from programming (over, say, typing real code).

Even though we have touch-screen laptops in our school enabling
kids with even the weakest motor skills to do code.org, inevitably
they will get to puzzles where they can't fit everything in the
workspace. This is particularly evident in [Stage 13: The Farmer
2 #1](http://studio.code.org/s/1/level/71) where students are given
infinite blocks to resolve the puzzle on a finite workspace. The
puzzle can be solved nicely within the workspace provided, but only
by those who are particularly good or persistent. Here's the smallest
solution we've found so far:

![s1level71](/images/s1level71_solution.png)

The point is when you start forcing the student to scroll the
workspace you not only defeat the purpose of an 'easy' interface,
you compound the problem by increasing the risk of losing everything
or getting the infamous 'you have unconnected blocks' bug, (which
I discuss next).

Sometimes you can change your computer screen resolution to buy you more
code.org workspace, but not everyone has that option.

# Blockly: Bugs With Unconnected Blocks

More than once a student and I have been unable to find which block is
unconnected. We think it might be off the screen, but more than once we have
been dealing with only blocks on the screen. The only solution to this bug,
no matter how much time you have invested (as in s1level71) is to reload the
page, (which I discuss below).

# Blockly: Losing All Your Progress

More than a few times students visit other pages, check their
progress, or otherwise click off the page or close it only to realize
they have lost everything they did on the page for that puzzle.
This is definitely a tear-inducing experience for a dedicated young
student. The worst part is that it is not an experience consistent
with actual programming careers because although lost work is part
of life, in a real programming environment you have auto-saves (such
as Python IDLE) or are using GitHub, (as we do), to regular save
progress. When an early learner experiences the sorry-no-going-back loss
they may conclude incorrectly that this is what life is like &mdash;
especially if they have heard "welcome to my world" a few times on other
matters related to programming in general. Associating unrecoverable loss
with programming careers and past-times is not fair nor is it necessary.
Blockly could be improved to do this auto-saving.

# Blockly: 'Show Code' Truncates

When I discovered 'Show Code' in the upper left I was sold on code.org's
approach over every other graphic teaching tool. Why? Because students can
actually see *real* code being created, that is, unless they do to much of
it. That's right. Clicking 'Show Code' truncates after about 20 lines of
code. This carries a number of frustrations for the student and teacher.

First, students are unable to see all the code of their most impressive
creations. "I created 80 lines of code, Mr.Rob!" they proclaim, but are then
unable to see any of it.

Second, students instinctually want to save this JavaScript code
and do stuff with it. In our school we started by putting it into
a long comment in Python and porting the Artist activities to Python
Turtle &mdash; especially the cool tree program at the very end.
This in turn led to the creation
[code-dot-org-python](http://github.com/skilstak/code-dot-org-python).
Unfortunately this truncation prevents students from using Show Code to help
them write actual code in whatever real language because they simply can't
see it all.

# Blockly: Farmer and Maze Have No Speed Adjustment

Students quickly become bored and aggravated by the time it takes
Farmer and Maze puzzles to complete. This makes keeping students
attention very difficult. The lose focus, disengage, and start to
distract others. The artist puzzles at least allow this to be sped
up.

# Blockly: Farmer and Maze Don't Let You Save Success

When you get one of these puzzles right you are never given the
opportunity to save it or even study why and how you finally
succeeded. The modal window that pops up blocks your answer and you
are immediately taken to the next puzzle blowing away your previous
solution if you try to go back to it. This is insanely annoying for
both teachers and students &mdash; especially when the 'Show Code'
option on the success modal window won't even show your whole
solution.

# Negative Counter Loops

[Stage 11, The Artist 3, #10](http://learn.code.org/s/1/level/68)
implied a negative counter loop but doesn't discuss the possibility
of adding a '-' anywhere. To make matters worse it accepts both a
positive 10 or a negative 10. This requires explanation to almost
every student and does not translate to other programming outside
the code.org puzzles.

# Unnatural Restrictions Reinforcing Bad Practices

Some of the Puzzles let you use 'if else' and others do not. Forcing
students to do it only one way seems inconsistent with the goals
of the puzzles themselves &mdash; especially when the result
emphasizes using redundancies and bad coding idioms rather than
what would normally be available to them if it were not for the
artificially enforced limited block use.

One small example of this is, again, [Stage 13: The Farmer 2
#1](http://studio.code.org/s/1/level/71) where an 'if else' block
would have been better than two 'if' blocks. Other examples abound.

# Function Naming Confusion

In the Farmer puzzles the green 'Remove 6' is always confused with the
singular 'Remove 1' block from the Actions group of blocks. Students will
regularly put the green 'Remove 6' function call block into the function
itself even with the example of putting a 'Repeat' block with a 'Remove 1'
action block right next to it. I don't know the solution, but it would
likely involve making a clearer name distinction between the function
definition and name and the action name, which technically is also
a function call.

# Learn and Teach to Use Page Reload

Even though there is a 'Reset' button at the bottom reloading the entire
page is often a much better solution. This is consistent with professional
programming techniques as well. At a certain point the code, whether it be
Blockly or Python, because so convoluted and hard to follow that it is
faster to simply start over. Frequently this is exactly the resolution
a student needs when they realize they have vastly overcomplicated an
otherwise easy solution. Helping students have this realization experience
is fundamental to learning computational thinking and challenge-based
learning. Make sure the students understand that scrapping it all and
restarting might seem like a failure, but actually it is part of the process
at decomposing the problem in search of the best solution (as in Thomas
Edison and the light bulb.)

# Enlist Help

Many of my senior students have independently started or helped run
code clubs at their main public schools. If you are lucky enough
to have one or more of these types of students around ask them to
help since they can guide the other students through the harder
challenges mentioned previously.
