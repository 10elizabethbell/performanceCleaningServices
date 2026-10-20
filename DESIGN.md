---
name: Performance Cleaning Services
description: Newark homes and job sites, left spotless. A calm band site in the logo's navy and gold.
colors:
  gold: "#e2ae52"
  gold-2: "#ecc273"
  gold-ink: "#7a5310"
  navy: "#15294b"
  deep: "#0d1a33"
  ink: "#0d1a33"
  body: "#27354a"
  soft: "#4a5668"
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c8d4e6"
  line: "rgba(13,26,51,.12)"
  focus: "#2f5fa8"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 11.4vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(20px, 5.8vw, 26px)"
    fontWeight: 400
    lineHeight: 1.15
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.3
rounded:
  field: "10px"
  row: "20px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-wide: "40px"
  band: "64px"
  band-wide: "96px"
  stack-sm: "12px"
  stack-md: "16px"
  stack-lg: "28px"
  column-gap: "64px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  service-row:
    backgroundColor: "rgba(255,255,255,.07)"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    rounded: "{rounded.row}"
    padding: "16px 16px 16px 24px"
    height: "84px"
  arrow-circle:
    backgroundColor: "rgba(255,255,255,.12)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    size: "44px"
  arrow-circle-hover:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  step-number:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: Performance Cleaning Services

## Overview

**Creative North Star: "The Freshly Cleared Room"**

The page behaves like a room after the crew has left: a few large, plain surfaces, nothing left lying around, everything where you expect it. Full-bleed bands alternate off-white paper with two navies so each section is its own clean room, and the logo's gold is the one warm thing in it, used as a fill on the things you can press. Shapes are soft and borderless: pills, 20 to 24px rounded cards, tinted fields. There are no hairline frames, no photos and no ornament beyond the faint diagonal texture on the dark bands.

Density is low and phone-first. One column of large Cal Sans headings and 16px system body text, generous band padding (64px phone, 96px desktop), and one clear action per band. Desktop adds a second column and nothing else. Motion is a single bounce-in on the hero heading plus a 12px fade-up for what starts below the first screen; everything is readable at rest, without JavaScript, and under reduced motion.

This is Ellie's house calm band style (`~/.claude/skills/pitch-site/references/calm-photo-style.md`) coloured from this client's black-and-gold logo. The logo sits on black marble, but the page ground is never black: the black becomes navy and the marble becomes paper.

**Key Characteristics:**
- Paper, two navies and one gold; gold is a fill, never text on light.
- Full-bleed bands alternate light and dark; the deep band carries the line texture.
- One display face (Cal Sans, weight 400 only) over a system body stack.
- Borderless, soft shapes: pills, 20px rows, 24px cards, 10px tinted fields.
- Flat bands; shadows only on objects that float above them (logo badge, floating circle).
- The real logo badge appears twice: header mark and closing band.

## Colors

A cool navy-and-paper neutral system with one warm accent taken from the logo's gold.

### Primary
- **Logo Gold** (`gold`): the only accent. Primary buttons, step numbers, the floating circle, the hover/focus fill of arrow circles, text selection, and the last phrase of headings on dark bands (`.accent`). On light bands it appears only as a fill.
- **Bright Gold** (`gold-2`): primary button hover only.
- **Burnished Gold Ink** (`gold-ink`): gold as text or icon on light grounds, at 6.3:1 on paper. Phone icons, claim icons, tap-to-call hover.

### Neutral
- **Paper** (`paper`): page ground, header and the light bands. Also the `theme-color`.
- **Brand Navy** (`navy`): the hero, the estimate band, and the Facebook row card on paper.
- **Deep Navy** (`deep`): the services band and the footer, always with the line texture. Same value as `ink` by design: the darkest navy is also the text colour.
- **Ink** (`ink`): headings on light, text on gold, the selected chip fill.
- **Body Slate** (`body`): running text on light (11.5:1 on paper).
- **Soft Slate** (`soft`): ledes, step descriptions, hints, placeholders (6.9:1 on paper, 6.3:1 on field).
- **Card White** (`card`): the form card on the navy band.
- **Field Mist** (`field`): input and chip fills on the white card.
- **On-dark** (`on-dark`) and **On-dark Soft** (`on-dark-soft`): headings and running text on navy bands (on-dark-soft is 9.7:1 on navy, 11.6:1 on deep).
- **Hairline** (`line`): the one divider, between claim rows on paper.
- **Focus Blue** (`focus`): hover and focus outlines on form controls and focus rings on light grounds, deliberately distinct from the gold fill so a focused gold button still shows a ring.
- **Error Red** (`error`): inline error text and the error border of a field.

