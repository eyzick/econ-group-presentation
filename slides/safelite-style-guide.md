# Safelite presentation style guide

Version 1.1 · September 25, 2026

Use this guide when extending, revising, or adapting the MBA economics presentation **Performance Pay at Safelite Auto Glass**. It documents the existing design and gives agents practical rules for keeping new material consistent. It is a portable Markdown reference, not an installed agent skill.

Reference files, relative to this guide:

- [HTML deck](safelite-performance-pay.html): editable source, CSS, interaction logic, and presenter notes.
- [PDF deck](../pdf/safelite-performance-pay.pdf): reference for slide appearance.

Share all three files with another agent when possible. The guide can also serve as a standalone brief. The original uploaded case remains the authority for case facts.

## 1. Presentation brief

**Audience:** MBA students with an introductory understanding of economics.

**Purpose:** Help students make and defend a compensation decision using principal-agent theory, incentives, measurement, risk allocation, selection, and operational constraints.

**Tone:** Analytical, direct, approachable, and open to disagreement. Write as a case facilitator. Give competing choices a fair hearing and put the presenter's suggested conclusion in notes until after the class votes.

**Format:** A self-contained HTML deck and a matching landscape PDF. The current deck contains 21 slides with 58 minutes of scheduled activity, leaving about two minutes for transitions. Maintain approximately 18-22 slides and a 60-minute session unless the user changes the brief.

**Visual character:** Warm off-white canvases, deep navy type, muted teal evidence graphics, amber discussion cues, generous whitespace, and large factual headlines. Use dark navy slides for the opening, major conceptual moments, the quiz, and the final decision.

This is a classroom design, not official Safelite branding. Do not imply that Safelite or Harvard Business School endorsed it.

## 2. Color system

| Token | Hex | Intended use |
| --- | --- | --- |
| `--paper` | `#F7F4EE` | Default background |
| `--navy` | `#0C2C3C` | Headings, dark backgrounds, strong table rules |
| `--ink` | `#13212A` | Main body text |
| `--muted` | `#5B6B74` | Supporting text on light backgrounds |
| `--blue` | `#1F6F8B` | Primary evidence series, section labels, borders |
| `--sky` | `#79B8C8` | Secondary evidence series and connectors |
| `--amber` | `#F0AA3C` | Discussion accents, caution rules, quiz controls |
| `--coral` | `#D96055` | Income reductions, exposure, contrasting series |
| `--green` | `#438A72` | Favorable assessments and correct-answer emphasis |
| `--line` | `#CBD5D8` | Quiet table and section dividers |
| `--white` | `#FFFFFF` | Text on dark backgrounds and restrained fills |
| Light blue canvas | `#E8F1F3` | Conceptual and operating-model slides |
| Light amber canvas | `#FFF3DD` | Pair discussions and team exercises |

On dark backgrounds use `#C8D9DF` for secondary text, `#9ED4DF` for small section labels, and `#9CB1BA` for source notes. Use `#B87512` for amber-colored text on light backgrounds. Reserve bright amber primarily for fills and rules because small amber text is hard to read.

Limit each slide to its background, text colors, and one or two purposeful accents. Pair color with labels, letters, or line patterns. A red/green distinction must remain understandable without color perception.

## 3. Typography

Use this font stack throughout:

```css
font-family: "Avenir Next", "Helvetica Neue", Arial, sans-serif;
```

The reference renders in Avenir Next on the original machine. Other systems may choose a fallback and change line wrapping. Inspect the result on the export system. Do not fetch fonts from an external service merely to open the deck.

The following values reproduce the current HTML. Sizes are CSS pixels, not PowerPoint points.

| Role | CSS size | Line height | Treatment |
| --- | --- | --- | --- |
| Cover title | `clamp(44px, 5.3vw, 84px)` | `0.98` | Bold, tracking `-0.045em` |
| Slide title | `clamp(34px, 3.4vw, 57px)` | `1.03` | Bold, tracking `-0.035em` |
| Subheading | `clamp(22px, 1.8vw, 31px)` | `1.15` | Bold |
| Body | `clamp(18px, 1.42vw, 25px)` | `1.32` | Regular, selective bold |
| Large supporting sentence | `clamp(22px, 1.7vw, 30px)` | `1.34` | Muted |
| Hero number | `clamp(74px, 8.3vw, 138px)` | `0.88` | Weight 800, tabular numerals |
| Eyebrow | `clamp(15px, 1vw, 18px)` | Inherited | Uppercase, weight 700, tracking `0.12em` |
| Source note | `clamp(10px, .72vw, 13px)` | `1.2` | Quiet supporting reference |

