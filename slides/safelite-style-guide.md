# Safelite presentation style guide

Version 2.2 · October 6, 2026 · Editorial design with whole-class discussion

Use this guide when extending, revising, or adapting the MBA economics presentation **Performance Pay at Safelite Auto Glass**. It documents the existing design and gives agents practical rules for keeping new material consistent. It is a portable Markdown reference, not an installed agent skill.

Reference files, relative to this guide:

- [HTML deck](safelite-performance-pay.html): editable source, CSS, interaction logic, and presenter notes.
- [PDF deck](../pdf/safelite-performance-pay.pdf): reference for slide appearance.

Share all three files with another agent when possible. The guide can also serve as a standalone brief. The original uploaded case remains the authority for case facts.

## 1. Presentation brief

**Audience:** MBA students with an introductory understanding of economics.

**Purpose:** Help students make and defend a compensation decision using principal-agent theory, incentives, measurement, risk allocation, selection, and operational constraints.

**Tone:** Analytical, direct, approachable, and open to disagreement. Write as a case facilitator. Give competing choices a fair hearing and put the presenter's suggested conclusion in notes until after the class votes.

**Format:** A self-contained HTML deck and a matching landscape PDF. The current deck contains 23 slides with 60 minutes of scheduled activity. Shorten optional questions to allow for transitions when the session must finish within an hour. Preserve the current slide count unless the user requests a change.

**Visual character:** Editorial serif headlines, large evidence figures, thin dividing rules, and a brighter classroom rhythm. Use white or pale blue for analysis, navy for the opening and final decision, cobalt for the first vote, guarantee reduction, and quiz, and lime for class discussions.

**Design reference:** McKinsey's December 2023 [Future of Work presentation to Indiana GWC](https://www.in.gov/gwc/files/McKinsey_Future-of-Work.pdf), especially PDF pages 3 and 4, informed the serif headlines, prominent numbers, blue palette, direct chart labels, and fine rules. No McKinsey text, images, logo, or proprietary typeface is reused. This is not a McKinsey-branded presentation.

This is a classroom design, not official Safelite branding. Do not imply that Safelite or Harvard Business School endorsed it.

## 2. Color system

| Token | Hex | Intended use |
| --- | --- | --- |
| `--paper` | `#FFFFFF` | Default canvas |
| `--navy` | `#071E32` | Headings, dark canvases |
| `--ink` | `#101F31` | Body text |
| `--muted` | `#506174` | Supporting copy |
| `--blue` | `#2455ED` | Cobalt evidence, poll, guarantee slide, quiz |
| `--sky` | `#92B6FF` | Secondary chart series |
| `--amber` | `#DDF96B` | Lime exercises, voting letters, correct answers |
| `--coral` | `#D73C55` | Contrasting risks |
| `--green` | `#087A64` | Favorable ratings and selected evidence |
| `--line` | `#CCD5E0` | Table and section dividers |
| Pale blue | `#F0F4FA` | Operating and conceptual slides |
| Warm cream | `#FFF7EC` | Munger/Hanoi analogy |

The legacy token name `--amber` now means lime. The guarantee slide uses white type and lime reduced-guarantee figures on cobalt. Dark-slide supporting text uses pale blue, with light source notes. Pair color with words or line patterns. The hourly-pay series is dashed, while PPP is solid.

## 3. Typography

Use Georgia with Times New Roman/serif fallbacks for titles and large figures. Use Avenir Next with Helvetica Neue/Arial/sans-serif fallbacks for supporting copy. Do not load external fonts.

Sizes below are CSS pixels on the 1280 × 720 canvas. The browser scales the entire canvas proportionally.