### Named Rules
**The Gold Is a Fill Rule.** Gold (`gold`) is never text on a light ground (it is about 2:1). Text on gold is always `ink`. When gold must be read on paper or white, use `gold-ink`.

**The Never Black Rule.** The logo's black becomes navy. No band, card or button uses black or a near-black outside the two navies.

**The One Warm Thing Rule.** There is one accent hue. Status colour (`error`) and the focus blue are functional, not decorative, and never fill a surface.

## Typography

**Display Font:** Cal Sans, self-hosted woff2 (with "Avenir Next", "Segoe UI", system-ui)
**Body Font:** system stack (-apple-system, BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial)

**Character:** Cal Sans is round, friendly and a little bold-looking at weight 400, which carries the "we do the hard work" voice without shouting; the system body keeps the running text native and fast on cellular in Facebook's in-app browser.

### Hierarchy
- **Display** (400, clamp(40px, 11.4vw, 80px), 1.02): the hero H1 only, white on navy, max 13ch, place in the heading.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): section H2s. `text-wrap: balance`.
- **Title** (400, 20 to 26px fluid, 1.15): service row names, claim rows, step titles (21px, 22px desktop), the Facebook row. Cal Sans.
- **Phone display** (400, clamp(30px, 9vw, 52px), 1): the closing tap-to-call number, with a gold-ink phone icon at 0.8em.
- **Label** (400, 17px, 1.2): form labels and legends, buttons (18px), the header phone (17px, 20px desktop), all in Cal Sans.
- **Lede** (400, clamp(17px, 4.6vw, 19px), 1.7): the sentence under a section heading, max 40ch. The hero promise is the same role at 17 to 20px, line-height 1.5, max 32ch (44ch desktop).
- **Body** (400, 16px, 1.7): running text. Inputs are 16px so iOS never zooms.
- **Small** (400, 14 to 15px): service row tags, "(optional)" hints, errors, the line under the submit button.
- **Wordmark sub-line** (600, 11px, 0.08em, uppercase, `soft`): "CLEANING SERVICES" under the "PERFORMANCE" wordmark in the header, echoing the logo's lockup. Not a general label style.

### Named Rules
**The One Display Face Rule.** Every heading, button, label and phone number is Cal Sans at weight 400; emphasis comes from size, not weight. Body text never uses Cal Sans, and no second body face is added.

