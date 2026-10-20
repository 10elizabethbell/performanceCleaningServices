# Performance Cleaning Services — handoff at ~60%

**Live:** https://10elizabethbell.github.io/performanceCleaningServices/ · **Repo:** https://github.com/10elizabethbell/performanceCleaningServices · **Built:** 2026-10-20 from Muse brief (run 2026-10-20, Morris County Business Network ad)

## What's built
- One page, calm band style: header (logo badge + wordmark, tap-to-call 732-861-9697 top right) → navy hero → paper "We treat your place like our own" (Free estimates, Fully insured, big Facebook link) → deep-navy services (3 rows, each opens the form with its chip picked) → paper "How it works" (3 steps) → navy free-estimate form → paper close (logo, name, tagline, big number) → deep footer (name, Newark NJ, phone, Facebook).
- Palette from their black-and-gold logo: paper #f4f6fb, navy #15294b, deep #0d1a33, logo gold #e2ae52 as fills only, #7a5310 when gold is text on light. Cal Sans headings.
- Hero is the plain textured navy band (no usable photo, see gaps). On desktop (≥1024px) the real logo sits as a card on the hero's right.
- Motion: hero H1 letter bounce-in (waits up to 500ms for the self-hosted Cal Sans so letters don't swap font mid-bounce), `.rise` fade-up, floating circle (shows after the hero, hides over the form). All off under reduced motion and without JS.
- **Floating circle goes to the estimate form, not `sms:`**, because texting isn't confirmed and once the circle shows no call number is on screen. When the owner confirms texts, set its `href` back to an `sms:` link (DPG pattern).
- Form: job chips (optional), name (required), town and details (optional) → opens Messages with a pre-written text; "Rather talk? Call 732-861-9697" sits under the button, and a "didn't open?" line appears after submit.
- Favicon, iPhone icon and og:image (1200x630) made from their real logo.

## Assumptions I made
- **Texting works on 732-861-9697.** Not confirmed (brief: "Accepts texts: unknown"). The form opens a text, with the call number right under the button. If they can't take texts, change the form to show the composed message + call link.
- **Place = Newark.** Their Facebook page lists "Newark NJ" (page meta, 2026-10-20). The brief guessed Ocean/Monmouth from the 732 area code; the ads went to Morris County groups. H1: "Newark homes and job sites, left spotless."
- **"We" voice** (their posts say "let us"/"call us").
- Service sub-lines are mine: "New builds and remodels", "Homes, top to bottom", "Offices and businesses".
- Promise and care copy ("We leave every room ready to live in, work in or hand over", "We clean the dust and grime other crews leave behind") are written from the services; nothing factual is claimed beyond Free estimates and Fully insured.
- Primary name is the plural "Performance Cleaning Services" (their sign-off and logo); the FB page says "Service".

## Placeholders and gaps
- **No work photos.** The only image was a video thumbnail of a dirty tub (a "before" with no "after"), so it's not used. Hero stays the navy band.
- No email (footer has none), no owner name, no hours, no towns list, no reviews, no prices.
- Logo is the 720px FB profile image (marble background baked in); a vector or higher-res file would sharpen the close and og image.

## Questions for the owner
1. Can 732-861-9697 take texts?
2. Which towns do you cover? (Newark only, or Essex/Morris/Monmouth too?)
3. Before/after photos or the full video from the Halloween post (the tub)?
4. Owner's first name, and an email for the footer?
5. Hours, and do you do move-in/move-out or recurring cleans?

## Ideas not built (yours to pick)
- **Before/after slider** from the tub video (grab the last frame as the "after").
- **Seasonal line** like their ad: "Get the house ready before the holidays" eyebrow or banner, swapped by month.
- **Contractor angle:** a short "For builders and contractors" row (they post in NJ Construction Connection).
- Opt-in signature motion worlds, best first: (1) a hero you wipe clean: drag a cloth across a dusty navy surface and gold sparkles (from the logo) show through; (2) drywall dust that settles and clears as you scroll; (3) the logo's sparkles twinkling on hover over services; (4) a squeegee streak across the hero.
- Impeccable flagged, kept on purpose (Ellie's calm style): the eyebrow pills (craft floor bans them), the diagonal band texture ("repeating-gradient stripes", silenced for index.html in `.impeccable/config.json`), the fade-up on every block next to the bounce-in (floor wants one motion moment), the texture behind the H1 (3.5%, within the calm limit). Also left: a "flat type hierarchy" warning about the 14–18px small sizes.
- Applied from the finish review: wordmark selector bug ("Performance" was grey), no gold accent on the paper-band heading, form eyebrow now "Fully insured", Facebook row reads "Click to see our work on Facebook." (no "more": the page shows none), post-submit hides the duplicate call line, gold focus ring on the Facebook row, `aria-required` on name, smaller desktop hero logo.

## Not verified
- Real-device SMS handoff on iOS and Android (body encoding checked in Chromium; the text opens with "Hi Performance Cleaning Services, this is …").
- Inside Facebook's in-app browser on a real phone.
- Frame rate of the bounce-in on old phones.
- Form field fill (#e6ecf5, the skill's recommended value) is only 1.19:1 against the white card; fields are identified by their labels, but a darker fill or a 1px border would satisfy WCAG 1.4.11 strictly.
