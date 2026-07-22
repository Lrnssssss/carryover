# Where to share Carryover, and what to say

Not promo copy. The tool is free and MIT licensed, so these are written as
"here is a thing you can have" rather than a pitch. The Ko-fi link stays where
it already is, at the bottom of the README, and is never the subject of a post.

## The one rule that matters most

Every source agrees on this: a brand new or low karma account posting a launch
link on day one is the single most common reason these posts get removed, even
in subreddits that allow self promotion. Reddit now runs a sitewide Contributor
Quality Score on top of each subreddit's own karma and account age filters, so a
low score account can be silently filtered even where it passes the stated rules.

If the account you post from is fresh, spend a week leaving genuine comments
first. If you have an older account with real history, use that one instead.

## Ranked targets

| Where | Verdict | The condition |
|---|---|---|
| Hacker News, Show HN | Safe | Must not read as a fundraiser. Ko-fi stays in the README, never in the title or post |
| r/SideProject | Safe | Must link a working product, not a waitlist. Carryover qualifies |
| r/coolgithubprojects | Safe | Needs a real repo link, which it has |
| r/opensource | Safe with a condition | Use the "Promotional" flair. Frame it as "I open sourced this" |
| r/webdev | Narrow window | Only inside the weekly Showoff Saturday thread, and one source says 100+ karma and 30+ day account age |
| r/OpenAI | Careful | Keep self promo under about 10% of your posting history. Lead with the ChatGPT angle |
| r/ChatGPT | Careful | Case by case, 11.6M members so heavy mod scrutiny. Do not frame it as an alternative to ChatGPT, frame it as complementary |
| r/ChromeExtensions | Unverified | Rules could not be read. Check the sidebar yourself before posting |
| r/ChatGPTPro | Unverified | Same, check the sidebar |
| r/productivity | Avoid | Direct self promotion is removed despite the name suggesting otherwise |

## Show HN draft

Title:

    Show HN: Carryover – see how full an AI chat is, then move it to a new one

Body:

    Long chats get slow and forgetful, and starting a fresh one throws away
    everything the model learned about your problem. This is a Chrome extension
    that shows a running token estimate for the conversation on screen, and on
    one click builds a handoff document you can paste into a new chat.

    The part I care about: there is no model call. The handoff is extracted from
    the text already on the page with plain pattern matching, so it cannot
    hallucinate a decision you never made and carry that fiction forward. The
    tradeoff is that it is blunt and keeps more than a human would, so it shows
    you the document in an editable box before you paste it.

    The manifest declares no permissions and no host_permissions, and the code
    makes no network requests at all. It is two files and you can read the whole
    thing in a few minutes.

    Builds for ChatGPT, DeepSeek and Grok. MIT licensed.

    https://github.com/cig13zs/carryover

    Known limits are in the README rather than hidden: the token count is a
    character heuristic and lands within about 15%, the percentage is measured
    against an assumed budget because the page never says which model you are
    on, and messages virtualized out of the DOM cannot be counted.

## r/SideProject and r/coolgithubprojects draft

Title:

    I built a Chrome extension that shows how full your AI chat is and moves the context to a new one

Body:

    I kept hitting the point where a ChatGPT conversation got slow and started
    forgetting things, and every time I opened a fresh chat I had to re-explain
    the whole problem.

    So the extension does two things. A small pill in the corner shows roughly
    how many tokens the conversation has reached. Clicking it builds a handoff
    document out of the first real message, the lines that stated a decision or
    a constraint, the code blocks with the newest version kept, and the last few
    turns verbatim. Then it copies that and shows it to you in an editable box
    so you can cut what you don't need.

    No model call anywhere in it, which means it cannot invent a decision you
    never made. No server, no account, no telemetry, and the manifest declares
    zero permissions.

    Free and MIT licensed. Works on ChatGPT, DeepSeek and Grok.

    https://github.com/cig13zs/carryover

    Happy to hear where the extraction gets it wrong, that is the part most
    worth improving.

## Notes

Answer comments for the first few hours. On Show HN especially, being present
to discuss it is part of the norm and a thread with no author replies dies.
