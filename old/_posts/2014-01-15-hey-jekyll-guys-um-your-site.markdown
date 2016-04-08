---
layout: post
title: Hey Jekyll Guys, Um, Your Site?
---

Yep, confirmed. The main Jekyll documentation at [jekyllrb.com][] is out
of sync pretty badly from that which is [bundled][] with Jekyll. Of course
the first is on the gh-pages branch and the second on the master branch.
Here's the [gist][] with a diff and the [issue][] I opened about it.

It's almost as if the Jekyll maintainers didn't read the GitHub
[instructions][] about using the gh-pages branch but I'm sure that's not
it. I'm still very new to Jekyll, which in this case may be a good and a
bad thing: good because I'm looking at the documentation on the main
[jekyllrb.com][] web site a lot more than most of the other Jekyll/Ruby
pros; good because I very recently read that all *projects*, which this
is, have to be on the gh-pages branch; bad because I may not be aware of
some special magic that might be happening (or should be) to make
site/docs on master sync with the docs directory on the actual site
source.

If I'm missing something let me know. Happy to help fix if I can.

UPDATE: Seems like there is some sort of reason for this, but I can't
imagine what it is. Best news is that [@parkr][] is very responsive
and thinking about these things. Threw my name in to help. We'll see.

UPDATE: Here's [Mr. Jekyll][] himself clarifying the concern about
updating the public docs with information about stuff that has not
been bundled and packaged into a release yet:

![@mojombo clarifies][]

That I get. Just unclear why the stuff unrelated to releases isn't
immediately updated in both places to prevent them from getting out of
sync, or worse, stuff in one place eventually blowing out changes in the
other.

FunFact: Found this write up of Obama's [tech][] during the campaign. He
used Jekyll.

[@mojombo clarifies]: /images/mojombo_on_jekyll_docs.png
[@parkr]: http://github.com/parkr
[Mr. Jekyll]: http://github.com/mojombo
[bundled]: https://github.com/jekyll/jekyll/tree/master/site
[gist]: https://gist.github.com/robmuh/8433813
[instructions]: https://help.github.com/articles/user-organization-and-project-pages
[issue]: https://github.com/jekyll/jekyll/issues/1954
[jekyllrb.com]: http://jekyllrb.com
[tech]: http://kylerush.net/blog/meet-the-obama-campaigns-250-million-fundraising-platform/