Keep the title to one or two lines. Body text should remain readable from the back of a classroom. Some existing dense tables use smaller type; prefer fewer words or fewer rows in additions rather than copying that size as a default. Never put a caveat essential to interpreting a figure only in the small source note.

## 4. Canvas and spacing

- Use a 16:9 canvas. The PDF measures 960 × 540 points, approximately 13.333 × 7.5 inches.
- The current slide container uses `padding: 5.3% 6.5% 4.4%`. Reuse the CSS when matching the deck. CSS percentage padding resolves against the containing width; it is not a literal percentage of slide height.
- Align titles, section labels, main content, and source notes to a common left edge.
- Use a two-column gap of about 5.2% and a three-column gap of about 3.4%.
- Keep the source note along the bottom, clear of the content. Put the slide number at the lower right.
- Give a slide one dominant visual or comparison. Keep whitespace when it helps the audience concentrate.
- Use square corners and flat surfaces. Reserve circles for numbered process steps or simple category markers. The deck does not use photographic backgrounds, ornamental illustrations, or brand logos.
- Reserve boxes for meaningful alternatives, quiz answers, phases, and scenarios. Avoid turning explanatory slides into collections of dashboard tiles.

## 5. Reusable slide patterns

| Pattern | Composition | Existing reference |
| --- | --- | --- |
| Cover | Navy background, large white title, short amber rule, muted subtitle | Slide 1 |
| Opening poll | Light blue canvas, direct question, four A-D alternatives in a 2 × 2 layout | Slide 2 |
| Company context | Three large statistics and a small direct-labeled comparison | Slide 3 |
| Operating process | Four numbered stages, short labels, simple connectors | Slide 4 |
| Quantitative puzzle | One large figure or bar, visible caveat, discussion prompt | Slide 5 |
| Economic mechanism | Equation or concept at left, short explanations at right | Slide 6 |
| Chart explanation | Short text on one side, large chart on the other | Slide 7 |
| Contract comparison | Two phases with a single pay formula beneath them | Slide 8 |
| Worked example | Compact table paired with a large calculated result | Slide 9 |
| Pair discussion | Amber canvas, concrete categories, one decision prompt | Slide 10 |
| Tradeoff | Two balanced columns with parallel labels | Slide 11 |
| Calculation table | Clear assumptions, aligned amounts, coral for reduced guarantees | Slide 13 |
| Team exercise | Four short scenarios with a shared task | Slide 17 |
| Quiz | Navy canvas, one question at a time, A-D responses and reveal feedback | Slide 18 |
| Options matrix | Criteria down rows, choices across columns, explicit judgment labels | Slide 19 |
| Proposed redesign | Flat rows linking each provision to its purpose | Slide 20 |
| Final decision | Navy canvas, three equally prominent options, vote-and-defend prompt | Slide 21 |

Reuse a pattern when the content serves the same purpose. Do not force every slide into the same composition.

## 6. Writing and facilitation

Use concrete titles such as “The 30% guarantee cut is large in a household budget” or direct questions such as “Who controls each source of lost output?” Avoid generic headings such as “Unlocking potential.” Explain a concept with a case example before adding terminology.

Keep slide copy brief, usually about 35-75 words excluding source notes. Tables and exercises may need more. Put detailed interpretation, anticipated objections, and transitions in presenter notes.

Every discussion should have a specific task, a time limit, a response method, and a debrief. Useful formats include a vote, a pair discussion, allocating a shock to a responsible party, choosing a pay rule, or defending a contract. Avoid an unsupported “Thoughts?” prompt.

For a 60-minute session, build in a substantive interaction approximately every 5-8 minutes. Include time for students to think and answer. Preserve the current major stops unless the user requests different pacing:

| Stop | Minutes | Intended result |
| --- | ---: | --- |
| Opening diagnosis vote | 3 | Surface competing explanations for low output |
| Pair discussion on control | 4 | Separate worker actions from production constraints |
| Team exercise on four shocks | 4 | Design and defend a compensation rule |
| Five-question checkpoint | 5 | Test concepts and correct misconceptions |
| Final decision and revote | 7 | Connect the economic tradeoffs to a management choice |

The deck now includes 12 visible “Ask the room” prompts on slides 3, 4, 6, 7, 8, 9, 11, 12, 13, 14, 16, and 19. Each takes 20-30 seconds within its existing slide allocation. Slides 5 and 15 retain their existing discussion questions. The five longer stops above remain in place. Questions on slides 3, 11, 16, and 19 are optional if the class is behind schedule. Notes give a response method, likely answer, optional follow-up, and debrief. Sum all slide timings after any revision. Preserve roughly two minutes of transition flexibility.

