---
layout: post
---

Yoeman, Bower, and Chalk are all far too opnionated for me ---
especially since their opinions are wrong and against established
community practices.

The frontend engineers (a term that still makes me chuckle inside)
come off as that annoying guy that has to be unique and do everything
his own way even if his own way sucks.

### "Solarized is broken"

No it's not, Chalk is. Solarized fixed a very broken color scheme that
existed from the creation of ANSI color. A professional photographer with
colors picked based on science and research about contrasts came up with
his color scheme. Chalk looks like someone spent too much time studying a
bottle of antacid tablets. We should be doing everything in our power
to bring the ideas behind Solarized to wide adoption, not shutting
them down with "I just refuse to work around a broken theme", as it's
creator says. But it doesn't end there.

### "We decided on 4-space indent"

Despite well-established standard 2-space indents by Google and the very
leaders of the Node community, the Yoeman guys (mostly guy) have decided
no, they don't give a fuck, they are doing it their way. This would be
fine if it were an isolated project, but it's not. Yoeman's a
*scaffolding* app designed to get people started out right on their
projects. This perfectly illustrates the problem. As soon as you say,
*everyone* should start out a particular way you get trouble ---
especially if that way is against what the rest of the entire community
has to say.

### Bower, Well-Intentioned and Unnecessary

It's all about the task manager and npm. We just don't need bower. For
example, look at the gulp-modernizr npm package. It allows the
incremental construction of usable modernizr parts. Were I using Bower
for that all I get is *all* of modernizr.js or all of jquery.js.
Anything that I would ever want will have a gulp-\* version and the
better ones will be smart enough to only bring in the front-end
material I need instead of the whole thing. Bower will never be able
to do that unless it becomes Gulp.

Besides, the granular, stream focus of Gulp makes is *perfect* for
analyzing my front-end builds and allowing me to only add what I need
from other front-end pieces later.

### Gulp Over Grunt

I'm sort of glad to see the Yoeman guys tripping over themselves
trying to say 'we like Gulp too' in order to keep people from chucking
the whole fucking yoeman-bower-grunt stuff in the garbage. Too late.
Already did. All I need is gulp and npm. 

