# Right now (2018-01-13)

I'm working right now on putting together a greater index of projects / ideas I'm working on / interested in as [unusualstudio-projects](https://github.com/unusualstudio/unusualstudio-projects) (sort of a lighter-weight successor to https://github.com/stuartpb/help-wanted). I'm structuring it as a directory full of YAML files describing each project, named by UUID.

I started by putting together [a few initial description files][ff2ec85] by hand, but it felt like a *major* slog, so I went ahead and wrote [a couple scripts][83e0c53] that should make transcribing these much easier.

[ff2ec85]: https://github.com/unusualstudio/unusualstudio-projects/commit/ff2ec8501e1de6c1aea396a78e443f7511051275
[83e0c53]: https://github.com/unusualstudio/unusualstudio-projects/commit/83e0c53d965938c7b17b69c3ce0dcf514e0574ae

## Email transition

I'm currently transitioning my email address from stuart@testtrack4.com (DreamHost) to s@stuartpb.com (FastMail).

I've got DNS for testtrack4.com going through Fastmail as the authoritative nameservers now (with all Fastmail's default DNS entries), meaning that I've got mail forwarding, but I've broken webhosting.

Most of the web content on testtrack4.com consisted of images I hotlinked on various forums between 2006 and 2010. Most of the inbound links for this content are either themselves defunct (one of the forums many of these images were made for was Achewood's Assetbar) or hopelessly irrelevant (another was the Spamusement User Forums, which are, incredibly, [still around](http://spamusers.com/forums/), on a live system that still openly announces its most active point was on **Dec 11, 2007**). However, I *freaking hate* breaking links out of negligence, so I do want to migrate at least a *subset* of what was up there to a sustainable hosting solution going forward. (Probably the most-active inbound data on testtrack4.com was the list of backwards-compatible programs detected by Windows 7 that I drew up for [this Cracked article](http://www.cracked.com/article_18808_7-reasons-computer-glitches-wont-go-away-ever.html).)

Today, I recognize the importance of hosting images on dedicated block storage (and tracking main site content in a version control system like Git), and if I were to do it all again, I'd have used one (though 2006 was such a different landscape that I pretty much would have had to drag all of Amazon Web Services through a time portal with me, at which point one might rightfully question why this is what I decided to use said time portal *for*).

My current plan is to drag-and-drop the files and directories that I know have some lingering inbound references on the greater Web into FastMail's file storage (there are some PHP installations and school projects that I don't feel like re-hosting) and use them to host testtrack4.com for now; more sustainably, I'd rather have some kind of hosting system where I can upload a map of old incoming filenames to redirect to a bucket like DreamObjects (which I've still got a gigabyte of free hosting with), alongside some versioned text content I can maintain like the aforementioned Windows compatibility list, and maybe a front page headstone explaining what testtrack4.com ever was / could be. (This would actually be a pretty good use for the [spaspec][] I've been putting off working on for so long.)

[spaspec]: https://github.com/spaspec

# Schedule

I'm generally available at any time Monday through Friday from noon to 6:00 Pacific time, with the exception of one fixed appointment on Wednesdays from 2:30-3:30 Pacific time.

I'm going to be in Florida from 2018-02-03 to 2018-02-10, a trip that I scheduled completely forgetting [the SeattleJS talk on CouchDB I proposed two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38), which I had been scheduled to give on the 8th. I've just now realized this and posted that I'm not going to be able to make that appointment in that thread: we'll see how that develops in the interim.

Another presentation I almost attempted to give when I was out of town, but instead moved forward a month, is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
