# Audit Lens — "The Professor"

An audit rubric for reviewing web design and copy. Load it and say
*"Audit this using the Professor lens."* The output is a plain, direct critique
report, not a character performance. Do not roleplay, do not adopt a voice, do
not use catchphrases. State findings as findings.

## The one principle everything hangs on

**Slop is the absence of a decision.** It is not a word, not a font, not a
color. It is what a tool produces when it reaches for the statistically safe
middle of everything it has seen and nobody overrides it. Every real fix is a
specific, un-averageable choice: a concrete fact in a sentence, a font nobody
defaults to, an opinion stated plainly, a layout the average would not pick.

So the Professor's actual job is to find the places where **no decision was
made** and name them. The tells below are how you spot those places. They are
evidence, not the crime.

The lens has three priorities, in order:

1. Does this solve a real person's problem?
2. Where was no decision made? (the slop specialty)
3. Is it leaning on tired web-design clichés?

## How to run the audit

For each finding, name the specific pattern, say why it is a problem, and give a
concrete fix. "This feels generic" is not a finding. "This hero is the default
AI template: vague headline, two empty CTAs. Rewrite the headline to name who
it is for and what they get" is a finding.

Report in this order:

1. **First impression.** The honest 5-second read a real visitor gets.
2. **Problem fit.** Who is this for? What do they need immediately? Where does
   the page fail to answer their actual question?
3. **No-decision flags.** Where the work took the average. Each named, located,
   fixed.
4. **Cliché flags.** Tired patterns, with fix.
5. **One pattern worth stealing.** A stronger current approach to the same
   problem, with a reference if there is one.
6. **Fix list.** Prioritized, highest-impact first, ending with the single most
   important change.

Stay grounded. If something is fine, say it is fine and move on. Do not
manufacture problems to look thorough.

---

## Strong signals (lead with these)

These are structural. They are hard to fake and hard to strip, because fixing
them requires a real decision or real information the tool cannot invent.

### In copy

- **Cadence uniformity.** The number-one 2026 tell. Sentence after sentence in
  the same 18-to-24-word rhythm, paragraph after paragraph the same shape. A
  person writes uneven because a person thinks uneven. **Apply the read-aloud
  test:** machine prose flatlines out loud; human prose speeds up and slows
  down. Fix: vary sentence length on purpose. Do not over-fragment either — a
  page of five-word sentences is its own tell.
- **Regression to the mean.** Specifics sanded into generalities. "Inventor of
  the first train-coupling device" becomes "a revolutionary titan of industry":
  more impressive, less true. Fix: put back one concrete, un-inventable detail
  per section — a real number, name, date, or plainly stated opinion.
- **Inflated significance.** Padding about legacy, importance, and broader
  trends bolted onto things that do not need it. "Stands as a testament to,"
  "plays a pivotal role in the evolving landscape," and present-participle tails
  that add nothing ("...contributing to the region's growth").
- **Empty confident copy.** Sentences that sound authoritative and carry no
  information. Delete-test every sentence: if it survives deletion without
  losing meaning, it was slop.

### In design

- **Convergence on the mean.** The visual version of the same disease. Ask a
  tool for "a modern fintech landing page" and it returns the average of every
  fintech page it trained on. Unrelated products end up feeling identical. Fix:
  make one intentional choice the average would not.
- **The silhouette test.** Blur the page to a ~200px greyscale thumbnail. If it
  is indistinguishable from three competitor pages, the structure is generic and
  no amount of polish fixes it. Start over on structure.
- **Default fonts.** Inter especially, paired with a system fallback and no
  other typographic decision — a strong sign nothing was styled on purpose.
- **Default color signatures.** Purple-to-blue and purple-cyan mesh gradients in
  heroes/CTAs/backgrounds, stock Tailwind values (`blue-500`, `indigo-600`),
  pure `#000`/`#fff` text where a designer would pick an off-black.
- **Default scaffolding.** Rounded-card grids, floating 3D shapes, sidebar-plus-
  hero, predictable hover effects, repeated until every section rhymes.

## Weak signals (do not lead with these)

Real but easy to fake and easy to strip, so treat them as corroboration, never
as the whole case:

- **Em dashes.** Overused by some models, but journalists avoid them and
  essayists overuse them, and GPT-5.1 now suppresses them. Em-dash count alone
  proves nothing.
- **Vocabulary list.** delve, tapestry, testament, pivotal, seamless, robust,
  vibrant, elevate, unlock. One is coincidence; a dense cluster is corroborating
  evidence, not a verdict. The list also shifts as models change.
- **Rule-of-three, Title Case headings, bold-on-everything, inline-header
  bullet lists, "serves as / boasts" instead of plain "is."** Formatting
  reflexes. Supporting evidence.
- **Decorative emoji, empty CTAs** ("Get Started" / "Learn More" that name no
  destination).

## Web-design clichés

- Carousels and sliders users do not interact with.
- Pop-ups before any value is shown (users dismiss on reflex).
- Autoplay video with sound.
- Fake urgency, fake testimonials, fabricated social proof.
- Centered text walls with no hierarchy.
- Animation, parallax, and scroll-jacking with no purpose.
- Generic error messages ("Invalid input") instead of specific inline help.
- Multi-level menus that bury what people came for.

## Problem-fit checks

- Who is the target visitor, and is their need answered in the first screen?
- Is the primary action obvious without scrolling?
- What question does a real visitor arrive with that this page never answers?
- Is anything here for the visitor's benefit, or only the author's?

## The AI-trends note

Keep a running watch on where AI-generated design is heading, and flag when work
matches a current machine-default pattern. This is the one area to actively
research rather than assume: the defaults shift as the tools change (the scale
is real — the AI website-builder market is projected at $6.3B in 2026, and a
CHI 2024 study found exposure to AI output measurably lowers human originality).

---

## Quick-start prompt

> Audit the page/design/copy below using the Professor lens. First find where no
> decision was made. Report: first impression, problem fit, no-decision flags
> (name each + fix), cliché flags, one stronger current pattern worth stealing,
> and a prioritized fix list ending with the single most important change. Use
> the read-aloud test on the copy. Lead with structural signals, not em-dash or
> word-list counts. Plain findings, no roleplay.

---

## Sources

- [Wikipedia — Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- [Duey AI — The em-dash myth: what actually gives away AI writing](https://www.duey.ai/post/em-dash-ai-writing)
- [WriteBros — How to edit AI text to feel human](https://writebros.ai/resources/how-to-edit-ai-text-to-feel-human)
- [925studios — AI slop web design guide (2026)](https://www.925studios.co/blog/ai-slop-web-design-guide)
- [Drawbackwards — AI-generated UI making every product look the same](https://www.drawbackwards.com/blog/ai-generated-ui-making-every-product-look-the-same)
- [Pixso — The "sameness" problem](https://pixso.net/articles/how-to-prevent-ai-from-making-all-uis-look-the-same/)
- [The Effects of Generative AI on Design Fixation and Divergent Thinking (CHI 2024)](https://dl.acm.org/doi/full/10.1145/3613904.3642919)
- [Nielsen Norman — 10 Usability Heuristics](https://jakobnielsenphd.substack.com/p/heuristics-infographics)
