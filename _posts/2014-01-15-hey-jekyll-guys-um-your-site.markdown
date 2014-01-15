---
layout: post
title: Hey Jekyll Guys, Um, Your Site?
---

Yep, confirmed. The [main jekyllrb.com documentation][main]
([jekyllrb.com][]) is out of sync
pretty badly from the [documentation that is bundled with Jekyll][bundled],
which is located in the site directory. Of course the first is on the
gh-pages branch and the second on the master branch. [Here's the
diff in a gist][gist] and the [issue I opened about it][issue].

It's almost as if the Jekyll maintainers didn't read the [GitHub
instructions about using the gh-pages branch][github] but I'm sure
that's not it.  I'm still very new to Jekyll, which in this case may be a good and a
bad thing: good because I'm looking at the documenation on the main
jekyllrb.com web site a lot more
than most of the other Jekyll/Ruby pros; good because I very recently
[RTFMed on GitHub][github] that all *projects*, which this is, have to
be on the gh-pages branch; bad because I may not be aware of some special
magic that might be happening (or should be) to make site/docs on
master sync with the docs directory on the actual site source.

If I'm missing something let me know. Happy to help fix if I can.

[main]: https://github.com/jekyll/jekyll/tree/gh-pages
[jekyllrb.com]: http://jekyllrb.com
[bundled]: https://github.com/jekyll/jekyll/tree/master/site 
[github]: https://help.github.com/articles/user-organization-and-project-pages
[gist]: https://gist.github.com/robmuh/8433813
[issue]: https://github.com/jekyll/jekyll/issues/1954
