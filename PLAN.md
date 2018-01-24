# Right now (2018-01-20)

[Right now, Stuart is listening to Van Halen.](https://www.youtube.com/watch?v=YCcLNmOpN3A)

I woke up Friday morning in a fey mood and ended up spending a couple hours [writing a pitch and treatment for a Black Mirror premise][Let's Talk Tommy]. As so often happens, I got stuck on the third act: I'm hoping that inspiration will strike again in a few days so I can finish it. We'll see.

[Let's Talk Tommy]: https://github.com/stuartpb/pitches-and-scripts/blob/master/tv-spec-scripts/black-mirror/lets-talk-tommy.md

---

I've officially added all the pre-Stage-3 projects I care to add from my Projects board on Trello into [unusualstudio-projects](https://github.com/unusualstudio/unusualstudio-projects), plus [my issues in lazyweb-requests](https://github.com/h5bp/lazyweb-requests/issues/created_by/stuartpb) and some assorted repositories I've had lingering around for a while. Right now, I've got 99 projects in the Cloud9 workspace where I've been putting these together: I'm debating scrounging around for one more to make it an even hundred, versus just straight up shipping 99 Projects and just letting that stand.

As much as my next priority should be building the template renderer to list these projects on unusual.studio, the thing I've got my eye on next is [converting Lean Notes from a series of Trello boards to a series of GitHub-Flavored-Markdown files][leannotes/leannotes#1]. I've got some [neat tag images][leannotes tags] I drew up in anticipation of keeping the flavor of the labels from Trello, and I'm itching to put them to use.

I looked at a few of the boards earlier, and I'm realizing that I'm probably going to need to update some of these as I port them, so I realize that this probably isn't going to be a simple afternoon's work; that said, I'm looking to do at least a *few* conversions before building the Unusual Studio Projects list page. (I might also make a couple tweaks to the data structure, namely [renaming the "status" field to "remarks"][unusualstudio-projects#6].)

I'm also looking at migrating Understanding Lua, which I have a Trello org with a couple boards for, and I appear to have never documented as something I was interested in, anywhere. There are only a couple of boards under the org I made for that project, but this is an idea I've been thinking about for a while, and I'm anticipating another burst of sudden inspiration to come when I start working on it again (maybe including some prototyping of what I'm picturing for the Dashseat environment in Google Blocks), so I'm holding it with the same cautious interest as revisiting Lean Notes.

---

I'd held off on updating this for a few days because I'd been so busy on Wednesday and Thursday:

- I drew [a rough logo for Dashseat](https://github.com/dashseat/dashseat-artwork/blob/master/dashseat-icon.svg).
- I [came up with the "SACRED" acronym][SACRED] to describe the principles I consider essential to making a project that can really be built upon, and polished up the rough work I'd done earlier to create a pretty good start for [The SACRED Tenets of Foundational Architecture][sacred-tenets].
- I hit on a reformulation of the "GitHub Best Practices" I'd been blanking on into something that I could work with, and went on to fill several sections on: [The Biggest Mistakes I See People Make on GitHub][github-mistakes].
- I got the autocomitter in [barfspace][] [well-polished][autocommit history], and after some thrashing and mania, came to take a moment to develop a more mindful and meditative relation to that long-neglected project (a significant prefigure to the creation of this PLAN file).
- I resurrected some long-lost work from my old notebook's hard drive that I'd forgotten has been plugged into my desktop this whole time.
- I installed Atom and GitHub Desktop, which I'll probably talk about here in a little more detail the next time I've got a moment, because I've got some thoughts around them.

[SACRED]: https://github.com/stuartpb/sacred-tenets/issues/1
[sacred-tenets]: https://github.com/stuartpb/sacred-tenets
[github-mistakes]: https://github.com/stuartpb/github-mistakes
[barfspace]: https://github.com/stuartpb/barfspace
[autocommit history]: https://github.com/stuartpb/barfspace/commits/master/bin/autocommit.sh

---

A few days ago, I re-read [Stewart Brand's Rolling Stone article on the First Spacewar Olympics from 1972][spacewar-article]: following the link on Stewart Brand from that has got me thinking that I might [join The WELL][], as it seems like it might be somewhere I could find some like-minded people who might be interested in some of this stuff I'm doing.

[leannotes/leannotes#1]: https://github.com/leannotes/leannotes/issues/1
[leannotes tags]: https://github.com/leannotes/leannotes/tree/master/tags
[unusualstudio-projects#6]: https://github.com/unusualstudio/unusualstudio-projects/issues/6
[spacewar-article]: https://github.com/stuartpb/spacewar-article
[Join The WELL]: https://www.well.com/join/

## Email transition

I'm currently transitioning my email address from stuart@testtrack4.com (DreamHost) to s@stuartpb.com (FastMail). All emait to the former is directed to the latter, with a [Sieve][] rule that knocks any mail addressed only to my old email address into a "legacy" subfolder that I don't check as often as the inbox (so make sure you're sending mail to the new address if it's important that I see it).

### Web content migration

I'm using FastMail's web hosting to serve the few static files that were previously available on testtrack4.com. Down the line, I'd like to have the text objects versioned through a Git-tracked repository, and the blobs (ie. images) served through a static blob CDN like S3. (This would actually be a pretty good use for the [spaspec][] I've been putting off working on for so long.)

[spaspec]: https://github.com/spaspec

# Schedule

I'm generally available at any time Monday through Friday from noon to P6:00 Pacific time, with the exception of one fixed appointment on Wednesdays from P2:30-P3:30 Pacific time.

I'm going to be in Florida from 2018-02-03 to 2018-02-10, a trip that I scheduled completely forgetting [the SeattleJS talk on CouchDB I proposed two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38), which I had been scheduled to give on the 8th. I've just now realized this and posted that I'm not going to be able to make that appointment in that thread: we'll see how that develops in the interim.

Another presentation I almost attempted to give when I was out of town (before realizing and getting it moved down a month) is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