| Role | Size | Treatment |
| --- | --- | --- |
| Cover title | 104px | Georgia, regular, 1.02 line height |
| Slide title | 43px | Georgia, regular, 1.07 line height |
| Activity title | 53px | Georgia, regular |
| Final decision title | 61px | Georgia, regular |
| Subheading | 25px | Sans serif, bold |
| Body | 21px | Sans serif, 1.3 line height |
| Supporting sentence | 23px | Muted sans serif |
| Large figure | 80–146px | Georgia, regular; slide-specific |
| Question band | 22px | Sans serif, semibold |
| Eyebrow | 12px | Uppercase, tracking 0.15em |
| Source note | 9px | Supporting attribution only |

Prefer concise copy over shrinking type. Essential caveats belong in readable body text. Check wrapping on the export system because fallback fonts can differ.

## 4. Canvas and spacing

- Fixed 1280 × 720 HTML canvas. `fitDeck()` computes the viewport scale, and the deck is centered using a translate-and-scale transform.
- PDF pages remain 960 × 540 points (13.333 × 7.5 inches). Printing removes the screen transform.
- Standard slide padding: 36px top, 64px sides, 70px bottom.
- Question slides reserve 162px at the bottom. Their question band sits 56px from the bottom, with a 127px label column and 28px gap.
- Source notes sit 15px above the bottom. Slide numbers sit at the lower right.
- Use thin rules and flat columns. Keep filled boxes primarily for actual quiz controls or a meaningful formula.
- Large letters and numbered scenarios help the audience act. Do not add ornamental illustrations or logos merely to fill space.
- The HTML retains the original base CSS followed by editorial overrides. The later rules define the approved appearance. Check selector specificity before changing either block.

## 5. Reusable slide patterns

| Pattern | Composition | Existing reference |
| --- | --- | --- |
| Cover | Navy, large white serif title, fine rule, lime subtitle | Slide 1 |
| Opening poll | Cobalt, large A–D letters, open two-column choices | Slide 2 |
| Company context | Three large serif figures, direct-labeled bars | Slide 3 |
| Operating process | Four large numbers, thin rules and connectors | Slide 4 |
| Quantitative puzzle | Time bar, large 2.5 figure, visible caveat | Slide 5 |
| Economic mechanism | Navy, open equation and numbered explanations | Slide 6 |
| Chart explanation | Text beside solid PPP and dashed hourly curves | Slide 7 |
| General pay tradeoffs | Two columns comparing the benefits and risks of piece rates | Slide 8 |
| Contract comparison | Two open phases and a highlighted pay formula | Slide 9 |
| Worked example | Compact table beside a large blue earnings figure | Slide 10 |
| Class discussion | Lime, three responsibility columns and discussion task | Slide 11 |
| Minimum-pay debate | Reasons for protection versus weak incentives below the floor | Slide 12 |
| Guarantee calculation | Cobalt, white table, lime reduced guarantees | Slide 14 |
| Historical analogy | Cream, parallel Hanoi and Safelite comparisons | Slide 16 |
| Compensation scenarios | Lime, four numbered scenarios and a shared task | Slide 18 |
| Knowledge check | Cobalt, one question, interactive answer choices | Slide 19 |
| Options matrix | Flat table with labeled analytical judgments | Slide 20 |
| Proposed redesign | Thin ruled rows connecting provisions to purposes | Slide 21 |
| Fairness discussion | Lime, personal preference and unequal-opportunity hypothetical | Slide 22 |
| Final decision | Navy, equally prominent lime A–C letters and open columns | Slide 23 |

Reuse the composition that matches the content's purpose. Keep the visual differences between evidence and activities.

## 6. Writing and facilitation

Use concrete titles such as “The 30% guarantee cut is large in a household budget” or direct questions such as “Who controls each source of lost output?” Avoid generic headings such as “Unlocking potential.” Explain a concept with a case example before adding terminology.

Use conventional labels such as “Discussion,” “Compensation scenarios,” and “Knowledge check.” Phrase audience prompts as direct questions. Avoid scripted instructions such as “Vote first, then…” or “Ask the room.” Use individual answers and whole-class discussion only. Do not assign pairs, breakout groups, or teams.

