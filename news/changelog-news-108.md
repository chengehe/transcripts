**Jerod Santo:**

What up, nerds? I'm Jerod and this is Changelog News for the week of Monday, August 19th, 2024.

If our Winamp/Napster [talk](https://changelog.com/friends/57) with Jordan Eldredge pushed your nostalgia buttons at all, then Ryan Finnie's [recreation](https://github.com/rfinnie/blockbuster) of Blockbuster Video's VHS insert (which is editable via SVG) should hit hard, too. I will link up the image and the repo in your chapter data and the show notes.

Be kind, rewind! Ok, let's get into this week's news.

**Break:**

**Jerod Santo:**

[Practices of reliable software design](https://two-wrongs.com/practices-of-reliable-software-design)

Chris Stjernlöf got nerd-sniped. Out of the blue, a friend asked him how he would build an in-memory cache, laying out a few design constraints. He couldn't not take the bait.

> In the process of answering the question and writing the code, I discovered a lot of things happened in my thought processes that have come with experience. These are things that make software engineering easier, but that I know I wouldn’t have considered when I was less experienced.

He jotted down eight practices that he's adopted with experience and used while writing a fast, small, in-memory cache. They are:

1. Use Off-The-Shelf
2. Cost And Reliability Over Features
3. Idea To Production Quickly
4. Simple Data Structures
5. Reserve Resources Early
6. Set Maximums
7. Make Testing Easy
8. Embed Performance Counters

A few of these I live by. A few of these I hadn't really considered. I imagine every experienced dev has a similar list floating around in their head. That'd be an aggregation project worthy of the effort...

**Break:**

**Jerod Santo:**

[Micro-libraries need to die already](https://bvisness.me/microlibraries/)

Ben Visness has had enough with the npm community's propensity to pull in micro-libraries to suit every need.

> Here is my thesis: Micro-libraries should never be used. They should either be copy-pasted into your codebase, or not used at all.
>
> However, my actual goal with this article is to break down the way I think about the costs and benefits of dependencies. I won’t be quantifying these costs and benefits, but I hope that by explaining the way I think about dependencies, it will be clear why I think micro-libraries are all downside and no upside.

"Micro" is a subjective measure, but Ben is talking about single function kind of libraries. The case study he uses is `is-number`, which certainly qualifies by any measure. I whole-heartedly agree with him. A saying I learned from years of producing [Go Time](https://gotime) comes to mind: "A little copying is better than a little dependency." ([src](https://www.youtube.com/watch?v=PAAkCSZUG1c&t=9m28s))

**Break:**

**Jerod Santo:**

[Harvesting, fishing, panning for gold](https://staysaasy.com/strategy/2024/08/18/harvesting-fishing-panning-for-gold.html)

I like this set of metaphors for how to think about bucketing challenges into different categories. Some problems are like harvesting:

> **Harvesting problems** have straightforward solutions and no shortcuts: You just get a big basket and pick every damn strawberry in the field. You solve these problems with pure perseverance, slogging away for weeks, months, or years until they are done.

> **Some problems are like fishing**. You know that there are fish out there in the ocean, but you don’t know exactly where. If a great fisherman knows where the hungriest fish are and how to set their lines just right, they might catch everything that they need in a few hours. Fishing problems can sometimes be solved shockingly fast by motivated teams with a bit of luck.

> **Some problems are like panning for gold** – going out to a river or stream where there might be gold, getting your pan out, and seeing if you can find traces of the shiny stuff in the sediment. If you find gold, you can become generationally successful – think of the massive moats created by Google Search or the AirBnB network.

If you can categorize the problem you're trying to solve into one of these buckets, applicable strategies become more clear.

**Break:**

**Jerod Santo:**

It's now time for Sponsored News!

[Supabase Launch Week 12 recap](https://supabase.com/launch-week)

Last week was [Launch Week 12](https://supabase.com/launch-week) for Supabase. Here's a recap of what they shipped:

**Monday:** They launched [postgres.new](https://postgres.new) - an in-browser Postgres with an AI interface.
**Tuesday**: Authorization for Realtime's Broadcast and Presence went public beta. You can now convert a Realtime Channel into an authorized Channel using RLS policies in two steps.
**Wednesday**: They shared 3 new announcements for Supabase Auth: Support for third-party Auth providers, Phone-based Multi-factor Authentication (SMS and Whatsapp) & new Auth Hooks for SMS and email.
**Thursday**: They released Log Drains so you can export logs generated by Supabase to external destinations, like Datadog or custom HTTP endpoints.
**Friday**: They released support for Wasm (WebAssembly) Foreign Data Wrapper. Now anyone can create a Foreign Data Wrappers (FDW) to allow Postgres to interact with externally hosted data and share it with the Supabase community.

That's a lot! Learn more about all of Supabase's Launch Week announcements [by following the link in the chapter data and newsletter](https://supabase.com/launch-week).

**Break:**

**Jerod Santo:**

[Inside the "3 billion people" National Public Data breach](https://www.troyhunt.com/inside-the-3-billion-people-national-public-data-breach/)

Troy Hunt:

> Usually, it's easy to articulate a data breach; a service people provide their information to had someone snag it through an act of unauthorised access and publish a discrete corpus of information that can be attributed back to that source. But in the case of National Public Data, we're talking about a data aggregator most people had never heard of where a "threat actor" has published various partial sets of data with no clear way to attribute it back to the source...
>
> I've been collating information related to this incident over the last couple of months, so let me talk about what's known about the incident, what data is circulating and what remains a bit of a mystery.

When Troy says he's been collecting info for a "couple of months", he's not kidding. This one goes deep. My summary of his summary: *it's a giant mess*. One important takeaway:

> there were no email addresses in the social security number files. If you find yourself in this data breach via HIBP, there's no evidence your SSN was leaked, and if you're in the same boat as me, the data next to your record may not even be correct... So, treat this as informational only, an intriguing story that doesn't require any further action.

**Break:**

**Jerod Santo:**

[Dasel: one data tool to rule them all](https://github.com/TomWright/dasel)

I like this pitch:

> Say good bye to learning new tools just to work with a different data format.
>
> Dasel uses a standard selector syntax no matter the data format. This means that once you learn how to use dasel you immediately have the ability to query/modify any of the supported data types without any additional tools or effort.

It's a lot like `jq`, but supports JSON, YAML, TOML, XML and CSV (with zero runtime dependencies). The only thing I can imagine that'd be better would be to use SQL instead. One less syntax for most of us to learn...

**Break:**

**Jerod Santo:**

That's the news for now, but also scan the Changelog Newsletter for more goodies, including: visual data structures cheat sheets, Go is my hammer, and everything is a nail, Steve Klabnik taking a stand against names, and data is just an added sense.

Oh, and did you know [Changelog++](https://changelog.com/++) members can now build their own custom feeds?! Feedback of this brand new feature has been overwhelmingly positive, and people have created 124 feeds already. So that's cool...

Have a great week! Leave us a 5-star review if you dig our work, and I'll talk to you again real soon.