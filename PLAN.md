# Right now (2018-01-27)

I'm a little disappointed that I never got around to describing [last week's projects][] (or [my Black Mirror pitch][]) in more detail: hopefully they can all get covered / elaborated on as I work on them more in the future.

[last week's projects]: https://github.com/stuartpb/stuartpb.plan/commit/b3fda4df84873bc244cab066f87bfd19e6dd2a54
[my Black Mirror pitch]: https://github.com/stuartpb/pitches-and-scripts/blob/master/tv-spec-scripts/black-mirror/lets-talk-tommy.md

I made [a desktop dock for my phone][dockitall] earlier this week, having found no parametric OpenSCAD charging docks on Wikipedia and not really being satisfied with the existing Pixel 2 XL docks on Thingiverse. I was originally plan on rewriting it to use additive geometry instead of the increasingly-byzantine geometry used in the current rough draft, then maybe re-printing it with some tweaked parameters and/or better quality and/or new material: however, the parameters I initially printed with were good enough (after wrapping the tip of the cable in double-stick tape), and I've kind of moved on for now.

[dockitall]: https://github.com/stuartpb/dockitall

I made a model for [a broken piece from the coffee maker I sometimes use for tea][b.scad] (I only use an AeroPress for coffee: it's bad enough for my teeth without the acidity of drip brewing), and have done a little initial work on making something to put over the broken hinge on my Brita pitcher lid (nothing workable enough to commit and push yet, though), which I'd put alongside it in the same repository.

[b.scad]: https://github.com/stuartpb/fiddly-bits/blob/master/b.scad

I also started writing up files for [a variant of Tic-Tac-Toe I used to play in my grade school days][nuketactoe], under the idle curiosity of whether or not its distribution of scoring made it a "dumb" game (ie. one in which it's almost always a tie, or some other such defect), or if I was actually on to something (after a comment exchange on Reddit led me to read about other variants like [Ultimate Tic-Tac-Toe][] on Wikipedia and find no mention of the game I'd played).

[nuketactoe]: https://github.com/stuartpb/nuketactoe
[Ultimate Tic-Tac-Toe]: https://en.wikipedia.org/wiki/Ultimate_tic-tac-toe

I'm planning on rewriting the README for [barfspace][] to better reflect how I'm currently holding it (as a space for unpublished drafts that may or may not be perpetually-unpublished, on a case-by-case and subject-to-change basis), rather than a manic allusion to the thoughts I had when I was creating / last reworking it (taking into account some of the understandings I've come to about my own discomfort with the bleeding-edge typing-before-thinking style I originally had in mind around it).

[barfspace]: https://github.com/stuartpb/barfspace

I've started work on the Harriet Tubman stamp project I previously posted [as an Unusual Studio seed][b0328876] (mostly because, having found all the pieces I would need to begin the undertaking, I've been reticent to spend any $20 bills without one): I'm planning on pushing a first commit for it once I've dialed my first-draft approach into the right size (should be ready by tomorrow).

One thing I'm thinking I'm going to tackle before the next phase in the Tubman stamp project is a project I've been sitting on for a while to make a UI for https://github.com/jankovicsandras/imagetracerjs: working on that made me think about how, working on static-page apps again (it's been a while), how I think such projects should be architected (with devs targeting only the very latest releases of evergreen browsers, and tooling filling in every other browser release in the world), and writing an articl about that: thinking about writihng *that* got me thinking about writing *here*, which is how I ended up editing this right now.

Anyway, it's late and I've still got more stuff to jot down, so I'll hold off on posting about that backfilling methodology &c until tomorrow.

Thinking about the way that I'm handling and planning this project, versus how [its Adafruit inspiration][Adafruit article] was handled (with only a rough draft being published and the final iteration being unmentioned but for some photographs implying it was the product of the documented process) have given me [some thoughts to write up in sacred-tenets][].

[b0328876]: https://github.com/unusualstudio/unusualstudio-projects/blob/ea2dc1fdfd611025b825120839aa5b59dc0e533e/projects/b0328876-0695-4750-8948-3852b5511ae6.yaml
[Adafruit article]: https://blog.adafruit.com/2017/10/12/turn-your-20s-into-tubmans-with-this-diy-3-d-printed-stamp-wired-adafruit-ustreasury-stevenmnuchin1/
[some thoughts to write up in sacred-tenets]: https://github.com/stuartpb/sacred-tenets/commit/a4baae577dc3c014cdb5641af20d138e1859377d

My plan to [convert Lean Notes from a series of Trello boards to a series of GitHub-Flavored-Markdown files][leannotes/leannotes#1] has kind of run out of steam for the moment. I think I'd rather try my hand at fully translating the Understanding Lua boards / org to GitHub first; I could have sworn I'd made a repo for it under https://github.com/dashseat, but I guess I must have opened the tab to do so and then ended up Tabalanching it away. (I should also think about making a repo there for Google Blocks data.)

[leannotes/leannotes#1]: https://github.com/leannotes/leannotes/issues/1

I'm not quite ready to write about using Atom just yet: all I have to say about GitHub Desktop right now is that I've got [one major issue with it][desktop/desktop#3841].

[desktop/desktop#3841]: https://github.com/desktop/desktop/issues/3841

## Unusual Studio

I've got [99 projects][], but the list ain't one: I still haven't made any progress on rendering the project data into an easy-reading page format. This should be my top priority for the next week, if my preparations ahead of my trip to Florida don't get in the way (see "Schedule" below).

[99 projects]: https://github.com/unusualstudio/unusualstudio-projects/tree/ea2dc1fdfd611025b825120839aa5b59dc0e533e/projects

I'm still drafting [thoughts on the project schema][]: figuring out whether I want stage 3 projects to be separated out of the main list or not feels like it's probably the biggest blocker for me (as considering this is stopping me from adding things like my phone dock project above, for instance).

[thoughts on the project schema]: https://github.com/unusualstudio/unusualstudio-projects/issues?q=is%3Aissue+is%3Aopen+label%3A%22model+%2F+schema%22

## Email transition

I'm currently transitioning my email address from stuart@testtrack4.com (DreamHost) to s@stuartpb.com (FastMail). All email to the former is directed to the latter, with a [Sieve][] rule that knocks any mail addressed only to my old email address into a "legacy" subfolder that I don't check as often as the inbox (so make sure you're sending mail to the new address if it's important that I see it):

```
### Custom filing code
# file email into legacy that doesn't contain a modern address
if allof (
  address :is ["To","Cc","Resent-To","X-Delivered-To"] "stuart@testtrack4.com",
  not address :domain :is ["To","Cc"] "stuartpb.com"
){
  fileinto "INBOX.legacy";
}
```

[Sieve]: https://en.wikipedia.org/wiki/Sieve_(mail_filtering_language)

### Web content migration

I'm using FastMail's web hosting to serve the few static files that were previously available on testtrack4.com. Down the line, I'd like to have the text objects versioned through a Git-tracked repository, and the blobs (ie. images) served through a static blob CDN like S3. (This would actually be a pretty good use for the [spaspec][] I've been putting off working on for so long.)

[spaspec]: https://github.com/spaspec

## The WELL

Earlier this month, I re-read [Stewart Brand's Rolling Stone article on the First Spacewar Olympics from 1972][spacewar-article]: following the link on Stewart Brand from that has got me thinking that I might [join The WELL][], as it seems like it might be somewhere I could find some like-minded people who might be interested in some of this stuff I'm doing.

[spacewar-article]: https://github.com/stuartpb/spacewar-article
[Join The WELL]: https://www.well.com/join/

## Boring personal developments

I roasted some green coffee beans in a saucepan on Monday morning: they've tasted good, but I don't know if I'd describe the taste as being anything better than other whole beans I've bought pre-roasted. (I guess my intention in buying these beans green was that I was thinking they'd last longer? I don't know.)

I went down to my building's fitness center Thursday and did some weight lifting while catching up on Slow Burn (lifting 3-and-5 pound weights while not even working up a sweat). I did a bunch of crunches, thinking about how I was probably doing them insufficiently, as I was barely feeling anything and was barely moving: today, the muscles at the bottom of my ribcage hurt, so I probably just need to work on my horribly-emaciated abs.

In general, I ought to read up a little: it's not like excercise is an under-documented subject, and I really have no idea what I'm doing when I try it right now. I use fitness equipment right now the way I wrote web pages ten to fifteen years ago: having no idea what I'm doing, clumsily imitating a couple things I vagely remember seeing clips of, accomplishing barely anything, and grossly squandering the vast array of educational and material resources available to me.

My PC speaker started going off a lot tonight, so I pulled it off the motherboard for now. Next time I can power the system down, I'll take a closer look at the motherboard and see if I can figure out what's going wrong.

# Schedule

I'm generally available at any time Monday through Friday from noon to P6:00 Pacific time, with the exception of one fixed appointment on Wednesdays from P2:30-P3:30 Pacific time.

I'm going to be in Florida from 2018-02-03 to 2018-02-10, a trip that I scheduled completely forgetting [the SeattleJS talk on CouchDB I proposed two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38), which I had been scheduled to give on the 8th. I've just now realized this and posted that I'm not going to be able to make that appointment in that thread: we'll see how that develops in the interim.

Another presentation I almost attempted to give when I was out of town (before realizing and getting it moved down a month) is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
