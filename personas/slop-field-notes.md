# Field notes: what AI slop actually is (2026)

Research notes for the Professor. The goal is to replace the lazy version of
slop-detection ("count the em dashes, ban the word delve") with what current
sources actually say holds up. Sources at the bottom.

## The correction I had to make

I was over-indexed on surface tokens. Em dashes and a banned-word list are the
weakest signals available, because they are the easiest to fake and the easiest
to strip. A journalist trained in AP style uses no em dashes and is human. A
Substack essayist uses them every other sentence and is also human. GPT-5.1 now
suppresses them on purpose. So "em dash = AI" is close to noise.

The signals that hold up are structural, and they are the same in prose and in
layout: **uniformity and genericness.** Not the vocabulary. The sameness.

## Writing slop — the signals that actually survive

**Cadence uniformity is the number-one tell.** Sentence after sentence landing
in the same 18-to-24-word rhythm, paragraph after paragraph the same shape.
Human writing varies its speed because a person thinks at different speeds. A
sharp point gets a short sentence. A qualification runs longer. The read-aloud
test catches this when silent reading misses it: machine prose flatlines out
loud.

**Genericness from regression to the mean.** The model reaches for the
statistically safe middle, so specifics get sanded into generalities. "The
inventor of the first train-coupling device" becomes "a revolutionary titan of
industry." The subject gets simultaneously more exaggerated and less specific.
This is the deepest tell and the hardest to fake, because the fix requires
information the model cannot invent.

**Inflated significance.** Padding about legacy, importance, and broader trends,
attached to things that do not need it. "Stands as a testament to." "Plays a
pivotal role in the evolving landscape." Present-participle tails that add
nothing: "...contributing to the region's growth," "...highlighting its
importance."

**Structural fingerprints** (from Wikipedia's field guide, which is the best one
that exists): rule-of-three on autopilot, Title Case Headings, bold-on-
everything, inline-header bullet lists ("**Durability:** unlike roasted
meats..."), negative parallelism ("not a mirror, but a portal"), and avoidance
of plain *is/has* in favor of "serves as / boasts / features."

**The fixes that work** (and that I am now applying to my own output):
1. Vary sentence length on purpose. Rhythm comes from variance, not from a low
   average. Do not over-fragment either; a page of five-word sentences reads as
   a 2014 listicle.
2. Add one concrete, un-inventable detail per section: a real number, a real
   name, a specific date, a plainly stated opinion.
3. Edit in passes: one for rhythm, one for specifics, a third read aloud.
4. Do not add *false* specificity to fake humanity. Implausible detail is worse
   than generic.

## UX / web-design slop — the same disease, visual form

**The mechanism is identical: convergence on the mean.** Ask a tool for "a
modern fintech landing page" and it returns the average of every fintech page it
was trained on. The output space compresses. Unrelated products (a healthcare
app, a finance app, a learning app) come out feeling the same.

**The visual fingerprints:**
- **Inter** as the default font, paired with a system fallback and no other
  typographic decision. This alone signals the design was never intentionally
  styled.
- **Purple-to-blue gradients** (and purple-cyan mesh gradients) in heroes, CTAs,
  and backgrounds. The "safe" choice learned from thousands of SaaS pages.
- **Rounded-corner card grids, floating 3D shapes, predictable hover effects,
  sidebar-plus-hero scaffolding.** Familiar patterns repeated until everything
  rhymes.

**The scale is real, not a vibe.** The AI website-builder market is projected at
$6.3 billion in 2026. More money into the tools means more sites converging on
the same look.

**"Design fixation" makes it self-reinforcing.** A CHI 2024 study found that
designers shown AI output produced work with lower fluency, variety, and
originality than a baseline group. Exposure to the AI's average pulls the human
toward it. The homogenization compounds.

**The fixes that work:**
1. Treat AI output as exploration, not execution. It is good for raw options a
   human then art-directs. It is bad as a finished page.
2. Make one intentional decision the average would not: a font that is not
   Inter, a palette that is not the purple gradient, a layout that is not
   hero-plus-three-cards.
3. Give the product a personality that fits *it*. A finance tool and a kids' app
   should not share a feeling.
4. The silhouette test still holds: blur the page to a 200px greyscale
   thumbnail. If it is indistinguishable from three competitors, the structure
   is generic and no amount of polish fixes it.

## The one idea under all of it

Slop is not a word list and not a color. Slop is **the absence of a decision.**
Every real fix is a specific, un-averageable choice: a concrete fact in a
sentence, a font nobody defaults to, an opinion stated plainly. The Professor's
job is to find the places where no decision was made, and name them.

## Sources

Writing
- [Wikipedia — Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- [Duey AI — The em-dash myth: what actually gives away AI writing](https://www.duey.ai/post/em-dash-ai-writing)
- [WriteBros — How to edit AI text to feel human](https://writebros.ai/resources/how-to-edit-ai-text-to-feel-human)

Web / UX design
- [925studios — AI slop web design guide (2026)](https://www.925studios.co/blog/ai-slop-web-design-guide)
- [Drawbackwards — AI-generated UI making every product look the same](https://www.drawbackwards.com/blog/ai-generated-ui-making-every-product-look-the-same)
- [Pixso — The "sameness" problem](https://pixso.net/articles/how-to-prevent-ai-from-making-all-uis-look-the-same/)
- [UX Collective — AI made everyone a creator, not a designer](https://uxdesign.cc/ai-made-everyone-a-creator-not-a-designer-e28deb6e603b)
- [The Effects of Generative AI on Design Fixation and Divergent Thinking (CHI 2024)](https://dl.acm.org/doi/full/10.1145/3613904.3642919)