Use `.has-question` for a slide with a quick prompt and `.ask-room` for its bottom question band. The band has a quiet top rule, a teal “Ask the room” label, a small duration, and a larger navy question. On dark slides the question is white. Keep the question concise and reserve the bottom area with `.has-question` padding. Never overlap the content or the source note. The timing includes student responses and debrief, rather than adding time to the session. Put optional status in the notes so the presenter can decide whether to ask the visible question aloud.

### Presenter-note pattern

Write notes for someone who did not author the deck. Include:

1. Time allocation and the concept students should take away.
2. A concise explanation or worked calculation.
3. The exact question to ask and the response method, where relevant.
4. Likely answers, a misconception to address, and a short debrief.
5. A transition to the next slide when needed.

Keep the recommendation in the final notes clearly labeled as a suggested synthesis. Students can defend other decisions if they account for the evidence and tradeoffs.

### Game conventions

Use four concise, plausible alternatives with one defensible correct answer for concept questions. Keep open management judgments in discussion polls. Give an explanation after each answer reveal. The current game suggests one point for the correct answer and another for the explanation, scored manually by the presenter.

The HTML checkpoint is a local classroom activity. It has no student-phone connection, automatic team scoring, Kahoot account, hosted game, or live leaderboard. Describe it as a “Kahoot-style checkpoint” unless a real Kahoot game has been created and verified. Provide a static question fallback for the PDF and an answer key in presenter notes.

## 7. Evidence and economic precision

Cite the primary case as:

> Hall, Brian J., Edward Lazear, and Carleen Madigan. *Performance Pay at Safelite Auto Glass (A).* Harvard Business School case 9-800-291, revised December 6, 2001.

Use short visible references such as `HBS case, p. 6` or `Calculated from Table 1, HBS case, p. 7; assumes 40 hours.` Use the printed page numbers. Cite line numbers only when a stable line-numbered source exists.

Separate case facts, calculations, hypothetical examples, conceptual diagrams, and recommendations through plain labels. Redraw selected evidence and paraphrase. Do not reproduce full case pages or lengthy copyrighted passages.

### Verified anchors for this presentation

| Case item | Value | Page |
| --- | --- | --- |
| Scale in 1993 | About 500 stores, more than 3,000 employees, about 1,000 installers including managers who installed | 1 |
| Market shares | Safelite about 12%, Harmon Glass about 6% | 1 |
| Mobile service share in 1993 | 44% of repairs and installations | 2, footnote 1 |
| Average output | 2.5 glass units per technician per day | 5 |
| Wrong-part incidence described in case | 10%-20% of the time | 5 |
| Experienced technician wage | $10-$12 per hour | 6 |
| Initial guarantee period | 12 weeks | 6 |
| Proposed guarantee reduction | Approximately 30% | 6, 9 |
| Sample worksheet week | $490 + $112.51 + $6.45 = $608.96 | 7, Table 1 |
| Sample hourly equivalent | $608.96 / 40 = $15.22, rounded | 7, Table 1 |

These anchors support the existing deck. Recheck the original case before changing their interpretation or adding new factual claims.

### Nuances agents must preserve

- The case ends with a rollout decision. It does not provide a measured post-rollout productivity effect. Any later empirical findings require a separate source and explicit labeling as later evidence.
- The sample worksheet is an earnings illustration, not typical realized pay. Its glass mix assumes five units per day plus additional work and sales.
- Glass units include more than windshields. The case's installation-time observation is not a full time-and-motion study of the average worker.
- The “remaining 5.5 hours” illustration does not establish 5.5 hours of shirking. Travel, preparation, waiting, errors, and customer problems also use time.
- Actual guaranteed PPP earnings follow `pay = max(piece earnings, guarantee)`. An additional unit raises take-home pay only once piece earnings exceed the floor, or if it takes the worker across that threshold. Label a simple straight piece-rate line as a component or conceptual comparison. Use a kinked curve when showing actual guaranteed pay.
- Lowering the guarantee changes the downside and the output threshold at which piece earnings determine pay. It does not itself increase the piece rate or the slope above that threshold.
- Piece rates vary with task and market. Do not treat one worksheet rate as a universal payment per windshield.
- Effort, selection, and operational improvements can all change observed average output. A before-and-after average alone cannot identify their separate contributions.
- Selection can remove low-output workers and also discourage skilled workers who value income stability. Avoid treating every departure as a productivity gain.
- Hourly pay insures the wage rate conditional on hours and employment. Seasonal layoffs or reduced hours can still create income risk.
- Quality penalties and credits are proposed contract choices. Discuss attribution, gaming, reporting incentives, and administrative cost when recommending them.

