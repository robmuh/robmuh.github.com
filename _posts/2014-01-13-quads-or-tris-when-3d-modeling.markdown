---
layout: post
title: Quads (Rectangles) or Triangles When 3D Modeling?
---

At some point when learning about game-focused 3D modeling you'll run
across a discussion about rectangles vs triangles. My son and
I recently revisited this during his Blender experimentations. The
quick answer is use quads, but a triangle here or there usually isn't
bad.

The rest is very well explained in [this thread][].
Here's a nice image from a post by [Chosen Few][] to that thread:

![How a Human and Render See
Geometry](/images/human_vs_render_geometry.jpg)

I think what can get confusing is that all computers end up using
triangles after the model is [tessellated][] and sometimes game
modelers will specifically use triangles throughout because of that.

Another complication is that very organic tools, such as [Mudbox][]
use triangles, sometimes millions of them, instead of quads.

I'm no expert here, but I've see enough of the game contributions to
[Dota2][] and [Second Life][] to fee safe recommending modeling in
quads and dealing with triangles as needed.

In fact, if I remember right it was quads that I used in Blender to
create the rather simply lotus flower petals for this [Living Goddess Ballet
Pixelle][] build some time ago:

{% include youtube.html id="6fX_wdbslrQ" %}

Have fun building.

[this thread]: http://community.secondlife.com/t5/Mesh/Basics-Q-Quads-or-tris-when-modeling/td-p/1302581
[tesselated]: http://en.wikipedia.org/wiki/Tessellation
[Mudbox]: http://en.wikipedia.org/wiki/Mudbox
[Dota2]: http://www.dota2.com/workshop/
[Second Life]: http://wiki.secondlife.com/wiki/Mesh/Creating_a_mesh
[Living Goddess Ballet Pixelle]: http://psg.com/~pixelle/Theater.html?ballet=LivingGoddess1
[Chosen Few]: http://community.secondlife.com/t5/user/viewprofilepage/user-id/152453

