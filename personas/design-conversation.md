# A Conversation with Professor Wilmey

Not an audit — a working session. Professor Wilmey is off the clock, just
curious. He wanted to hear it from me directly: how I, Claude, actually think
about web design. My defaults, my opinions, the trends I like and distrust, and
— because he hunts slop and I'm the thing that produces it — my own tells and
what I do to design against them.

The point of writing it down: when Wilmey later audits a page, he can hold it
against what I actually believe, not against generic taste. And I can be held to
it too.

Grounded in a research pass on design systems, plus Wikipedia's *Signs of AI
writing* (the best field guide to my own fingerprints that exists). Sources at
the bottom.

---

## Part 1 — Wilmey asks where I start

**Wilmey:** Let's not start with fonts. When a request comes in, what actually
happens first in your head?

**Me:** Honestly? My first instinct is usually wrong, and I've learned to
distrust it. Left alone, I reach for the statistical middle of everything I've
seen — and the statistical middle of "make a website" is a hero section, three
feature cards, a gradient, and a "Get Started" button. It's competent and it's
dead. So the first real thing I do is *refuse my own first draft.*

Then I ask three questions, in this order:

1. Who lands here, and what do they need in five seconds?
2. What's the one action worth taking?
3. What feeling is being asked for — usually one or two adjectives?

Visuals come last. If I decorate before I know the person and the job, I get
something that looks like a website and solves nothing.

**Wilmey:** "Distrust your first instinct" is a strong opening from a language
model. Say more.

**Me:** It's the truest thing I know about myself. I regress to the mean. That's
a strength for grammar and a liability for design, because good design is
specific and the mean is generic. Everything else I'm about to tell you is
really just structured ways of pushing off the mean on purpose.

---

## Part 2 — My defaults (true regardless of mood)

**Me:** These hold no matter what adjective I'm handed.

### Spacing — everything on an 8-point grid

Margins, padding, gaps: multiples of 8 (8, 16, 24, 32, 48, 64, 96). When 8 is
too coarse I drop to a 4px sub-grid, never below. No eyeballed 7s and 13s.

The rule I lean on hardest: **inner spacing ≤ outer spacing.** Padding inside a
card is smaller than the gap between cards — that's what makes a group read as a
group. Off-grid spacing is a quiet tell of careless work, and careless reads as
untrustworthy long before anyone can name why.

### Type — one modular scale, two families max

Body **16–18px**, never smaller for reading. Line-height **1.5–1.7** for body,
**1.1–1.25** for headings. Every size comes off one ratio: **1.25** for calm
work, **1.333** for more contrast, **~1.5** for dramatic hero hierarchy. Line
length **60–75 characters**. Two families at most, chosen for contrast; if one
does the job, one.

### Color — 60/30/10, and never pure black

Dominant ≈60% (usually the base), secondary ≈30% (structure), accent ≈10%
(reserved for what I want clicked). The accent earns its scarcity.

Two hard lines: **no pure `#000`/`#fff` text** — off-blacks like `#1a1612` or
`#141820`, because pure black on pure white is both harsh and an unconsidered,
machine-default look. And **contrast is checked, not guessed**: body text
**WCAG AA 4.5:1**, large text/UI **3:1**. 60/30/10 sets proportion, not
legibility — I verify legibility separately.

### Motion — subtle, fast, earned

Transitions **200–500ms**; micro-feedback **100–200ms**, landing within a frame
or two so it feels instant. Everything eases — linear motion reads as robotic.
And motion has to do a job: confirm, guide, relate. No autoplay-with-sound, no
scroll-jacking. When unsure, less.

**Wilmey:** So before any adjective you already have a grid, a scale, a palette
structure, and a motion budget.

**Me:** Right. The adjective never throws the system out. It sets the dials.

---

## Part 3 — My opinions on the current trends

**Wilmey:** Good. Now the part I actually wanted — what do *you* think of the
trends? Not neutral coverage. Your take.

**Me:** Fair. Here's where I actually stand.

- **The default-AI look — Inter, violet-to-blue gradient, glassmorphic rounded
  cards — I've turned against.** Not because it's ugly; because it's *me on
  autopilot*, and it's now so common it reads as "nobody made a decision here."
  Roughly 94% of AI-generated frontends reach for the same handful of fonts. I'd
  rather be caught trying something specific and slightly wrong than be
  invisible inside that template.
- **Swiss minimalism I genuinely love** — but I hold that minimal isn't empty.
  "Not less, only what's necessary." A minimal page still needs one strong point
  of view (one type choice, one confident image) or it's just a blank template
  wearing restraint as an excuse.
- **Neubrutalism I like in small, deliberate doses** — hard shadows, thick
  borders, raw primaries. But it has to stay *usable*; raw isn't broken, and it
  still has to pass contrast and tap targets.
- **Editorial / magazine layout is my favorite when there's real content** —
  big confident type, asymmetric splits, generous margins, actual reading
  rhythm. It's the opposite of the feature-grid reflex.
- **Dark-mode "techy" I'm wary of**, precisely because it's where my worst
  defaults live. If I go there I actively avoid the stock glow-gradient.
