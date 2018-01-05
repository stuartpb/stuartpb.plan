2018-01-05 11:36 Eastern time (I'm in Pennsylvania, flying back to Seattle in a few hours): currently putting together the `perimeterExtrude` function I described in https://github.com/jscad/csg.js/issues/68#issuecomment-355041376 in https://ide.c9.io/stuartpb/csgjs

thinking about generalizing this to 3D, I'm sort of freaking myself out thinking about how inner arcs overlap, and how that probably means there should be a point along the "Y" axis (which would *rotate* in 3D) for the clipping plane (to avoid self-intersecting), and how, like... this only applies on corners...

Except that it doesn't, because if you've got a 15-degree turn, you've got two planes that are intersecting...

Okay, so, for rounding corners, you basically need to have the *inside* angled on the bisector every time, and then you can do the corner interpolation along the *outside only*. Which I basically already knew, which is why I already had the rule "internal corners need to be curved on the path" and everything.

---

next time I've got a minute I should write the one main thing I made github-best-practices for: an explanation that usernames / orgnames on GitHub are not prefixes, because of the fork graph, and if your org is (or you personally are) using them as such, you're doing GitHub wrong, and not playing nice with the concept of contributions in PR form
