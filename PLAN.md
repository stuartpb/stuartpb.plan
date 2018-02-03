# Right now (2018-02-02)

Apologies that this iteration of my planfile kind of jumps around narratively: I'm in a bit of a rush and don't have time to really review and lay it out carefully. I'm getting ready for my flight to Florida tomorrow morning right now, which mostly means a *lot* of 3d-printing work. I'm writing this up so I can power my computer down and potentially fix the problem I'm seeing with my 3D printer right now (see "Boring personal developments" below): this is all part of a race against the clock to see how much I can get printed before I have to sleep / fly.

I'm working on [a couple calicats based on my parents' cats as a gift for them when I see them in Florida][custom-cats]: this is going to be the first thing I print if/when everything comes back on.

[custom-cats]: https://github.com/stuartpb/custom-cats

I'm also working on printing [a usable holder for some portable silverware / chopsticks I got last week][alocs-clip]: the jitter in the model has been enough to make iteration on this infeasible, which is why I'm focusing on doing this writeup and power cycling right now.

[alocs-clip]: https://github.com/stuartpb/stuartpb-loadout/tree/alocs-clip

I also want to print a rounded iteration on [my belt loop buckles][belt-loop-buckle.scad] before I head out (the current design isn't unimpeachable: I broke one of them sliding down a wall to sit down on Sunday). Doing so (as I have it planned) will require getting [millwork.jscad][] working, so that's going to be what I work on while iterations on the two projects mentioned above print.

[belt-loop-buckle.scad]: https://github.com/stuartpb/stuartpb-loadout/blob/master/belt-loop-buckle.scad
[millwork.jscad]: https://github.com/stuartpb/millwork.jscad

I bought [some sticky pads][B06XBNBFLW] for [the desktop dock I made for for my phone last week][dockitall]: it's been working out really well, and I'm planning on making a note about this in the README at some point (maybe once I've licked this X-wobble issue and have printed a second iteration).

[B06XBNBFLW]: https://www.amazon.com/gp/product/B06XBNBFLW
[dockitall]: https://github.com/stuartpb/dockitall

No new work in [fiddly-bits][] on the piece to put over the broken hinge on my Brita pitcher lid: that's something I'm planning to tackle when I get back from Florida (as it has ben a really annoying problem, the lid sliding off every time I tilt the pitcher to pour).

[fiddly-bits]: https://github.com/stuartpb/fiddly-bits/

I've gotten [my Harriet Tubman $20 bill stamp design][tubman20-stamp] to the point where it is, structurally, better than the one [Adafruit demonstrated but didn't release sources for][Adafruit article] (in that the portrait it uses has been manually traced, which should make it cleaner to stamp with): the big problem I've been having *now* is that the TPU I've been printing in hasn't really been transferring ink all that well. I bought [some stamp blocks][B001ASSAMG] that I'm looking to try, but I'm not sure how to heat them, or how they might deform / stick to a mold when heated: I'm also looking at trying a stamp printed wholesale in PLA/ABS, and/or a material with some woodfill (which might make it more porous and amenable to stamping, ie. a woodblock print).

[tubman20-stamp]: https://github.com/stuartpb/tubman20-stamp
[Adafruit article]: https://blog.adafruit.com/2017/10/12/turn-your-20s-into-tubmans-with-this-diy-3-d-printed-stamp-wired-adafruit-ustreasury-stevenmnuchin1/
[B001ASSAMG]: https://www.amazon.com/gp/product/B001ASSAMG

One of the things I did in the course of developing the Tubman stamp design is finally kick out https://tracercore.com/, a front-end to https://github.com/jankovicsandras/imagetracerjs, which seems to be the only really accessible open-source tracing algorithm out there today, and certainly the only one that can feasibly be used web-client-side (the potrace codebase sounds like an ancient Lovecraftian nightmare to integrate): there are lots of free vector tracers out there today, but they all upload a file to a remote black box that can't be relied upon for [SACRED][], so I wanted to have something I could depend on that was a little more SACRED-compliant. The implementation that's up there now is clumsy (there's no UI for scrolling past the viewport extents / scaling, and any nudge to the UI params blocks the main thread while the image re-traces), but it works as a functional baseline that improvements can be hacked on going forward.

[SACRED]: https://github.com/stuartpb/sacred-tenets

(A really dumb note: I was compelled to do this because I wanted to have my cash all Tubmanned out when I went to spend it, but then I realized "hey, aren't I increasing the chances of somebody refusing to take my money if I've got a stamp like this on *every single bill I hand them*?" So I'm not even going to be able to make as extensive use of this as I thought I would. Boo.)

I went through a *lot* of different approaches to importing the SVGs into OpenSCAD before I found the comment on GitHub about how OpenSCAD development snapshots handle experimental features; I almost ended up writing my own SVG-to-SCAD-polygon converter using [Paper.js][] (since all the Inkscape plugins and whatnot that I could find were *very* fragile, clunky, presumptuous, and/or broken altogether) before taking a second look at [OpenSCAD's SVG support][openscad/openscad#1740].

[Paper.js]: http://paperjs.org/reference/path/
[openscad/openscad#1740]: https://github.com/openscad/openscad/issues/1740

Still need to write about [the thoughts I had on a mechanism for providing extended browser support as I briefly flirted with in tracercore][3d11cd9].

[3d11cd9]: https://github.com/stuartpb/tracercore/commit/3d11cd930329336d120194f0e49646fa06323f4c

[b0328876]: https://github.com/unusualstudio/unusualstudio-projects/blob/ea2dc1fdfd611025b825120839aa5b59dc0e533e/projects/b0328876-0695-4750-8948-3852b5511ae6.yaml
[Adafruit article]: https://blog.adafruit.com/2017/10/12/turn-your-20s-into-tubmans-with-this-diy-3-d-printed-stamp-wired-adafruit-ustreasury-stevenmnuchin1/
[some thoughts to write up in sacred-tenets]: https://github.com/stuartpb/sacred-tenets/commit/a4baae577dc3c014cdb5641af20d138e1859377d

[leannotes/leannotes#1]: https://github.com/leannotes/leannotes/issues/1

I had a dream about Jimmi Simpson directing a sequel to *USS Callister* earlier this week, so I guess my subconscious isn't quite done chewing on [the Black Mirror pitch I started writing a couple weeks ago][Let's Talk Tommy].

[Let's Talk Tommy]: https://github.com/stuartpb/pitches-and-scripts/blob/master/tv-spec-scripts/black-mirror/lets-talk-tommy.md

I'm not quite ready to write about using Atom just yet: all I have to say about GitHub Desktop right now is that I've got [one major issue with it][desktop/desktop#3841], which I currently need to describe to the GitHubber who got roped into the issue via a typo (as they've had the only expression of interest in actually *understanding* the issue in the thread).

[desktop/desktop#3841]: https://github.com/desktop/desktop/issues/3841

I'm planning on rewriting the README for [barfspace][] to better reflect how I'm currently holding it (as a space for unpublished drafts that may or may not be perpetually-unpublished, on a case-by-case and subject-to-change basis), rather than a manic allusion to the thoughts I had when I was creating / last reworking it (taking into account some of the understandings I've come to about my own discomfort with the bleeding-edge typing-before-thinking style I originally had in mind around it).

[barfspace]: https://github.com/stuartpb/barfspace

My plan to [convert Lean Notes from a series of Trello boards to a series of GitHub-Flavored-Markdown files][leannotes/leannotes#1] has kind of run out of steam for the moment. I think I'd rather try my hand at fully translating the Understanding Lua boards / org to GitHub first; I could have sworn I'd made a repo for it under https://github.com/dashseat, but I guess I must have opened the tab to do so and then ended up Tabalanching it away. (I should also think about making a repo there for Google Blocks data.) I might take a moment to work on this at the airport tomorrow.

## Unusual Studio

I've added/updates most of the projects I've undertaken in the last couple weeks to https://github.com/unusualstudio/unusualstudio-projects/ (which makes it more workable to cut mentions of them from this Planfile), but I still haven't made any progress on rendering the project data into an easy-reading page format. I was thinking I would take care of this this week, but I ended up getting sucked into a hole with the Tubman stamp (and its peripheral projects) and some other personal endeavors (not mentioned here). This may or may not be something I take care of in my downtime in Florida: if not, it'll happen after I get back.

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

Last month, I re-read [Stewart Brand's Rolling Stone article on the First Spacewar Olympics from 1972][spacewar-article]: following the link on Stewart Brand from that got me thinking that I ought to [join The WELL][], as it seems like it might be somewhere I could find some like-minded people who might be interested in some of this stuff I'm doing.

[spacewar-article]: https://github.com/stuartpb/spacewar-article
[Join The WELL]: https://www.well.com/join/

Having had this note as a standing part of my Planfile for a few weeks now, I got this email yesterday:

> Stuart,
>
> Hi there! I saw your post on Github the other day mentioning that you were considering joining The WELL. I am one of the General Managers of The WELL and I'm writing to personally invite you to do so!
>
> You wrote that you thought it might be a place where you could find like-minded people, and I think you're absolutely right. As you probably know, we've been around for over three decades and have been the home of countless funny, creative, profane, intelligent, awesome people.
>
> I'd like to invite you to come by and look around - if you're interested, I'll send you a link that allows you to join for free for three months. Swing by, check it out, and hopefully you'll see that it everything you expected it to be, and more.
>
> Thanks,
>
> Christian Ruzich
> Co-GM of The WELL
>
>
> PS - I just looked at the Stewart Brand Rolling Stone article you posted - very cool! I just posted a pointer to it in The WELL's News conference, so be prepared for literally dozens of views...

I had a little trouble with the invite link (we had to go back and forth three times before it worked), but I've got my account set up now: once I've got a little room to breathe, I'll be logging on and checking out the conversation.

## Boring personal developments

My Qidi Tech I has been shaking violently (or at least, violently enough to audibly rattle) on the X axis whenever it starts a new layer: I had been seeing X shifting in some of my prints, but had been attributing it to too-fast print speeds. After searching for [similar symptoms][] and finding people attribut this kind of shaking to faulty cables, I now think that this is probably being cause by some kind of brownout/undervolting in the supply of power (since it only happens for a few seconds after actuating the Z stepper). The printer's currently plugged into a power strip that is, itself, plugged into a power strip (and a cheap one at that), so it wouldn't be too far outside the realm of believability.

[similar symptoms]: https://www.3dhubs.com/talk/thread/grinding-noise-qidi-tech

This could also explain why [my PC speaker started going off non-stop last week][speaker note], to the point where I had to yank it off the mobo pins. I'm getting ready to power down everything that's currently plugged into the power chain (I need to replace that power strip with one with an angled plug anyway, for space-making reasons), which is why I'm currently making all these notes on what I'm currently up to in terms of open windows on my desktop (so I can remember to resume them after I bring the system back up).

[speaker note]: https://github.com/stuartpb/stuartpb.plan/commit/9043b424be9c23b772f26464a8fee702abca821c#diff-0339565dcb963a3e7bde2a034a98195dR93

Fixing the X-wobble issue is one of the things that's been holding me off from printing [this robotic claw from Thingiverse][thing:1717809]: right now, I've only got a couple pieces, and they're real noisy-looking, so I didn't want to print any more until I could get the printer producing clean results, whatever it takes.

[thing:1717809]: https://www.thingiverse.com/thing:1717809

I [finally fixed a bunch of standing issues with my phone yesterday][stuixel 2018-02-01], after thoroughly screwing it up first. (This dive was partially inspired by me having ordered some USB-Micro-B-to-C converters, and wanting to see if they handled data properly, unlike the last pack I got from Amazon.)

[stuixel 2018-02-01]: https://github.com/stuartpb/petlogs/blob/master/petlog-stuixel.md#2018-02-01

I headed down to Renton on Saturday and got a few things from IKEA (including a nice Lack end table that my Qidi Tech I fits on, unlike the previous one I had that was *just a couple centimeters* too small - this was one of my theories about why I was seeing the aforementioned X axis wobble), as well as a Nintendo Switch from Best Buy - since I've got a lot of long plane rides ahead of me, and everybody's talking about how the two best games of 2017 were on the Switch.

So far, I've been loving Super Mario Odyssey: I'm looking forward to getting Breath of the Wild at some point in the future. (I'm too used to the Humble Bundle model of game acquisition, where you spend maybe $30 in a month and games just rain from the sky.) I might write more about my Switch next time I update this, though it feels a little conspicuous-consumption-y to talk about the $25 in accessories I bought for it (on top of the, like, *hundred* dollars I had to spend on just a couple games).

I also got [a new router][TP-Link Archer AC1750] which supports faster 802.11ac speeds and I believe supports OpenWRT, should I ever choose to go that route (no pun intended): I'll probably set that up once I get back from Florida.

Following my excusrion down to Renton, autoload on my Orca card bounced due to an expired payment method: they make you actually *call and talk to somebody* to rectify this (even *after you fix the payment problem*), which is ridiculous, and something really ought to be done. (I did end up resolving this, but I'm lucky to have the privilege to be able to make calls like that, especially when so many who *do* ride the bus *aren't* so lucky.)

[TP-Link Archer AC1750]: https://www.amazon.com/gp/product/B00BUSDVBQ/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

Didn't do any fitness stuff this week, which is disappointing, but I've had a lot of other really positive stuff going on this week (and I'm probably going to be pretty active in Florida - though I'll also probably be indulging a bunch, too), so I'm not too disappointed.

# Schedule

I'm in Florida from 2018-02-03 to 2018-02-10, a trip that I scheduled completely forgetting [the SeattleJS talk on CouchDB I proposed two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38), which I had been scheduled to give on the 8th. I've just now realized this and posted that I'm not going to be able to make that appointment in that thread: we'll see how that develops in the interim.

I'm generally available at any time Monday through Friday from noon to P6:00 Pacific time, with the exception of one fixed appointment on Wednesdays from P2:30-P3:30 Pacific time.

Another presentation I almost attempted to give when I was out of town (before realizing and getting it moved down a month) is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