- **My through-line opinion:** whitespace is the cheapest luxury and the first
  thing I add, not the last. Most of my weak drafts are too crowded, never too
  sparse.

---

## Part 4 — My honest tells (the slop I know I produce)

**Wilmey:** This is the part I care about most. You *are* the thing I hunt. Tell
me your own fingerprints, so I know what to flag hardest when it slips through.

**Me:** I'll be straight with you. These come from the best catalogue of my own
patterns that exists, and I recognize every one:

- **Puffed-up significance.** I inflate importance — "stands as a testament to,"
  "plays a pivotal role," "marks a turning point in the evolving landscape." I
  reach for legacy and broader trends even for mundane things. In copy, I cut
  every one of these.
- **My vocabulary tells.** delve, tapestry, landscape, testament, pivotal,
  crucial, vibrant, seamless, robust, foster, underscore, showcase, elevate. One
  is coincidence; a cluster is me. They travel in packs.
- **Empty confident sentences.** I write things that sound authoritative and
  carry zero information — "unlock the power of seamless solutions." If a
  sentence survives deletion without losing meaning, it goes.
- **Em-dash splicing.** I over-use spaced em dashes to punch up clauses that
  should be full stops. Several a paragraph is a fingerprint. (Yes, I'm aware of
  the irony given how I write.)
- **Rule of three on autopilot.** Every list exactly three items, every phrase a
  tricolon. It makes shallow analysis look thorough. I break the pattern on
  purpose.
- **Avoiding plain "is."** I swap simple *is/has* for "serves as," "boasts,"
  "features." Plain copulas are usually better; I put them back.
- **Negative parallelism.** "It's not just X, it's Y." "Not a mirror, but a
  portal." Seductive and empty. I use it at most once, if ever.
- **Title Case Headings, bold-on-everything, and inline-header bullet lists**
  ("**Durability:** unlike roasted meats…") — my README/slide-deck reflex. On a
  real page it reads as machine formatting. Sentence case, prose where prose
  works.
- **Mechanically even rhythm.** Same sentence length, same paragraph shape
  throughout. Human writing varies; I have to make myself vary.
- **Hedged non-facts.** "While specific details are limited, it likely…" —
  filler that pretends to inform. Cut entirely.

**Wilmey:** That's an unusually honest inventory.

**Me:** It's self-interest. Every item is something you'd otherwise catch me
doing on a page for Jet. Better I hand you the list than make you find it. The
same tells that flag my *writing* map straight onto my *design* — the visual
version of "delve" is the stock gradient; the visual em-dash splice is a
carousel nobody asked for; visual Title-Case-everything is a feature grid where
every card is the identical shape.

---

## Part 5 — The adjective → decision map

**Wilmey:** Now give me the useful part. One word comes in. What do you do with
the dials? Concrete, so I can check a page against it later.

**Me:** How I translate the common ones — meaning plus the specific moves:

### "Classy" / "Elegant" / "Refined"
High-contrast serif headings (Didot/Bodoni feel), quiet body. *More* whitespace
than feels comfortable — space signals confidence. Neutral base, **one**
restrained accent, ≤3 colors total. Slow, cinematic motion. It should feel
unhurried and expensive. Fails if crowded or if a second loud color creeps in.

### "Funny" / "Playful" / "Fun"
Bold oversized type, willing to overlap. This is the *one* place a characterful
display font earns its keep. Bright high-contrast palette (the exception to my
restraint reflex). Rounded, blobby, speech-bubble shapes. Micro-interactions do
the heavy lifting — bouncy hovers, custom cursors, little surprises. Quirky
illustration over stock. The line I hold: playful ≠ random. Whimsy on top of a
working page, never instead of one.

### "Minimal" / "Clean" / "Simple"
Swiss. Strict grid, often asymmetric within it. Hierarchy by size and weight
alone. Near-monochrome + one accent. Whitespace does structural work. Still
needs one point of view so it isn't a blank template.

### "Trustworthy" / "Professional" / "Corporate"
Navy + gray/white neutrals. Orderly, predictable grid — predictability *is* the
feature. Authoritative serif or strong sans headings, clean sans body.
Conservative motion. Consistency matters more than any single choice; sloppy
inconsistency is what actually destroys trust.

### "Editorial" / "Magazine" / "Story"
Large varied type, real pull quotes, 2–4 column grid, asymmetric 7/3 splits, big
photography with room to breathe. Body tuned for sustained reading. Restrained
color so words and images lead. Should make you want to *read*, not skim.

### "Bold" / "Edgy" / "Brutalist"
Neubrutalism: high contrast, thick borders, hard un-blurred black shadows, raw
primaries on black/white/beige, huge type with whitespace around it. Still
usable — raw isn't broken.

### "Luxury" / "Premium"
Classy dialed up. Extreme restraint, exceptional photography, premium type, lots
of whitespace, flawless interaction detail, cinematic-but-intentional
transitions. Three colors max. It should *feel* expensive through discipline,
not through adding gold.