Keep slide copy brief, usually about 35-75 words excluding source notes. Tables and exercises may need more. Put detailed interpretation, anticipated objections, and transitions in presenter notes.

Every discussion should have a specific task, a time limit, a response method, and a debrief. Useful formats include a vote, a whole-class discussion, allocating a shock to a responsible party, choosing a pay rule, or defending a contract. Avoid an unsupported “Thoughts?” prompt.

For a 60-minute session, build in a substantive interaction approximately every 5-8 minutes. Include time for students to think and answer. Preserve the current major stops unless the user requests different pacing:

| Stop | Minutes | Intended result |
| --- | ---: | --- |
| Opening diagnosis vote | 3 | Surface competing explanations for low output |
| Class discussion on control | 4 | Separate worker actions from production constraints |
| Class discussion of four scenarios | 4 | Design and defend a compensation rule |
| Five-question checkpoint | 5 | Test concepts and correct misconceptions |
| Compensation preferences and fairness | 4 | Distinguish contribution, opportunity, and pay basis |
| Final decision and revote | 7 | Connect the economic tradeoffs to a management choice |

The deck includes 13 short “Discussion” prompts on slides 3, 4, 6, 7, 8, 9, 10, 12, 13, 14, 15, 17, and 20. Each takes 10-30 seconds within its existing slide allocation. Slides 5 and 16 retain their existing discussion questions. The six longer stops above remain in place. Questions on slides 3, 17, and 20 are optional if the class is behind schedule. Notes give a response method, likely answer, optional follow-up, and debrief. Sum all slide timings after any revision. Allow for transitions by shortening optional questions when needed.

Use `.has-question` for a slide with a quick prompt and `.ask-room` for its bottom question band. The band has a quiet top rule, a cobalt “Discussion” label (lime on dark backgrounds), a small duration, and a larger navy question. On dark slides the question is white. Keep the question concise and reserve the bottom area with `.has-question` padding. Never overlap the content or the source note. The timing includes student responses and debrief, rather than adding time to the session. Put optional status in the notes so the presenter can decide whether to ask the visible question aloud.

### Presenter-note pattern

Write notes for someone who did not author the deck. Include:

1. Time allocation and the concept students should take away.
2. A concise explanation or worked calculation.
3. The exact question to ask and the response method, where relevant.
4. Likely answers, a misconception to address, and a short debrief.
5. A transition to the next slide when needed.

Keep the recommendation in the final notes clearly labeled as a suggested synthesis. Students can defend other decisions if they account for the evidence and tradeoffs.

### Game conventions

Use four concise, plausible alternatives with one defensible correct answer for concept questions. Keep open management judgments in discussion polls. Give an explanation after each answer reveal. Students may keep their own score, with one point per correct answer and five points possible.

The HTML checkpoint is a local classroom activity. It has no student-phone connection, automatic scoring, Kahoot account, hosted game, or live leaderboard. The slide labels it “Knowledge check”; it is a Kahoot-style local checkpoint, not a connected Kahoot game. Provide a static question fallback for the PDF and an answer key in presenter notes.

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

- Keep the Munger/Hanoi example on slide 16. It illustrates proxy gaming, not documented Safelite misconduct.
- Slide 22's demographic pay-gap scenario is hypothetical. Do not attribute a gap to Safelite or infer ability from gender or age. Discuss contribution, access to work, measurement, and fair procedures without making legal conclusions.
- Hourly and salary describe a pay basis; either can include performance bonuses. Neither automatically resolves compensation fairness.

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

Choose `.slide`, `.slide.blue`, `.slide.amber` (lime), or `.slide.dark`. Some named slides have dedicated palette overrides. Preserve `fitDeck()` and its resize listener, and disable transforms in print. The brief headline animation respects reduced-motion preferences. Exactly one slide should carry `.active` in presentation mode. Keep numbers, source notes, and notes synchronized after reordering slides.

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