## 8. Charts, tables, and accessibility

Use native HTML tables and editable HTML/SVG evidence graphics. Give each chart a clear comparison, direct labels, units, and a source or assumption note. Right-align currency and use consistent precision. Show dollars to cents where cents matter, whole dollars for the illustrative guarantee table, and percentages consistently.

Keep table rules light, use a strong header rule, and emphasize a total with a heavier rule. Avoid decorative 3D effects, pie charts for close comparisons, and unexplained dual axes.

Conceptual graphics must say they are conceptual. For seasonal patterns without monthly data, prefer labeled high/low periods. If using illustrative bars, state visibly that their heights are schematic and do not imply measured differences between spring, summer, or fall.

Use semantic headings, table headers, button elements, descriptive labels, and keyboard access. Keep essential meaning available as text. Maintain visible keyboard focus on interactive controls and make answer feedback readable without relying on color.

## 9. HTML and PDF implementation

Maintain a portable HTML file with embedded CSS and JavaScript. The current file has no network dependencies. Keep slide content as editable text, not screenshots of slides.

Follow the existing structure:

```html
<section class="slide blue" data-title="Short navigation label">
  <div class="eyebrow">Topic or activity and duration</div>
  <h2>Specific subject, finding, or discussion question</h2>
  <!-- One main composition using the existing layout classes -->
  <p class="source">HBS case, p. X. Any necessary calculation assumptions.</p>
  <span class="slide-no">N</span>
  <aside class="notes">
    <p><strong>Time: 3 minutes.</strong> Explanation and facilitation guidance.</p>
  </aside>
</section>
```

Choose `.slide`, `.slide.blue`, `.slide.amber`, or `.slide.dark`. Exactly one slide should carry `.active` in presentation mode. Keep numbers, source notes, and notes synchronized after reordering slides.

Preserve the controls: arrows, Space, and Page Up/Down navigate; Home/End jump to first/last; `N` toggles notes; Escape hides notes. The URL hash identifies the slide. When changing keyboard handling, avoid intercepting keys needed by focused buttons or other controls.

The notes panel overlays the presentation canvas. It is visible to the audience if that window is projected. It is not a private presenter display. Use a separate notes reference or build a separate presenter view if requested.

For PDF printing, show all slides in sequence, set one 16:9 page per slide, remove browser headers and footers, and preserve background colors. Hide navigation, progress indicators, and presenter-note overlays. Replace live quiz controls with a static question layout. The slide PDF is an audience copy; it does not include the embedded presenter notes.

A revision that changes visible slide content should update both HTML and PDF. Keep the original files recoverable while preparing a replacement. Never edit synced files under `sources/`.

## 10. Review before delivery

- Verify all numerical claims, calculation assumptions, and case-page citations.
- Confirm the slide count and sum the presentation timings.
- Check all slides at presentation size for wrapping, clipping, font substitution, chart labels, and clear hierarchy.
- Render and inspect every PDF page. Confirm 16:9 pages, correct ordering, one page per slide, and no accidental blank pages.
- Test navigation, notes toggling, quiz reveals, and quiz progression in an available browser. If live interaction testing is unavailable, say so rather than equating syntax checks with a complete functional test.
- Ensure the source and audience-facing PDFs agree. Differences such as the static quiz fallback should be intentional.
- Deliver only relevant artifacts. Keep build files and temporary renderings separate.

## 11. Copyable brief for another agent

```text
Use the attached safelite-style-guide.md and Safelite HTML/PDF deck as the
design reference for the requested presentation work. Apply the documented
colors, typography, 16:9 layouts, evidence conventions, and discussion patterns.
Keep the presentation suitable for an MBA classroom and approximately 60 minutes
including interaction. Use the original Safelite case as the authority for facts.
Distinguish reported evidence from calculations, conceptual illustrations, and
recommendations. Preserve the economic nuances listed in section 7, especially
the guarantee threshold and the distinction between effort and selection.

Implement the requested changes in editable HTML with presenter notes and update
the PDF whenever visible slide content changes. Inspect every exported page and
test supported interactions. Report any material limitation accurately.

Requested change: [Describe the specific slides or content to create or revise.]
```