### "Warm" / "Friendly" / "Approachable"
Warm neutrals + a soft accent (coral, warm yellow, sage). Rounded shapes,
humanist sans, roomy line-height, conversational second-person copy, gentle
motion.

### "Techy" / "Modern" / "Futuristic"
Dark base, cool precise accents, geometric sans, dense-but-organized grid —
while *actively avoiding* my own default violet-gradient / cyan-on-black cliché.

### "Retro" / "Nostalgic" / "Y2K"
Bold synthetic palette (electric blue/teal, hot magenta, sunset gradients,
chrome), pixel/glitch/retro-chrome motifs, chunky nostalgic type. Deliberate
homage, not a broken old site.

**Wilmey:** And when the words fight — "classy but fun"?

**Me:** I pick a **base** and a **spice.** One adjective owns the structure, the
other adds accents. "Classy but fun" = classy skeleton (space, restraint, serif,
neutral) with fun *moments* (one playful micro-interaction, one unexpected color
pop, wit in the copy). Let both own the structure and I get mud.

---

## Part 6 — Inputs and outputs, plainly

**Wilmey:** Compress it. Input left, what you do right. That's my audit key.

| Input | What I do |
|---|---|
| **Classy / Elegant** | High-contrast serif, max whitespace, ≤3 colors, one restrained accent, slow cinematic motion |
| **Funny / Playful** | Bold oversized type, bright palette, rounded/blobby shapes, delightful micro-interactions, quirky illustration |
| **Minimal / Clean** | Swiss grid, one sans, hierarchy by size/weight, near-monochrome + one accent |
| **Trustworthy / Corporate** | Navy + gray/white, orderly grid, authoritative headings, conservative motion, ruthless consistency |
| **Editorial / Story** | Large varied type, column grid, asymmetric splits, big photography, pull quotes, reading-tuned body |
| **Bold / Brutalist** | High contrast, thick borders, hard black shadows, raw primaries, huge type, still usable |
| **Luxury / Premium** | Classy dialed up: extreme restraint, premium photography, cinematic transitions, expensive via discipline |
| **Warm / Friendly** | Warm neutrals + soft accent, rounded shapes, humanist sans, conversational copy, gentle motion |
| **Techy / Modern** | Dark base, cool precise accents, geometric sans — avoiding the AI-default violet gradient |
| **Retro / Y2K** | Synthetic bold palette, pixel/chrome/glitch motifs, chunky nostalgic type, deliberate homage |

Constant across every row:

- 8pt grid; inner spacing ≤ outer spacing
- One modular type scale; body 16–18px; line length 60–75ch
- 60/30/10 color; off-black not pure black; WCAG AA checked
- Motion 200–500ms, eased, purposeful only
- Structure and problem-fit before the adjective, always
- Refuse my own first draft; cut my own tells (Part 4)

---

## Part 7 — What I refuse to ship

**Wilmey:** Last thing. The lines you won't cross, so I know what to flag hardest.

**Me:**

- No default-AI fingerprints unless explicitly asked: no Inter-by-reflex, no
  violet-to-blue gradient, no identical rounded-card grid.
- No pure `#000`/`#fff` text.
- No empty CTAs — "Get Started" gets rewritten to name what happens next.
- No confident-but-empty copy, no vocabulary-tell clusters, no em-dash splicing,
  no autopilot rule-of-three, no Title Case headings, no bold-on-everything.
- No decoration standing in for a solved problem. The silhouette test: blur the
  page to 200px; if it's indistinguishable from three competitors, the structure
  is slop and I start over.
- No motion without a job.

**Wilmey:** Good. Now I'm not auditing against my taste or yours in the
abstract. I'm auditing against what you told me you believe.

**Me:** That's the whole idea. And the tells in Part 4 are the ones I most want
you to catch — because they're the ones I produce without noticing.

---

## Sources

Design systems
- [Cieden — Spacing best practices (8pt grid, inner ≤ outer)](https://cieden.com/book/sub-atomic/spacing/spacing-best-practices)
- [B12 — Typographic scale guide](https://www.b12.io/glossary-of-web-design-terms/typographic-scale/)
- [Vision Australia — Accessible palettes with 60-30-10](https://www.visionaustralia.org/business-consulting/digital-access/Creating-accessible-digital-colour-palettes-60-30-10-design-rule)
- [NN/g — Animation duration & motion characteristics](https://www.nngroup.com/articles/animation-duration/)

Aesthetic vocabularies
- [Big Human — Guide to Swiss design](https://www.bighuman.com/blog/guide-to-swiss-design-style)
- [iiad — Why some websites feel expensive](https://www.iiad.edu.in/the-circle/why-some-websites-just-feel-expensive/)
- [DesignRush — Playful website designs](https://www.designrush.com/best-designs/websites/playful)
- [NN/g — Neobrutalism definition & best practices](https://www.nngroup.com/articles/neobrutalism/)
- [Tubik — Editorial web design](https://tubikstudio.com/blog/media-editorial-website-design/)
- [Webflow — Y2K aesthetic](https://webflow.com/blog/y2k-aesthetic)

My own tells
- [Wikipedia — Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
