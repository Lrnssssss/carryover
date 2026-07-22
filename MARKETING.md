# Getting people to actually find it

The tool is finished. Distribution is now the whole job, and it is the harder
half. This is the order that costs least and returns most.

## The single biggest lever

Get it on the Chrome Web Store. Everything below converts maybe three times
better once "install" is one click instead of "download a zip, unzip it, enable
Developer mode, load unpacked." Every hour spent on outreach before the store
listing exists is an hour spent at a third of its value.

That is $5 and it is the only thing standing in the way.

## Tier 1: free, high intent, do these first

People here are actively looking for what this does.

**Show HN** on Hacker News. Post Tuesday to Thursday, roughly 9am US Eastern.
Then sit in the thread for three hours and answer every comment. A Show HN with
no author replies dies. Do not title it as a fundraiser and keep Ko-fi out of
the post entirely, their guidelines ban fundraisers by name.

**r/SideProject**, **r/coolgithubprojects**, **r/opensource** with the
Promotional flair. Drafts already written in `SHARING.md`. Post from an account
with real history, not a fresh one, or it gets filtered before anyone sees it.

**r/ChatGPT and r/OpenAI**, carefully and later. Millions of readers, heavy mod
scrutiny. Frame it as complementary to ChatGPT, never as a fix for how bad
ChatGPT is at long chats.

**Answer existing questions.** Search Reddit and Stack Overflow for people
asking "how do I continue a long ChatGPT conversation" or complaining about
context limits. Those threads already rank in Google and keep pulling traffic
for years. Answer the question properly first, mention the tool second, and only
where it genuinely fits. This is slow, unglamorous, and outperforms almost
everything else on this page over six months.

## Tier 2: directories, ten minutes each, permanent

Submit once, they keep sending small amounts of traffic and they help the store
listing rank:

- Product Hunt (schedule for 12:01am US Pacific, that is when the day resets)
- AlternativeTo, listed as an alternative to manual copy-pasting
- There's An AI For That, Futurepedia, Toolify
- awesome-chatgpt and awesome-chrome-extensions lists on GitHub, via pull request

## Tier 3: outreach to people with an audience

This works, but only if it is genuinely personal. A template blasted to fifty
channels gets zero replies and a spam reputation. Ten researched emails beat a
hundred generic ones, every time.

**Who to contact.** Not the million-subscriber channels, they ignore cold email.
Target 5k to 80k subscribers, people who make videos about ChatGPT workflows,
prompt engineering, AI productivity, or Chrome extensions. Newsletter writers are
even better: Ben's Bites, TLDR AI, and the smaller AI newsletters actively hunt
for free tools to feature and reply far more often than YouTubers.

**How to find them.** Search YouTube for "ChatGPT context limit", "ChatGPT long
conversation", "AI productivity extensions" and sort by upload date. Anyone who
made a video on that topic in the last six months has an audience with exactly
this problem.

**The rules that make it work:**

- Reference the specific video or issue, by name, in the first line. If you
  cannot, you have not researched them enough to email them.
- Say why *them* specifically, not why your tool is great.
- Keep it under 120 words. Shorter than feels polite.
- Send it as a gift, not a request. There is nothing to buy and no affiliate
  link, which is unusual and worth saying plainly.
- No follow-up more than once, and not within ten days.

### Email template, YouTuber

Subject: `free, no-signup extension for the context-limit thing`

    Your video on running out of context in long ChatGPT threads is what made me
    finally build this.

    It is a Chrome extension that shows how full the conversation is, then
    compacts it into a handoff you can paste into a new chat. The part I think
    you would care about: there is no model call. It extracts the lines that are
    already there, so it cannot hallucinate a decision you never made.

    No permissions in the manifest, no server, no account. MIT licensed, free,
    and it stays free.

    https://cig13zs.github.io/carryover/

    Not asking for a video. If it is useful to you personally that is already
    worth the email.

### Email template, newsletter writer

Subject: `free tool for the context-window problem, no signup`

    Carryover is a Chrome extension that shows how full an AI chat is getting and
    compacts it into a handoff for a new one. Works on ChatGPT, DeepSeek and Grok.

    Two things that make it different from the others in this space: the summary
    is extracted with pattern matching rather than generated, so it cannot invent
    anything, and the manifest declares zero permissions, so it cannot leak your
    conversations even in principle.

    Free, MIT, no account, no upsell.

    https://cig13zs.github.io/carryover/

    If it is not a fit, no reply needed.

## What actually decides this

Not the launch. The launch gives you a spike that decays in three days.

What compounds is the store listing ranking for "chatgpt context" and similar
searches, the Reddit and Stack Overflow answers that keep surfacing in Google,
and people telling each other. All three depend on the tool being genuinely good
and honest about its limits, which it is.

## On the donation side, realistically

Free tools convert to donations at something like 0.2 to 1 percent of active
users, and that is with the link visible. The Ko-fi link is in the popup, the
README, and the site, which is the right amount. Making it louder will not raise
the rate, it will only make the tool feel cheaper.

The realistic path to the $100/month goal is thousands of users, not better
placement of the button. Which means Tier 1 and the store listing are the
donation strategy. There is not a separate one.