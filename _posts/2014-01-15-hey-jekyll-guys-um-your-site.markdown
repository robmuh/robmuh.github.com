---
layout: post
title: Hey Jekyll Guys, Um, Your Site?
---

Yep, confirmed. The [main jekyllrb.com documentation][]
([jekyllrb.com][]) is out of sync
pretty badly from the [documentation that is bundled with Jekyll][], which
is located in the `site` directory. Of course the first is on the
`gh-pages` branch and the second on the `master` branch. Here's the gist:

{% gist 5555251 %}

I'm still very new to Jekyll, which in this case may be a good and a
bad thing: good because I'm looking at the documenation on the main
jekyllrb.com web site a lot more
than most of you other Jekyll/Ruby pros; good because I was very recently
[instructed by the GitHub docs][] that all sites have to be on the
`gh-pages` branch; bad because I may not be aware of some special
magic that might be happening (or should be) to make `site/docs` on
`master` sync with the `docs` directory on the actual site source.

If I'm missing something let me know. Happy to help fix if I can.

[main jekyllrb.com documentation]: https://github.com/jekyll/jekyll/tree/gh-pages
[jekyllrb.com]: http://jekyllrb.com
[documentation that is bundled with Jekyll]: https://github.com/jekyll/jekyll/tree/master/site 
[instructed by the GitHub docs]: https://help.github.com/articles/user-organization-and-project-pages
