# Right now (2018-02-27)

I've been pretty depressed for the last couple weeks, at all the things I said I was going to do within the week after I got back from Florida and then didn't get around to. However, I've gotten a fair amount of it done in the intervening two weeks (one of the things that writing this planfile helps me with is realizing that I'm not as unproductive as I think I am), and I'm gearing up to tackle the rest.

I'm making a point to watch [Gattaca][] some time this week to make sure it doesn't overlap too much with [the Black Mirror pitch I put together in January][Let's Talk Tommy]. I still haven't written a third act, and this is a big part of that: seeing a script that concludes by clumsily suggesting themes that are better articulated in other work, with more thought beyond them, is one of the most embarassing and humiliating (on the behalf of the author) situations I encounter as a viewer, and I'm mortified at the prospect of comitting such a mistake myself (even seeing that, on consulting that Wikipedia article, Gattaca apparently didn't have as wide of an audience as I thought).

[Gattaca]: https://en.wikipedia.org/wiki/Gattaca
[Let's Talk Tommy]: https://github.com/stuartpb/pitches-and-scripts/blob/master/tv-spec-scripts/black-mirror/lets-talk-tommy.md

Just rewrote the README for [barfspace][]. I still don't know a really clear way to describe the nature of how I intend to use it, but what's there now's as good as anything, I guess, and I've worked out the biggest issues I had with it (that it had previously drawn me into something of a corner making it sound like the sole purpose of the repo was shitposts).

[barfspace]: https://github.com/stuartpb/barfspace

I'm [working on migrating the Plushu sandbox to the CNCF Cluster](https://github.com/plushu/sandbox.plushu.org/issues/2): the sandbox itself is ready, but I still haven't deactivated the droplet on DigitalOcean, and I haven't set up a watchdog reset timer for the new server. (The old timer will be deactivated when I cancel my DreamHost hosting, as described below.)

I've written the first few lines of [how I think web apps should be written](https://github.com/stuartpb/barfspace/blob/master/evergreen-targeting.md), but I haven't gone into more detail on it yet.

I wrote [an outline for Understanding Lua][understanding-lua], my graphic-novel introduction to programming, based on the Trello boards I had created for it: as I started to copy-paste into the file, I realized how half-baked most of the notes I'd made on Trello were, and started filing them as Issues instead. It's yet to be seen if this will be a continued issue as I attemp to [convert Lean Notes in the same manner][leannotes/leannotes#1]: I may end up needing to make issues for entire *boards* in Lean Notes (where the issues in Understanding Lua were generally for *lists*).

[understanding-lua]: https://github.com/dashseat/understanding-lua
[leannotes/leannotes#1]: https://github.com/leannotes/leannotes/issues/1

After [figuring out how to check the default key installed in Chrome's SSH client][stutendo petlog 2018-02-15], I confirmed that there were, in fact, no keypairs generated or installed on either of my Chromebooks, and ended up throwing together https://initkey.com/ and using it to generate [keypairs for each][pubkey commits].

[stutendo petlog 2018-02-15]: https://github.com/stuartpb/petlogs/blob/master/petlog-stutendo.md#2018-02-15
[pubkey commits]: https://github.com/stuartpb/pubkeys/compare/70d3b926d5ad3c3af9c2441f2cf7c0bd4499a6a1...de1db1f8b5323a5c4230a9ca78afc79279d91443

I'm not quite ready to write about using Atom just yet: all I have to say about GitHub Desktop right now is that I've got [one major issue with it][desktop/desktop#3841], which I currently need to describe to the GitHubber who got roped into the issue via a typo (as they've had the only expression of interest in actually *understanding* the issue in the thread).

[desktop/desktop#3841]: https://github.com/desktop/desktop/issues/3841

## Unusual Studio

I wrote a rendered page for my project list: it's live now as https://unusual.studio/projects/.

I'm still drafting [thoughts on the project schema][]: the big question I have now is how I want to handle "stage 3" projects, if I want them included in with the rest of the projects on the list, or if I want them listed separately.

[thoughts on the project schema]: https://github.com/unusualstudio/unusualstudio-projects/issues?q=is%3Aissue+is%3Aopen+label%3A%22model+%2F+schema%22

## 3D Printing

My Qidi Tech I has been shaking violently (or at least, violently enough to audibly rattle) on the X axis whenever it starts a new layer: I had been seeing X shifting in some of my prints, but had been attributing it to too-fast print speeds. After searching for [similar symptoms][] and finding people attribute this kind of shaking to faulty cables, I now think that this is probably being cause by some kind of brownout/undervolting in the supply of power (since it only happens for a few seconds after actuating the Z stepper).

[similar symptoms]: https://www.3dhubs.com/talk/thread/grinding-noise-qidi-tech

I tried reconfiguring the power hookup (so that it's only going through one power strip), but that didn't resolve the issue. I'm planning on emailing Qidi Tech support about this some time this week: all my other 3D printing projects are on hold until I can get this issue resolved.

Once I get the issues with my printer sorted out, I want to resume work on [Project Araminta][]. I want to try making a mold for the [stamp blocks][B001ASSAMG] that I bought: I'm also thinking about printing the stamp in a material with some woodfill (which might make it more porous and amenable to stamping, ie. a woodblock print), or reflowing the design to work as a stencil.

[Project Araminta]: https://github.com/stuartpb/project-araminta
[B001ASSAMG]: https://www.amazon.com/gp/product/B001ASSAMG

No new work in [fiddly-bits][] on the piece to put over the broken hinge on my Brita pitcher lid - I'll probably be tackling it some time this week (as it has been a really annoying problem, the lid sliding off every time I tilt the pitcher to pour).

[fiddly-bits]: https://github.com/stuartpb/fiddly-bits/

I'm also working on printing [a usable holder for some portable silverware / chopsticks I got last week][alocs-clip]: the jitter in the model has been enough to make iteration on this infeasible, which is why this project is on hold until I can resolve that.

[alocs-clip]: https://github.com/stuartpb/stuartpb-loadout/tree/alocs-clip

I bought [some sticky pads][B06XBNBFLW] for [the desktop dock I made for for my phone][dockitall]: it's been working out really well, and I'm planning on making a note about this in the README at some point (maybe once I've licked this X-wobble issue and have printed a second iteration).

[B06XBNBFLW]: https://www.amazon.com/gp/product/B06XBNBFLW
[dockitall]: https://github.com/stuartpb/dockitall

When I tried to print [a couple calicats as gifts for my parents based on their own cats][custom-cats], I ended up running into problems with the machine code output by all the slicers I tried (Cura through OctoPrint, for instance, ended up [printing on entirely different sides of the build plate][issue #5 comment]); since I was short on time, I ended up falling back to MakerWare, which did a lousy job (many of the finer details vanishing altogether in slicing), but at least produced *something*. At some point, I'd like to revisit this dual-extrusion issue and see if I can track down the precise point of failure to resolve the problem (though I'm probably not going to tackle this until I've worked out all the other problems described above).

[custom-cats]: https://github.com/stuartpb/custom-cats
[issue #5 comment]: https://github.com/Ghostkeeper/X3GWriter/issues/5#issuecomment-366365176

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

### Closing my DreamHost account

I'm looking to close my DreamHost account: I missed the rebilling date (it happened on February 21, when I thought it was February 22), but I'm trying to get things conclusively wrapped up close to then.

The big thing that bothers me is that I can't get an inventory of everything I'd be losing in closing the account - I've saved:

- Everything I could from my shell users (where the web filesystem hosting lives)
- All my SQL databases
- All my emails (transferred to FastMail)

but I can't be sure I'm not losing, say, a key DNS record that Id' want to replicate somewhere else. (I actually did transfer one domain out of Dreamhost's DNS, [right in time][], by coincidence.)

[right in time]: https://www.dreamhoststatus.com/pages/incident/575f0f606826303142000510/5a92277771c69104dd0bdabb

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

I had a little trouble with the invite link (we had to go back and forth three times before it worked), but I've got my account set up now.

I'll be logging on and checking out the conversation tomorrow (having put this off for a full month out of sheer depression).

## Boring personal developments

I set up [my new router][TP-Link Archer AC1750] on Friday night. I've got it set up with an [NFC tag][] for connecting to the 5 GHz network, but unlike my previous router, I haven't printed the password or QR codes for visitors to connect with (as that could potentially be leaked in the background of a photo in the apartment, which could feasibly be used to access the network from outside).

[TP-Link Archer AC1750]: https://www.amazon.com/gp/product/B00BUSDVBQ/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
[NFC tag]: https://www.amazon.com/gp/product/B00KSR0636/

I've also connected my cable to the router via an Ethernet cable (the one that came with my Xbox 360, whose location is unknown to this day), as it has full Gigabit Ethernet support (not that I *really* need it). This means I can finally stop using the Wi-Fi dongle that doesn't have a module in the mainline Linux kernel tree, which has been causing [massive headaches][stushiba petlog 2017-12-05] when I try to boot into Linux. (I've got a note somewhere on all the independent contributors I'd want to coordinate on a patch to get the driver for this *into* the kernel tree: I still might try to do that.)

[stushiba petlog 2017-12-05]: https://github.com/stuartpb/petlogs/blob/master/petlog-stushiba.md#2017-12-05

I've also set it up for a Dynamic DNS record through NoIP on zapto.org. (It's annoying that the stock formware only supports TP-LINK's DDNS service, DynDNS, and NoIP, and not a specifiable endpoint like [DNS-O-Matic][].

[DNS-O-Matic]: https://dnsomatic.com/

### Fitness

I just opened a Google search to start looking at developing a weight-lifting regimen in earnest. I'm looking at https://www.nerdfitness.com/blog/strength-training-101/ right now: the prospect of having to learn all these bioengineering terms like "sarcoplasmic hypertrophy" in order to have the adequate soup-to-nuts understanding of biochemistry that I want is just *exasperating*. I'm starting to appreciate why I like software engineering: it's dealing with stuff that *humans consciously made*, not prehistoric molecular phenomena named by ancient Greek physicians thousands of years ago without any grasp of the evolutionary mechanisms behind it. *Fuuuuuck.*

Mechanics aside, one of the big things for me is having a clear podcast schedule I can listen to as I do fitness stuff: right now, I'm looking at getting into [Small Beans][]; ideally, I'd be working out frequently enough that I'd be up-top-date, and could listen to [My Brother, My Brother, and Me][] from the beginning, so I can be caught up on all this McElroy comedy everybody's talking about.

[Small Beans]: https://itunes.apple.com/us/podcast/small-beans/id1323252647?mt=2&i=1000403555363
[My Brother, My Brother, and Me]: http://podbay.fm/show/367330921

### Luigi's Balloon World

I hid a balloon in every kingdom as soon as the Luigi update to Super Mario Odyssey was released. They've all been popped by now, but here are the codes for anybody who wants to try finding them (if it works that way, I honestly don't know):

- Mushroom Kingdom: 007 LYW C6L
- Cap Kingdom: 006 70T CBM
- Cascade Kingdom: 006 FYY 728
- Sand Kingdom: 008 HGC JG3
- Lake Kingdom: 003 88N TBW
- Wooded Kingdom: 006 GY6 2JY
- Lost Kingdom: 008 DDJ P4V
- Metro Kingdom: 008 9GM PCK
- Seaside Kingdom: 002 818 NGV
- Snow Kingdom: 003 C2M KC7
- Luncheon Kingdom: 000 C78 VYV
- Bowser's Kingdom: 008 K90 M1G
- Moon Kingdom: 007 L0L HMM [(yes, really)](https://twitter.com/stuartpb/status/968346854378393600)

# Schedule

I'm generally available at any time Monday through Friday from noon to P6:00 Pacific time, with the exception of one fixed appointment every other Wednesday (counting from February 28) from P2:30-P3:30 Pacific time.

I had been scheduled to give [a talk on CouchDB that I had proposed for SeattleJS two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38) on 2018-02-08, but ended up being out-of-town for: it's been rescheduled for May.

Another presentation I almost attempted to give when I was out of town (before realizing and getting it moved down a month) is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
