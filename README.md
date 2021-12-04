# seethrough
Monitor for inactivity, and keep the train going.

Idea inspired by John Kozubik's @ rsync.net [HN post](https://news.ycombinator.com/item?id=29436913): `Thanks! I will pass that along and see that it is "fixed" ... `

> and see that it is "fixed"

We can subscribe to a bunch of stuff, but we can't anti-subscribe.

In a leading position, or even as a support rep, where you've taken the responsobility to get a thing done, things can just die. A year later, you notice it, or the same person nags you 'uhh reporting this for the 3rd time'.

So, `seethrough` would be an attempt to monitor issues, mails, chat, whatever, that the case gets solved.

edit: so uhh, got lost, pretty much it will attempt to high-quality notify you when a thing you promised or want to see get done is not moving as you'd expect it to

Few features:
 - keep in touch?
   - usually when you'd anti-subscribe, you'd like to see progress (or foremost, no progress), with anti-subscribe; subscribing is probably possible via other (native) methods
   - this should be possible in a digest-like place: anti-subscriptions and (silent) subscriptions should collect to a place you access often
 - ignore non-relevant boops:
   - some are the comments of :+1:, that don't add something
     - others are actually good information, but the issue is still at a standstill, or moving way too slow
   - implementation of this is not really well possible ..uhh ML or something? ✨ AI
     - ignore actual comments as activity, and track only assignements, PRs and commits 'Closing' the issue somewhere, relation is not great either
       - this is not really possible in public repos, it's a problem gh has: you don't have any rights to manage the project / indicate labels or assignement, if you are not a member; giving sb member gives practically full access to the repo, not great

for gh: stalebot is pretty much already doing it

indeed, staledetector is kind of it (yet it can be dismissed by bops, and you can't only anti-subscribe).. except you can: by subscribing to repo's stale label with RSS (but that needs to be set up per-repo, and can't be global nor (anti-**subscribe**) issue-specific)
