# How to actually upload it, click by click

You have never done this before, so this is every step with nothing assumed.
Budget about 40 minutes for the first listing. The other two take 10 each.

Before you start, have ready:
- the `lrnsdc@gmail.com` Google account, with **2-Step Verification already on**
- a card that can take a $5 charge
- the file `dist/packages/carryover-chatgpt-1.0.0-store.zip`
- the folder `store-assets/chatgpt/` (3 screenshots + 1 promo tile)
- `STORE-SUBMISSION.md` open in another window, to copy text out of

---

## Part 1: create the developer account (once, $5, ~10 min)

1. Sign into Chrome with `lrnsdc@gmail.com`, or open an Incognito window and sign
   in there so you do not mix it up with your other Google account.
2. Go to **https://chrome.google.com/webstore/devconsole**
3. It will ask you to accept the developer agreement. Read it, tick the boxes.
4. It asks for a **publisher name**. Type `jju1s`. This is the name the public
   sees under your extension title. Do not put your real name.
5. It asks you to verify your email. Click the link it sends.
6. Pay the **$5 one-time fee** with your card. This covers your whole account,
   not one extension, so you never pay it again for DeepSeek and Grok.
7. Find the **account settings** page and look for the question about
   **trader status**. Choose **Non-Trader**.

   This step matters more than anything else on this page. Trader means Google
   publishes your legal name, phone number and home address at the bottom of
   your listing where anyone can read it. Non-Trader shows a generic sentence
   that names nobody.

---

## Part 2: create the listing (~25 min for the first one)

8. In the dev console, click **+ New Item** (top right).
9. It asks for a zip. Upload `carryover-chatgpt-1.0.0-store.zip`.

   Use the file with `-store` in the name. The other zip has everything inside a
   folder, which is right for humans loading it by hand but wrong here. Google
   needs `manifest.json` sitting at the top level of the zip or it rejects it.

10. It processes the zip and drops you into a form with tabs down the left:
    **Store listing**, **Privacy**, **Distribution**.

### Store listing tab

11. **Description**: paste the long description from `STORE-SUBMISSION.md`.
12. **Category**: choose **Productivity**.
13. **Language**: English.
14. **Store icon**: it usually picks this up from the zip. If it asks, the 128x128
    icon is inside the zip at `icons/icon128.png`.
15. **Screenshots**: upload all three PNGs from `store-assets/chatgpt/`
    (`01-pill`, `02-handoff`, `03-privacy`). They are already the exact 1280x800
    Google requires.
16. **Small promo tile**: upload `promo-440x280.png` from the same folder. This
    one is **required**, the form will not let you submit without it.
17. Skip the marquee tile, it is optional.
18. **Official URL / homepage**: `https://cig13zs.github.io/carryover/`
19. **Support URL**: `https://github.com/cig13zs/carryover/issues`

### Privacy tab

This is where most first submissions get rejected, purely for blank fields.
Fill in every one.

20. **Single purpose**: paste the single purpose paragraph from
    `STORE-SUBMISSION.md`.
21. **Permission justification**: you request no permissions, so there should be
    nothing to justify. If a box appears anyway, paste the permission paragraph.
22. **Remote code**: choose **No, I am not using remote code**. This is true, and
    lying here is an instant ban, not a rejection.
23. **Data usage**: tick **nothing**. The extension collects none of the listed
    data types. Then tick all three certification checkboxes at the bottom. All
    three are true for this extension.
24. **Privacy policy URL**: `https://cig13zs.github.io/carryover/privacy.html`

### Distribution tab

25. **Visibility**: Public.
26. **Regions**: all regions, unless you have a reason not to.

---

## Part 3: submit

27. Click **Submit for review** (top right).
28. Done. You will get an email when it is approved or rejected.

Review usually takes a few days and can take a few weeks when Google is backed
up. Because your extension asks for zero permissions, it should be on the faster
end. Nothing is public until they approve it.

---

## Part 4: the other two, AFTER the first is approved

Do not submit all three at once. A brand new developer account posting three
near-identical listings on day one is the exact pattern reviewers treat as spam.
Wait for the ChatGPT one to be approved, then repeat Part 2 with:

- `carryover-deepseek-1.0.0-store.zip` and `store-assets/deepseek/`
- `carryover-grok-1.0.0-store.zip` and `store-assets/grok/`

Rewrite the first paragraph of each description so the three are not identical
text. Copy-pasted listings with only the site name swapped get flagged as
keyword stuffing.

---

## If it gets rejected

You get an email saying which policy. It is nearly always one of:

- a blank field in the Privacy tab, so fill every box
- the description promising something the extension does not do
- the name implying you are official, which is why it is now called
  "Carryover - unofficial context handoff for ChatGPT"

Fix the thing named, click resubmit. A rejection is not a strike and it does not
count against your account.

## After it is live

Add the store link to the README, the site, and the release notes. Ask me and I
will do it in one pass.