**The Hero Only Bounce Rule.** Only the hero H1 animates letter by letter (each letter from translateX(50px), 1s cubic-bezier(.34,1.56,.64,1), 20ms stagger, plain heading restored on the last letter's animationend). No other heading animates its letters.

## Layout

A single centred container (max 1160px) with a 20px gutter on phones and 40px from 760px. Every section is a full-bleed band with 64px vertical padding (96px from 760px); the hero uses 56/68px (96/112px desktop).

Phones are one column throughout. From 760px the hero buttons sit side by side (min 240px each). From 1024px each band becomes two columns with a 64px gap: heading left and service rows right (1fr / 1.25fr); intro and Facebook row left with claims right; sticky heading left and the form right (1fr / 1.2fr); the logo badge left of the closing text; the three steps in a row (40px gap). The hero adds the logo badge as a 300px right column on desktop only.

Vertical rhythm inside a band uses 12px between rows, 16px between heading parts, 20px in the hero stack and between form fields, and 28 to 36px between a heading block and its list. Headings and ledes are measure-capped (heading block 640px, ledes 40ch). All tap targets are at least 44px; buttons are 56px tall.

## Elevation & Depth

Flat bands, tonal layering. Depth comes from the alternation of paper and navy, from translucent white panels on navy (service rows at 7% white, arrow circles at 12%), and from the white form card on the navy band. Shadows appear only on objects that physically sit above the page: the logo badge and the floating circle. Header, buttons, rows and cards cast none.

### Shadow Vocabulary
- **Badge lift, paper** (`box-shadow: 0 20px 40px -22px rgba(13,26,51,.55)`): the logo badge in the closing band.
- **Badge lift, navy** (`box-shadow: 0 30px 60px -28px rgba(0,0,0,.6)`): the desktop hero logo badge.
- **Float** (`box-shadow: 0 10px 28px rgba(8,20,42,.3)`): the floating circle.

### Named Rules
**The Only Things That Float Rule.** A shadow means the object is above the page. Surfaces that are part of a band (rows, cards, buttons, fields) stay flat; state is shown with fill and outline, never with a shadow.

**The Faint Lines Rule.** The deep navy band and the footer, and the hero, carry `repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`. Keep it at about 4% white or fainter so it never reads as lines through text. Paper bands are never textured.

## Shapes

Soft, borderless and round. Pills (999px) for buttons, chips and every circle (arrows, step numbers, the floating circle, the header mark). Rows and the Facebook card use a 20px radius; the form card and the logo badges use 24px; fields use 10px. Nothing has a visible border at rest except the ghost button's 2px light outline. The one divider is a 1px hairline between claim rows. Icons are stroked SVG line icons (2.2 to 2.6 stroke, round caps and joins), never glyphs or emoji.

## Components

### Buttons
Big, round and plain.
- **Shape:** full pill, 56px tall, 26px side padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** gold fill with ink text. Hover lifts to bright gold. Inside the form the primary button is full width and also takes a 3px focus-blue outline on hover and focus.
- **Ghost:** transparent with a 2px on-dark border at 70%, on navy only. Hover: full white border and a 10% white fill.
- **Press:** scale(.98). Transitions 0.2s on colour and border.
- **Count:** at most two per hero (one primary, one ghost). No Call button in the hero; the number stays in the header.

### Service Rows (signature)
Each row is the whole link on the deep navy band: Cal Sans title, a small on-dark-soft tag beneath, a 44px arrow circle at the right. Only the arrow changes: on hover and focus it fills gold with ink arrow; the row's own fill and outline do not change. Tapping a row pre-selects the matching chip in the estimate form. The same row shape on paper, filled navy, is the Facebook link.

### Claim List
Large Cal Sans claims on paper, each with a 40px gold-ink line icon, separated by hairlines. Not links, no arrows.

### Numbered Steps
Gold 48px number circles (CSS counter, Cal Sans 20px) beside a Cal Sans title and a soft-slate line. One column on phones, three across from 1024px.

### Chips
- **Style:** field-mist pill, 48px tall, ink 16px system text, 2px transparent border.
- **State:** hover takes a focus-blue border; selected fills ink with white text; keyboard focus is a 3px focus-blue outline offset 2px (a border alone is invisible on the ink fill).

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** white on the navy band.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none.
- **Internal Padding:** 20 to 32px fluid, 20px between fields.

### Inputs / Fields
- **Style:** field-mist fill, 10px radius, 2px transparent border, 52px min height (textarea 110px), 16px text, placeholder in soft slate. Labels above in Cal Sans 17px with a small "(optional)" hint.
- **Focus / hover:** the border turns focus blue. No glow.
- **Error:** border turns error red and stays red while focused; a plain-sentence message appears below. The field-mist fill is only 1.19:1 against the white card, so the label above and the 52px height carry the field's identity; do not lighten the fill further.

### Navigation
A paper header, not sticky: the round logo mark (44px, 52px desktop) with the uppercase "PERFORMANCE" wordmark and its sub-line on the left, and the tap-to-call number with a gold-ink phone icon on the right (hover gold-ink). Under 375px the icon drops. The footer is the deep textured band with the name, place and number and a single Facebook link (hover gold). There is no menu.

### Floating Circle (signature)
One 60px gold circle with an ink chat icon, bottom right inside the safe area. It slides in (translateY, 0.35s cubic-bezier(.2,.8,.2,1)) once the hero has scrolled away and hides while the estimate form is on screen; hidden, it is `tabIndex=-1` and `aria-hidden`. It currently links to the estimate form (`#ask`), not `sms:`, because texting is unconfirmed; when the owner confirms texts, its href becomes an `sms:` link. Never a bottom bar.

### Fade-up
Blocks marked to rise move up 12px and fade in over 0.4s ease-out as they enter. Only blocks that start below the first screen are hidden first; nothing waits at opacity 0 without JS or under reduced motion.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands (paper, navy, paper, deep textured navy, paper, navy) so each new section is obvious.
- **Do** use gold as a fill with ink on it, and `gold-ink` (#7a5310) whenever gold must be read on a light ground.
- **Do** colour only the last phrase of a heading gold, and only on dark bands.
- **Do** keep every heading, button and label in Cal Sans 400 and every paragraph in the 16px/1.7 system stack.
- **Do** show state with fill and outline: gold arrow fill on rows, focus-blue borders on fields, a 3px outline offset 3px for keyboard focus (gold on navy, focus blue on light).
- **Do** keep tap targets at 44px or larger and inputs at 16px or larger.
- **Do** keep motion to the hero bounce-in and the 12px fade-up, and drop both under reduced motion.

### Don't:
- **Don't** use a black ground anywhere; the logo's black becomes navy.
- **Don't** set gold text on paper or white, or white text on gold.
- **Don't** add borders, hairline frames or shadows to rows, cards, buttons or fields.
- **Don't** texture a paper band or push the line texture above about 4% white.
- **Don't** animate any heading letter by letter except the hero H1.
- **Don't** replace the floating circle with a bottom bar, or show it while the form is on screen.
- **Don't** add a second accent hue or a second body font.
