# Right now (2018-02-12)

I just got back from a week-long trip to Florida. In the run-up to the trip, I'd been thinking I *might* pursue a few things described here while I was on vacation; I ended up not touching any of them, which I'm fine with (it was a vacation, after all). Now, I'm focusing on getting back into the swing of things.

One of the nights while I was down there, I had a talk that touched on some of the themes contained in [the Black Mirror pitch I started writing a few weeks ago][Let's Talk Tommy] (namely [parentification][]), and it's got me thinking that I should maybe revisit that aspect of the pitch, elucidating the problems therein in more detail.

[Let's Talk Tommy]: https://github.com/stuartpb/pitches-and-scripts/blob/master/tv-spec-scripts/black-mirror/lets-talk-tommy.md
[parentification]: https://en.wikipedia.org/wiki/Parentification

I'm planning on rewriting the README for [barfspace][] to better reflect how I'm currently holding it (as a space for unpublished drafts that may or may not be perpetually-unpublished, on a case-by-case and subject-to-change basis), rather than a manic allusion to the thoughts I had when I was creating / last reworking it (taking into account some of the understandings I've come to about my own discomfort with the bleeding-edge typing-before-thinking style I originally had in mind around it).

[barfspace]: https://github.com/stuartpb/barfspace

Still need to write about [the thoughts I had on a mechanism for providing extended browser support as I briefly flirted with in tracercore][3d11cd9]: that'll probably go in barfspace, at least as incubation until I've got a full, coherent statement explaining my thoughts.

[3d11cd9]: https://github.com/stuartpb/tracercore/commit/3d11cd930329336d120194f0e49646fa06323f4c

My plan to [convert Lean Notes from a series of Trello boards to a series of GitHub-Flavored-Markdown files][leannotes/leannotes#1] has kind of run out of steam for the moment. I think I'd rather try my hand at fully translating the Understanding Lua boards / org to GitHub first; I could have sworn I'd made a repo for it under https://github.com/dashseat, but I guess I must have opened the tab to do so and then ended up Tabalanching it away. (I should also think about making a repo there for Google Blocks data.) I'm going to see if I can port that content tonight (as it's only a couple of boards).

[leannotes/leannotes#1]: https://github.com/leannotes/leannotes/issues/1

I'm not quite ready to write about using Atom just yet: all I have to say about GitHub Desktop right now is that I've got [one major issue with it][desktop/desktop#3841], which I currently need to describe to the GitHubber who got roped into the issue via a typo (as they've had the only expression of interest in actually *understanding* the issue in the thread).

[desktop/desktop#3841]: https://github.com/desktop/desktop/issues/3841

## Unusual Studio

I've added/updates most of the projects I've undertaken in the last couple weeks to https://github.com/unusualstudio/unusualstudio-projects/ (which makes it more workable to cut mentions of them from this Planfile), but I still haven't made any progress on rendering the project data into an easy-reading page format. Finishing this is my top priority this week.

I'm still drafting [thoughts on the project schema][]: figuring out whether I want stage 3 projects to be separated out of the main list or not feels like it's probably the biggest blocker for me (as considering this is stopping me from adding things like my phone dock project described below, for instance).

[thoughts on the project schema]: https://github.com/unusualstudio/unusualstudio-projects/issues?q=is%3Aissue+is%3Aopen+label%3A%22model+%2F+schema%22

## 3D Printing

My Qidi Tech I has been shaking violently (or at least, violently enough to audibly rattle) on the X axis whenever it starts a new layer: I had been seeing X shifting in some of my prints, but had been attributing it to too-fast print speeds. After searching for [similar symptoms][] and finding people attribute this kind of shaking to faulty cables, I now think that this is probably being cause by some kind of brownout/undervolting in the supply of power (since it only happens for a few seconds after actuating the Z stepper). 

[similar symptoms]: https://www.3dhubs.com/talk/thread/grinding-noise-qidi-tech

I tried reconfiguring the power hookup (so that it's only going through one power strip), but that didn't resolve the issue, so I'm planning on emailing Qidi Tech support about this some time this week.

If I can get the issues with my printer sorted out, I want to resume work on [Project Araminta][] (the name I'd been searching for for the DIY-Harriet-Tubman-$20-bill project I've been working on, which I only realized shortly after posting my 2018-02-02 update). I want to try making a mold for the [stamp blocks][B001ASSAMG] that I bought: I'm also thinking about printing the stamp in a material with some woodfill (which might make it more porous and amenable to stamping, ie. a woodblock print), or reflowing the design to work as a stencil. (Another thing I did after posting the 2018-02-02 update was try printing the stamp entirely in PLA: it worked *even worse than the TPU stamps*, so that's a non-starter. I *might* try doing it again in ABS, but I wouldn't expect that much of a difference.)

[Project Araminta]: https://github.com/stuartpb/project-araminta
[B001ASSAMG]: https://www.amazon.com/gp/product/B001ASSAMG

No new work in [fiddly-bits][] on the piece to put over the broken hinge on my Brita pitcher lid - I'll probably be tackling it some time this week (as it has been a really annoying problem, the lid sliding off every time I tilt the pitcher to pour).

[fiddly-bits]: https://github.com/stuartpb/fiddly-bits/

I'm also working on printing [a usable holder for some portable silverware / chopsticks I got last week][alocs-clip]: the jitter in the model has been enough to make iteration on this infeasible, which is why this project is on hold until I can resolve that.

[alocs-clip]: https://github.com/stuartpb/stuartpb-loadout/tree/alocs-clip

I bought [some sticky pads][B06XBNBFLW] for [the desktop dock I made for for my phone][dockitall]: it's been working out really well, and I'm planning on making a note about this in the README at some point (maybe once I've licked this X-wobble issue and have printed a second iteration).

[B06XBNBFLW]: https://www.amazon.com/gp/product/B06XBNBFLW
[dockitall]: https://github.com/stuartpb/dockitall

When I tried to print [a couple calicats as gifts for my parents based on their own cats][custom-cats], I ended up running into problems with the machine code output by all the slicers I tried (Cura, for instance, ended up printing on entirely different sides of the build plate); since I was short on time, I ended up falling back to MakerWare, which did a lousy job (many of the finer details vanishing altogether in slicing), but at least produced *something*. At some point, I'd like to revisit this dual-extrusion issue and see if I can track down the precise point of failure to resolve the problem (though I'm probably not going to tackle this until I've worked out all the other problems described above).

[custom-cats]: https://github.com/stuartpb/custom-cats

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

I had a little trouble with the invite link (we had to go back and forth three times before it worked), but I've got my account set up now: once I've got a little room to breathe (hopefully tomorrow), I'll be logging on and checking out the conversation.

## Boring personal developments

I gained a *lot* of weight on vacation (like, nearly twenty pounds). It left me pretty depressed, through the weekend and into today. However, I've stocked back up on Keto-appropriate groceries, and am looking forward to doing the best I can to get back to where I was (and, next time I go on vacation, I'm not going to indulge *nearly* as much).

Just before I left, I got [a new router][TP-Link Archer AC1750] which supports faster 802.11ac speeds and I believe supports OpenWRT, should I ever choose to go that route (no pun intended): I'm planning on setting that up this week.

[TP-Link Archer AC1750]: https://www.amazon.com/gp/product/B00BUSDVBQ/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

# Schedule

I'm generally available at any time Monday through Friday from noon to P6:00 Pacific time, with the exception of one fixed appointment on Wednesdays from P2:30-P3:30 Pacific time.

I had been scheduled to give [a talk on CouchDB that I had proposed for SeattleJS two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38) on 2018-02-08, but ended up being out-of-town for: it's not clear what's going to happen there (the organizers never got back to me).

Another presentation I almost attempted to give when I was out of town (before realizing and getting it moved down a month) is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
