# Chrome Web Store submission kit

Everything ready to paste. Three things I cannot do for you, marked **YOU**:
create the developer account, pay the fee, and click Publish. Creating accounts,
entering payment details, and accepting developer terms are off-limits for me
regardless of context, so those stay with you.

## Cost and scope

One-time **$5 USD**, charged **per account, not per extension**. All three
listings cost $5 total. Card payment only. One community report says MasterCard
and PayPal get refused while Visa works, but that is not in Google own docs, so
have a second card ready rather than assuming.

## Staying pseudonymous: the one setting that matters

**Declare Non-Trader.** That is the whole ballgame.

- **Traders** must submit legal name, phone number, and physical address, and
  Google **publishes all three at the bottom of the listing**.
- **Non-Traders** get a generic line reading "This developer has not identified
  itself as a trader". It names nobody.

So: Non-Trader, and set **Publisher Name** to `jju1s`. That field is free text
with no legal-name requirement for non-traders, and it is what appears under the
extension title.

What is NOT private, stated plainly:

- **Google knows who you are.** The account needs a verified email, mandatory
  2FA, and a payment card. Pseudonymity here means invisible to people browsing
  the store, not unknown to Google.
- **The GitHub link connects the dots.** The listing points at
  `github.com/Lrnssssss/carryover`, and that account owns other repos. For real
  separation the tool needs its own GitHub account.
- **Git history is already scrubbed.** Commits now show
  `123896289+Lrnssssss@users.noreply.github.com`, not your real address.
- **Close the hole permanently**: GitHub, Settings, Emails, then tick *Keep my
  email addresses private* and *Block command line pushes that expose my email*.

### One judgement call on Ko-fi

Trader status turns on whether you are acting for business purposes, and Google
publishes no ruling on whether donation links count. There is no official
guidance either way. The tip jar lives on the GitHub page, the site, and in the
extension UI, which is fine. The cautious move is simply not to repeat it in the
store listing description, so keep it out of there and let the linked site carry
it. It stays one click away either way.

## Names

Renamed to lower trademark risk. Google impersonation policy bans implying you
are endorsed by another company, and a bare "X for ChatGPT" is a known pattern
for both rejections and trademark complaints. Carryover now leads, the site name
is descriptive, and "unofficial" is explicit.

    Carryover - unofficial context handoff for ChatGPT     (50 of 75 chars)
    Carryover - unofficial context handoff for DeepSeek    (51)
    Carryover - unofficial context handoff for Grok        (47)

Use no logos, wordmarks, or brand colours from those companies anywhere in the
icon, screenshots, or promo tile.

## Short description (132 char limit)

    See how full your chat is getting, then carry its context into a new one. No account, no server, works fully offline.

## Category

    Productivity

## Detailed description

Write a genuinely different opening paragraph for each of the three. Do not
paste identical copy with only the site name swapped, because that is the shape
that gets flagged as keyword-stuffed.

    Long chats get slow and forgetful, and starting a fresh one throws away
    everything the model learned about your problem.

    Carryover puts a small pill in the corner of the chat showing roughly how
    many tokens the conversation has reached. Click it and the extension builds
    a handoff document out of the conversation already on your screen, copies it,
    and shows it to you in an editable box so you can trim it before pasting into
    a new chat.

    WHAT GOES IN THE HANDOFF
    - What you were working on: your first real message
    - Decisions and constraints: the lines that stated a choice, a rule or a
      correction, so the model does not re-suggest the approach you already
      rejected
    - Code and artifacts: code blocks, deduplicated, newest version kept first
    - Where you left off: the last few turns, verbatim

    THE SUMMARY IS EXTRACTED, NOT GENERATED
    There is no model call anywhere in this. The handoff is pulled out of the
    text already on the page using plain pattern matching. That means it works
    instantly and offline, and it cannot invent a decision you never made and
    carry that fiction into your next chat. The tradeoff is that it is blunt and
    keeps more than a human would, which is why it shows you the whole document
    before you paste it.

    PRIVACY
    - No network requests. No server, no API key, no analytics, no telemetry.
    - No declared permissions. There is no permissions key and no
      host_permissions key in the manifest.
    - No remote code and no dependencies. Two files, readable in a few minutes.
    - Your chat text is rendered as text, never as markup.

    HONEST LIMITS
    - The token count is an estimate from a character heuristic, not the real
      tokenizer. Expect it within about 15 percent. It is a fuel gauge, not a
      receipt.
    - The percentage is measured against a fixed assumed budget, because the page
      never states which model or plan you are on.
    - Images do not carry over. A turn that was an uploaded screenshot is marked
      so you can see something visual is missing.
    - Very long chats may be partly virtualized by the host page. Messages that
      are not in the page cannot be counted or carried.

    Free and open source under the MIT licence.
    Source: https://github.com/Lrnssssss/carryover

    Not affiliated with, endorsed by or connected to OpenAI, DeepSeek or xAI.

## URLs

    Homepage:        https://lrnssssss.github.io/carryover/
    Privacy policy:  https://lrnssssss.github.io/carryover/privacy.html
    Support:         https://github.com/Lrnssssss/carryover/issues

## Images still needed

- **Icon** 128x128, already in the zip
- **Screenshots** 1280x800, between 1 and 5, full bleed, square corners, no padding
- **Small promo tile** 440x280, **required**, submission will not go through without it
- Marquee 1400x560 is optional, skip it

## Privacy tab in the dashboard

A privacy policy URL is mandatory even at zero data collection. Leaving fields
blank is a rejection trigger, so fill every one.

- Single purpose:

      Carryover reads the conversation rendered on the current chat page in order
      to estimate its size and to compact it into a text handoff the user can
      paste into a new conversation. That is its only function. It makes no
      network requests and collects no data.

- Permission justification, if the field is required:

      This extension declares no permissions and no host_permissions. It runs a
      single content script on one site and reads only the page content already
      rendered there.

- Remote code: **No, I am not using remote code.**
- Data collection: declare **none** of the listed types, then tick all three
  certification boxes. All three are true here.

## Upload package

The store wants a zip whose **root** contains `manifest.json`, so zip the
*contents* of the folder, not the folder itself. The release zips are already
built that way.

    node build.js
    # dist/chatgpt, dist/deepseek, dist/grok

## Sequence

1. **YOU** register with the dedicated email, pay the $5, set up 2FA
2. **YOU** set Publisher Name to `jju1s` and declare **Non-Trader**
3. Upload ChatGPT, paste the fields, add screenshots and the 440x280 tile
4. Submit, then wait for approval
5. Only then submit DeepSeek, then Grok

Step 5 is deliberate. Review takes a few days normally and up to a few weeks
when Google is backed up. New accounts and new extensions already draw closer
manual review, and three near-identical listings landing at once from a brand
new account is the pattern reviewers associate with spam. Requesting zero
permissions works in your favour, since dangerous permissions are the main thing
that slows a review down.