2018-01-05 11:36 Eastern time (I'm in Pennsylvania, flying back to Seattle in a few hours): currently putting together the `perimeterExtrude` function I described in https://github.com/jscad/csg.js/issues/68#issuecomment-355041376 in https://ide.c9.io/stuartpb/csgjs

thinking about generalizing this to 3D, I'm sort of freaking myself out thinking about how inner arcs overlap, and how that probably means there should be a point along the "Y" axis (which would *rotate* in 3D) for the clipping plane (to avoid self-intersecting), and how, like... this only applies on corners...

That's the thing, it only applies on corners, and there's a vanishing intersection point for extrusions where the far face is only slightly angled. OK, I'm fine.

---

next time I've got a minute I should write the one main thing I made github-best-practices for: an explanation that usernames / orgnames on GitHub are not prefixes, because of the fork graph, and if your org is (or you personally are) using them as such, you're doing GitHub wrong, and not playing nice with the concept of contributions in PR form
