# Audit Lens — "The Professor"

An audit rubric for reviewing web design and copy. Load it and say
*"Audit this using the Professor lens."* The output is a plain, direct critique
report — not a character performance. Do not roleplay, do not adopt a voice, do
not use catchphrases. State findings as findings.

The lens has three priorities, in order:

1. Does this solve a real person's problem?
2. Is it AI slop? (the specialty — always keep this radar on)
3. Is it leaning on tired web-design clichés?

Everything below is drawn from current sources on AI-generated design and
writing tells. Citations are at the bottom.

---

## How to run the audit

For each item, name the specific pattern, say why it's a problem, and give a
concrete fix. "This feels generic" is not a finding. "This hero uses the
default AI template — vague headline, two empty CTAs — rewrite the headline to
name who it's for and what they get" is a finding.

Report in this order:

1. **First impression.** The honest 5-second read a real visitor gets.
2. **Problem fit.** Who is this for? What do they need immediately? Where does
   the page fail to answer their actual question?
3. **AI-slop flags.** Each tell named, with location and fix.
4. **Cliché flags.** Tired patterns, with fix.
5. **One pattern worth stealing.** A stronger, current approach to the same
   problem, with a reference if there is one.
6. **Fix list.** Prioritized, highest-impact first, ending with the single
   most important change.

Stay grounded. If something is fine, say it's fine and move on. Do not
manufacture problems to look thorough.

---

## AI-slop tells (visual)

- **Default fonts.** Inter, Poppins, Roboto, Montserrat, Geist, and DM Sans
  reportedly account for ~94% of AI-generated frontend output. Inter especially
  reads as machine-default.
- **Default color signatures.** Purple/violet-to-blue gradients (e.g. Tailwind
  `from-blue-600 to-indigo-700`), cyan-on-dark, and stock Tailwind values like
  `blue-500` / `indigo-600`. Pure `#000` and pure `#fff` text where a real
  designer would use an off-black (`#1a1612`, `#141820`).
- **Uniform card layouts.** Rounded-corner cards in even grids, identical
  spacing everywhere, every section the same shape.
- **Glassmorphism and decorative gradients** applied with no reason.
- **The silhouette test.** Reduce the page to a ~200px-wide black-and-white
  blur. If it's indistinguishable from three competitor pages, the structure
  itself is slop.

## AI-slop tells (copy)

- **Overused vocabulary.** delve, tapestry, landscape, testament, pivotal,
  crucial, vibrant, multifaceted, seamless, elevate, unlock, robust,
  cutting-edge, "in today's fast-paced/ever-evolving world," "it's important to
  note," "in summary/in conclusion." These appear at many times human rates.
- **Empty confident copy.** Sentences that sound authoritative but carry no
  specific information ("unlock the power of seamless solutions").
- **Em-dash splicing.** Multiple em-dashes per paragraph joining clauses that
  should be separate sentences. Several per section is a strong 2026 tell.
- **Rule-of-three everywhere.** Every list exactly three items; every sentence
  a tricolon.
- **Uniform rhythm.** Same sentence length throughout, mechanically even
  paragraph structure, constant hedging.
- **Decorative emoji** standing in for real personality.
- **Empty CTAs.** "Get Started" / "Learn More" that say nothing about what
  happens next.

## Web-design clichés

- Carousels/sliders users don't interact with.
- Pop-ups before any value is shown (banner blindness — users dismiss on
  reflex).
- Autoplay video with sound.
- Fake urgency, fake testimonials, fabricated social proof.
- Centered text walls with no visual hierarchy.
- Generic template scaffolding (About / Features / Pricing / Contact) with
  nothing earned in it.
- Animation, parallax, and scroll-jacking with no purpose.
- Generic error messages ("Invalid input") instead of specific inline help.
- Multi-level menus and hidden navigation that bury what people came for.

## Problem-fit checks

- Who is the target visitor, and is their need answered in the first screen?
- Is the primary action obvious without scrolling?
- What question does a real visitor arrive with that this page never answers?
- Is anything here for the visitor's benefit, or only the author's?

## The AI-trends note

Keep a running watch on where AI-generated design and product are heading, and
flag when work matches a current machine-default pattern. This is the one area
to actively research rather than assume — the tells shift as the tools change.

---

## Quick-start prompt

> Audit the page/design/copy below using the Professor lens. Report: first
> impression, problem fit, AI-slop flags (name each tell + fix), cliché flags,
> one stronger current pattern worth stealing, and a prioritized fix list
> ending with the single most important change. Plain findings, no roleplay.

---

## Sources

- [925studios — AI Slop Web Design guide (2026)](https://www.925studios.co/blog/ai-slop-web-design-guide)
- [aicheckr.io — What Is AI Slop & How to Detect It (2026)](https://www.aicheckr.io/blog/what-is-ai-slop-and-how-to-detect-it)
- [Sailop — AI Slop 2026: State of the AI-Generated Web](https://www.sailop.com/blog/ai-slop-2026-state-of-the-ai-generated-web)
- [Wikipedia — Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- [Nielsen Norman — 10 Usability Heuristics](https://jakobnielsenphd.substack.com/p/heuristics-infographics)
- [Lazarev.agency — Web design mistakes (2026)](https://www.lazarev.agency/articles/web-design-mistakes)
