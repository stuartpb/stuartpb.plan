# Right now (2018-01-16)

I've added most of my decent ideas (and a fair number of the middling-to-bad ones) from my Projects board into [unusualstudio-projects](https://github.com/unusualstudio/unusualstudio-projects) (see https://github.com/stuartpb/help-wanted#1). Down the line, I expect I'll probably add [my issues in lazyweb-requests](https://github.com/h5bp/lazyweb-requests/issues/created_by/stuartpb), too.

Right now, I'm distracted at a couple of works I'd put together in Trello that would work better as Markdown repos. I've got an idea how I'm going to [migrate Lean Notes][leannotes/leannotes#1], which I've just now created a repo for. (Thinking of a design for one of the tags set me off on a journey through various archives that I largely forgot I had.)

I'm also looking at migrating Understanding Lua, which I have a Trello org with a couple boards for, and I appear to have never documented as something I was interested in, anywhere.

I also got distracted earlier (searching my [list of Collected Writings][collected-writings] to see if I really hadn't made either of those into a repo yet) and re-read [Stewart Brand's Rolling Stone article on the First Spacewar Olympics from 1972][spacewar-article]: following the link on Stewart Brand from that has got me thinking that I might [join The WELL][], as it seems like it might be somewhere I could find some like-minded people who might be interested in some of this stuff I'm doing.

[leannotes/leannotes#1]: https://github.com/leannotes/leannotes/issues/1
[collected-writings]: https://github.com/stuartpb/collected-writings
[spacewar-article]: https://github.com/stuartpb/spacewar-article
[Join The WELL]: https://www.well.com/join/

## Email transition

I'm currently transitioning my email address from stuart@testtrack4.com (DreamHost) to s@stuartpb.com (FastMail).

I've got DNS for testtrack4.com going through Fastmail as the authoritative nameservers now (with all Fastmail's default DNS entries), meaning that I've got mail forwarding, but I've broken webhosting.

FastMail has a list of [Sieve][] rules that you can insert custom code into (paired with a UI to manage simpler "Discard", "Forward", and "Organize" custom rules), structured as (from top to bottom):

- `require` extensions
- [Slot #1 for custom code]
- `1. Sieve generated for save-on-SMTP identities`
- `2. Sieve generated for discard rules`
- `3. Sieve generated for spam protection`
- [Slot #2 for custom code]
- `4. Sieve generated for forwarding rules`
- `5. Sieve generated for vacation responses`
- [Slot #3 for custom code]
- `6. Sieve generated for calendar preferences`
- `7. Sieve generated for organise rules`
- `8. Sieve generated for pop-link filing`
- [Slot #4 for custom code]

[Sieve]: https://en.wikipedia.org/wiki/Sieve_(mail_filtering_language)

I've got this Sieve rule in slot #3 (so it takes precedence over any UI-defined "organize" rules) for sorting emails that don't exhibit an awareness of my address update:

```sieve
### Custom filing code
# file email into legacy that doesn't contain a modern address
if allof (
  address :is ["To","Cc","Resent-To","X-Delivered-To"] "stuart@testtrack4.com",
  not address :domain :is ["To","Cc","Resent-To","X-Delivered-To"] "stuartpb.com"
){
  fileinto "INBOX.legacy";
}
```

### Web content migration

Most of the web content on testtrack4.com consisted of images I hotlinked on various forums between 2006 and 2010. Most of the inbound links for this content are either themselves defunct (one of the forums many of these images were made for was Achewood's Assetbar) or hopelessly irrelevant (another was the Spamusement User Forums, which are, incredibly, [still around](http://spamusers.com/forums/), on a live system that still openly announces its most active point was on **Dec 11, 2007**). However, I *freaking hate* breaking links out of negligence, so I do want to migrate at least a *subset* of what was up there to a sustainable hosting solution going forward. (Probably the most-active inbound data on testtrack4.com was the list of backwards-compatible programs detected by Windows 7 that I drew up for [this Cracked article](http://www.cracked.com/article_18808_7-reasons-computer-glitches-wont-go-away-ever.html).)

Today, I recognize the importance of hosting images on dedicated block storage (and tracking main site content in a version control system like Git), and if I were to do it all again, I'd have used one (though 2006 was such a different landscape that I pretty much would have had to drag all of Amazon Web Services through a time portal with me, at which point one might rightfully question why this is what I decided to use said time portal *for*).

My current plan is to drag-and-drop the files and directories that I know have some lingering inbound references on the greater Web into FastMail's file storage (there are some PHP installations and school projects that I don't feel like re-hosting) and use them to host testtrack4.com for now; more sustainably, I'd rather have some kind of hosting system where I can upload a map of old incoming filenames to redirect to a bucket like DreamObjects (which I've still got a gigabyte of free hosting with), alongside some versioned text content I can maintain like the aforementioned Windows compatibility list, and maybe a front page headstone explaining what testtrack4.com ever was / could be. (This would actually be a pretty good use for the [spaspec][] I've been putting off working on for so long.)

[spaspec]: https://github.com/spaspec

# Schedule

I'm generally available at any time Monday through Friday from noon to P6:00 Pacific time, with the exception of one fixed appointment on Wednesdays from P2:30-P3:30 Pacific time.

I'm going to be in Florida from 2018-02-03 to 2018-02-10, a trip that I scheduled completely forgetting [the SeattleJS talk on CouchDB I proposed two and a half years ago](https://github.com/seattlejs/seattlejs/issues/38), which I had been scheduled to give on the 8th. I've just now realized this and posted that I'm not going to be able to make that appointment in that thread: we'll see how that develops in the interim.

Another presentation I almost attempted to give when I was out of town, but instead moved forward a month, is a brief story I'm planning to tell at an Open Mic night in [The Royal Room][] in Seattle's Columbia City at P8:30 on 2018-03-08, about watching someone completely fail at [the Disney World version of *Who Wants to Be a Millionaire?*][WWTBAMPI] many years ago. This will be my first time going up on stage to give a completely non-technical monologue since at *least* high school, so if you're in the neighborhood, feel free to come down and watch.

[The Royal Room]: http://theroyalroomseattle.com/
[WWTBAMPI]: https://en.wikipedia.org/wiki/Who_Wants_to_Be_a_Millionaire_%E2%80%93_Play_It!
