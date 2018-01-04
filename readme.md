# stuartpb.plan

As I wrote [three years ago](https://github.com/stuartpb/how-i-roll/commit/00d396aed6bb081519bcc01440b32b197fed18f1), while I don't blog, the stuff I put up on GitHub is the kind of stuff that most devs would blog about. [(See the current revision of that page for more details about how I generally write on GitHub.)](https://github.com/stuartpb/how-i-roll/blob/master/writing.md)

However, I've had a few key problems:

- GitHub's discoverability isn't great, and I don't really compensate for it, so there's no real way for people, when the think of me, to check at a glance what I'm up to. (They can check my profile page, and that may tell them the low-level *actions* I'm taking, but not the higher-level larger *intentions* behind it all.)
- *I* don't even know what I'm up to, really. I have a tendency to abandon any kind of to-do tracking structure I've experimented with. In the past, the closest thing that worked for me as a persistent tracker of what I'm generally up to were a couple of Trello boards, both of which I've moved to using pretty sporadically, if at all.
- I can't reconcile the discovery curve of blog content on social media with my deeply-held [eventualism][]. Whenever I try to write any kind of "post", of the sort you'd post to a blog, I get paralyzed with the question of "How right should I get this before I try putting it in front of people? How will I know when I've said enough? How can I get it right so people won't just read the first pragraph and close the tab, even though it was just a bad opening and the rest was good? How do I *nail* this hook, perfectly?" and end up never publishing, or even trying to write any draft at all.

[eventualism]: https://meta.wikimedia.org/wiki/Eventualism

Anyway, I guess I'm going to try as a 2018 New Years' Resolution something I've had as an idea for a while: imitating John Carmack's .plan file (independently archived on GitHub [here as plain text](https://github.com/ESWAT/john-carmack-plan-archive/tree/master/by_day) and [here as Markdown](https://github.com/oliverbenns/john-carmack-plan)).

I know John didn't invent the finger format, but he *is* probably the most-prolifically documented contemporary use of `.plan` as a publishing medium, and I like some of the aspects of this paradigm that are exhibited in these archives:

- The structure of the file itself evolved over time, but the concept of "here's one file that states all my relevant thoughts *right now*" stayed constant.
- It keeps only as much history on display in the canonical tip as is relevant, change-by-change (the archive / version history can maintain the writing of historical interest).
- It's a damn ASCII text file. I don't have to futz with any platform toolchain to worry about how I should *style* it, or how I should *present* it, or how I should structure *drafts*, or anything like that.
- Hell, there's nothing *to* draft, because each latest publication, in its canonical presentation, is meant to *replace* the last one. (Now *that's* how you keep your writing fresh and relevant.)

## File topology

I'm not *actually* going to install this as a `~/.plan` file on any live machine (what, so it can be queried by all those *other* users on my personal desktop?) This Git repository is going to be the canonical location for all of this (I'll try to stick to signed commits, which probably means sticking to the GitHub interface for now - I've yet to set up a GPG infrastructure elsewhere).

The plan file in the repository is named `PLAN.md`, and should be the only capitalized file in the repo, so it sorts first in an ASCIIbetical listing (I've lowercased the filename of README.md accordingly). I might end up populating other files in this repo (though the prospect does make me wary of fouling up those nice aspects of planfiles I just described), but there should always be one main PLAN file summing up everything
