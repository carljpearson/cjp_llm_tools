# Survey Question Design: Technical Reference

Scope: writing the questions themselves — what to ask, how to phrase the stem, and how to design the response options. Excludes sampling, mode, pretesting, privacy, and analysis. Synthesized from *Surveying the User Experience* (Sauro & Lewis), *Surveys That Work* (Jarrett, 2021), and *Usability Testing for Survey Research* (Geisen & Romano Bergstrom, 2017).

## 1. Choosing What to Ask

### 1.1 Tie every question to a decision

- Every candidate question must pass four challenges:
  - What do you want to know?
  - Why do you want to know?
  - What decision will you make from the answers?
  - What number do you need to make the decision?
- Cut any item that does not map to a research question or decision.
- One survey cannot answer everything; defer out-of-scope items to a later survey.

### 1.2 Identify the question that matters most

- Identify a **Most Crucial Question** — the single item whose answer drives the key decision.
- Identify the audience's **Burning Issue** — the topic respondents most want to tell you about; including it raises engagement and response quality.
- Confirm both by listening (interviews, search logs, support transcripts) before drafting.

### 1.3 Use a research grid to find gaps and bloat

- Rows = candidate items, columns = research questions, cells = which item covers which question.
- *Gap* = research question with no item → add or defer the question.
- *Bloat* = item not tied to any research question → cut.

### 1.4 The four content classes of questions

Classify each candidate item into one class; the class drives the appropriate format.

- **Attributes**: characteristics of respondents or their organizations (age, education, income, role, company size).
  - Common pitfalls: overlapping ranges (18–21 / 21–25), incomplete ranges, sensitive items asked when not needed.
  - Ask only the attributes you will actually use; cluttering with unused demographics lowers completion.
- **Behaviors** (reported): self-reports of past or current actions (frequency, duration, intensity, recency).
  - Always anchor with a reference period; the longer the period, the more error.
  - Distinct from observed behavior — self-reports are a useful but imperfect predictor.
- **Abilities**: knowledge or skill assessments, including task-based UX items ("find a blender under $45 with ≥4 stars").
  - Distinct from self-rated ability, which is a sentiment item.
- **Thoughts / sentiments / judgments**: attitudes, satisfaction, preference, intent, awareness, perceived usability.
  - Where standardized scales exist for the construct (SUS, NPS, SEQ, UX-Lite), prefer them over custom items.

### 1.5 Prefer standardized items where they exist

- A standardized questionnaire is one whose items have been psychometrically validated for reliability, validity, sensitivity, and (often) normative interpretation.
- Use them when the construct matches; do not modify wording beyond cosmetic substitutions (e.g., "system" → "product").
- The Net Promoter item is a single item, not a Likert scale; do not call any one-item scale a "Likert scale."

### 1.6 Keep the set small

- Up to ~60% of survey dropout is effort-related; length is a primary driver.
- Aim for the smallest set that answers the decision; "light-touch" surveys of ~5–7 substantive items outperform omnibus surveys.
- If you must collect many items, group thematically and break across pages.

## 2. Anatomy of a Question

A survey *item* has up to six components (Saris & Gallhofer); only the request and response options are required.

- **Introduction** (optional): orients the respondent to the topic, especially at topic shifts or before items needing recall.
- **Information / definitions** (optional): defines unfamiliar terms or scopes ambiguous concepts.
- **Instructions** (optional): tells the respondent how to answer; required for uncommon formats (ranking, Kano, pick-some, MaxDiff, allocation).
- **Opinions of others** (optional, rare in UX/CX): inserts a third-party view; usually biasing — avoid unless the reaction to others' opinions *is* the research target.
- **Request for an answer** (required): the core of the stem; three forms below.
- **Response options** (required, except for pure open-ends): the menu the respondent picks from.

### 2.1 Three ways to phrase the request

- **Direct request**: invert subject and auxiliary verb of a statement ("You would need help" → "Would you need help?").
- **Indirect request** (statement + agreement scale): "I felt confident using the software." — respondent rates agreement.
- **Wh-request**: use who, what, when, where, why, how, which ("What is your age?", "Why did you select that number?").

## 3. The Cognitive Model the Stem Must Support

Respondents pass through four stages; each stage is a failure point.

- **Comprehension**: perceive the words and construct meaning.
- **Retrieval**: locate the relevant information in memory or elsewhere.
- **Judgment**: combine retrieved information into an answer.
- **Response**: map that answer onto the offered options.

Design each item so all four stages succeed.

## 4. Writing Clear Stems

### 4.1 Length and structure

- Keep stems short: <25 words, <3 commas.
- Strip filler phrases:
  - "due to the fact that" → "because"
  - "at this point in time" → "now"
  - "if conditions are such that" → "if"
  - "take into consideration" → "consider"
- Use simple language; pick the shorter, more common word ("angry" not "irate"; "use" not "utilize").
- Prefer high-frequency words; common words require less processing.
- Use the respondent's vocabulary, not internal jargon; validate with informal interviews before fielding.
- Minimize acronyms; spell out on first use unless universally known (NATO, SCUBA).
- Use active voice; passive is rarely justified in questions (it can soften instructions, but not items).

### 4.2 Avoid complex syntax

- **Adjunct wh-questions**: avoid garden-path structures.
  - Bad: "When did you tell your account rep your software license needed to be renewed?"
  - Better: "When did you tell your account rep that you needed to renew your software license?"
- **Embedded clauses**: avoid putting clauses between subject and verb.
  - Bad: "The task that I just completed in this study was easy."
  - Better: "This task was easy."
- **Left-embedded syntax**: avoid stacking adjectives, adverbs, or prepositional phrases before the main clause.
  - Bad: "Even if it would cost them some money and make their code more complex because the rules are a complicated mix of regulations, Twitter should comply with industry guidelines."
  - Better: lead with the agreement claim, then qualify after.

### 4.3 Ask one thing per question

- **Double-barreled items** combine two questions into one and produce uninterpretable answers.
  - Bad: "Do you have independence in choosing projects and directing your energy?"
  - Fix: split into two items.
- Same rule applies to triple-barreled items (e.g., "How is your mood at work, at home, and with other people?").

### 4.4 Avoid faulty presuppositions and leading framing

- Statements that presuppose a contested fact bias both response and memory ("Family life has suffered during COVID because parents are concentrating too much on work" presupposes the cause).
- Leading wording ("How outstanding was the experience?") pushes positive responses.
- The Loftus stop-sign/yield-sign study: a single word in the question implanted false memories in 41% of participants.
- Fix presuppositions by splitting into a filter item plus a conditional follow-up.

### 4.5 Eliminate vague concepts

- A concept is *vague* if respondents differ on whether it applies to them ("How many children are staying?" — does an infant count?).
- Define the boundary in the stem: "How many children (aged 0–18) are staying?"
- Balance precision against complexity — overly specified items become unreadable.

### 4.6 Eliminate vague quantifiers

- Vague quantifiers (often, frequently, near, very, quite, much, most, few, several, occasionally, sometimes) are interpreted as anywhere from 52 to 365 occurrences per year by different respondents.
- For frequency, use concrete intervals ("0–2 times per week", "3–4 times per month").
- For *perception* of frequency, vague quantifiers are acceptable — but do not treat the result as a frequency count.
- Vague quantifiers appear in both stems *and* response option labels; check both.

### 4.7 Avoid false inferences

- Words like *any*, *all*, or *every* invite the respondent to consider edge cases the researcher did not intend.
  - "Are there any situations in which you would approve of Robinhood removing access?" — literal reading captures fraud cases, not the intended construct.
- Constrain scope explicitly when using broad quantifiers.

### 4.8 Specific words to watch

- **Absolutes** (*ever, always, never*): extreme responders read them literally and others read them loosely; you cannot tell which is which.
- **Modal verbs** (*could, should, would, might*): each implies a different level of obligation/probability — pick deliberately.
- **You**: ambiguous between the individual and their household — clarify when scope matters.
- **Our**: introduces sponsorship cues; replace with the explicit entity name.

### 4.9 When to use introductions, information, and instructions

- **Introduction** between question blocks when the topic shifts or when the next block requires recall.
- **Information** when the topic uses unfamiliar terms, complex constructs, or response options that can be confused.
- **Instructions** for any non-standard response format (ranking, Kano, MaxDiff, pick-some, allocation), or when a common mistake is likely (e.g., people picking one when "all that apply" is allowed).

## 5. Designing for Memory

When a question requires recall, design the stem and reference period to compensate for predictable memory failures.

### 5.1 Four memory failures

- **Retrieval failure**: detail was encoded but cannot be retrieved; worsens with time and lower salience.
- **Reconstruction**: respondent fills gaps with generic memory of similar events.
- **Distortion**: memory is altered by intervening exposure (photos, others' accounts, social media).
- **Term mismatch**: researcher's term doesn't trigger the respondent's memory ("online shopping" may not include Grubhub or pharmacy pickup).

### 5.2 Telescoping

- *Forward telescoping*: events recalled as more recent than they were.
- *Backward telescoping*: events recalled as more distant.
- Both inflate counts in a stated reference window.

### 5.3 Techniques that improve recall

- **Shorten the reference period** — shorter windows reduce telescoping and approximation; in one study a 1-month window produced reports of 32% more home repairs than a 6-month window of comparable recall accuracy.
- **Anchor to personal landmarks** ("since your last birthday", "since you started this job") — reduces telescoping.
- **Reverse chronological order** ("Tell me about your most recent visit, then the one before") — often improves recall for sequences.
- **Decompose broad categories** — "shopping" → clothing / groceries / furniture; visits → primary care / specialist / urgent care.
- **Use concrete cues in the introduction** to constrain scope.
- **Give more time** in interview/phone modes; on web, encourage reflection.
- Ask about *recent, vivid* experience whenever possible; unremarkable repetitive events have very low recall accuracy after a short interval.

## 6. Response Options: Decision Logic

Choose the response format by walking the decision tree from research goal downward.

1. Goal = **discovery** → open-ended item.
2. Goal = **measurement** → categorical or non-categorical.
3. **Categorical** → mutually exclusive (single-select) or not (multi-select).
4. **Non-categorical** → ranking, allocation, or rating.

Use the simplest format that satisfies the goal — added complexity costs effort without guaranteed gain.

## 7. Open-Ended Items

### 7.1 When to use them

- **Exploratory research** — learning about a phenomenon before constraining it.
- **Bias reduction** — placing an unconstrained open item *before* a related closed item to avoid priming.
- **Unaided recall / awareness** — measuring what comes to mind without showing a list (stronger than aided recognition).
- **Follow-up to a closed rating** — capture the "why" behind a low NPS or SEQ.
- **End-of-survey catch-all** — give respondents one last chance to surface anything the survey missed.

### 7.2 Drafting rules

- Phrase neutrally; do not presuppose the answer ("What did you like about your visit?" assumes liking — use "Please describe your visit").
- Match box size to expected answer length — small box signals short answer, large box signals long answer.
- Larger boxes increase data richness but lower completion rate; balance deliberately.
- For long forms, consider a primarily closed item with an "Other [text]" escape rather than a fully open item.

## 8. Categorical Items

### 8.1 Selecting the right form

- **Mutually exclusive + single-select** → radio buttons.
- **Not mutually exclusive + multi-select** → checkboxes ("select all that apply", SATA).
- On web, enforce the distinction with the control type; on paper, you cannot enforce it — make it clear in instructions.

### 8.2 Common construction errors

- **Overlapping ranges** (e.g., 10–20 / 20–30 / 30–40): respondent at 20 has two valid answers — use 10–19, 20–29, 30–39.
- **Gaps in ranges** (e.g., $25k–$39k / $40k–$50k): respondent at $39,500 has no answer.
- **False mutual exclusivity**: presenting categories as single-select when respondents can legitimately belong to several.
- **Incomplete option lists**: missing categories force respondents to guess or drop out; include "Other" or a complete set.

### 8.3 "Other" and escape options

- Always include an "Other [text]" option when the list may be incomplete; "Other" answers are often the most informative.
- In sensitive contexts, relabel "Other" as "Something else", "Another answer", or "In your own words" — being labeled "other" can alienate.

### 8.4 SATA vs. yes/no series vs. yes/no grid

- **SATA (multi-select checkbox)** is the recommended default for non-mutually-exclusive categories.
- A **yes/no series** (one yes/no per option) produces a ~3% higher Yes rate than SATA — likely because some respondents click Yes through long lists to finish faster, so the count is inflated.
- A **yes/no grid** produces selection frequencies indistinguishable from SATA (effect size ~0.1%) but respondents strongly prefer SATA.
- Recommendation: SATA for breadth questions; reserve forced-choice grids for cases where you need an explicit non-selection per option.

## 9. Ranking and Allocation

### 9.1 Forced rank

- Respondent orders all items from most to least important.
- Cognitive load grows steeply past ~7 items.
- Use only when the relative order of every item matters.

### 9.2 Pick-some ranking

- Respondent picks the top *k* (e.g., top 3) and orders only those.
- Lower load than full rank; preferred when only the top tier matters.

### 9.3 MaxDiff (best-worst scaling)

- Respondent sees rotating subsets of items and picks the most and least important in each.
- Scales to many items (15+) with manageable per-screen load.
- Requires specialized software to rotate subsets and compute scores.

### 9.4 Allocation / constant sum

- Respondent distributes a fixed total (100 points, $100, 100%) across items to indicate relative importance.
- Have the survey tool auto-sum and display the running total — reduces mental math errors.

### 9.5 Instructions

- All ranking and allocation formats need explicit instructions; do not assume respondents know how to interact.

## 10. Rating Scale Types

Match the rating type to how the construct is *conceptualized*.

- **Linear numeric (general purpose)**: numbered options, endpoint labels, optional intermediate labels; treatable as continuous when n is reasonable.
- **Likert-type (agreement)**: statement + Strongly Disagree → Strongly Agree.
  - A *Likert scale* technically refers to the composite (mean/sum) of multiple agreement items; a single agreement item is a Likert-*type item*.
- **Unipolar (none-to-much)**: the attribute is conceptualized from zero to maximum (e.g., satisfaction, confidence).
- **Bipolar (semantic differential)**: opposing endpoints (easy ↔ difficult, useful ↔ useless).
- **Performance / adequacy / quality**: rate the quality of an experience (e.g., "Far below average" → "Far above average").
- **Disconfirmation (meeting expectation)**: "Much worse than expected" → "Much better than expected"; midpoint anchored to "About what I expected"; **always odd number of points**.
- **Comparative**: rate one item against a benchmark or another item; useful for relative judgments.
- **Frequency**: use concrete intervals, not vague quantifiers.

## 11. Number of Scale Points

### 11.1 Defaults

- 5 points is the most common; 3 and 7 are also defensible; 11 is standard for NPS-style likelihood items.
- Use an **odd number** when the construct supports a real midpoint; use an even number to force a directional choice.

### 11.2 Evidence on point count

- Respondents use all points on 3-, 5-, 7-, and 11-point scales — large numbers of points do not confuse them.
- Two- and three-point scales sacrifice individual-level fidelity; they may be acceptable only when averaging across many items at the group level.
- Five points is sufficient when discrimination at the individual level matters less; seven, ten, or eleven points increase sensitivity, reliability, and (in some cases) validity.
- Mixing scale lengths (5, 7, 11) within one survey does not measurably degrade quality when each item is a known standardized item.

### 11.3 The neutral midpoint

- An odd-numbered scale gives a midpoint that serves both genuine neutrals and respondents who do not have a clear answer.
- On *sensitive topics*, a labeled neutral can absorb weak preferences and reduce the count of soft favor/oppose responses — consider whether you want a directional read.
- Adding a labeled neutral *attracts* some responses to the midpoint but generally does not damage validity.
- Alternative: keep the midpoint and add "Don't know" / "Not applicable" as separate escape options.
- Default rule: include a midpoint unless you have a specific reason to force direction.

## 12. Labeling Scale Points

### 12.1 Three labeling strategies

- **Fully labeled**: every point has a word label.
- **Endpoints only**: just the two ends are labeled; intermediate points show only numbers.
- **Endpoints + midpoint**: ends and the neutral point are labeled.

### 12.2 What the evidence says

- For *sentiment* scales used in UX/CX (satisfaction, agreement, usability), full labeling has no clear advantage over endpoint-only labeling; differences in means are typically <2% of scale range.
- For *rubrics and objective frequencies* (e.g., specific frequencies like "daily" vs. "monthly"), full labeling improves validity because the labels carry objective meaning.
- Fully labeled scales can evoke more acquiescence; endpoint-only scales can evoke more extreme responses; effects are small and topic-dependent.
- Past 7 points, full labeling becomes impractical and forces the use of vague modifiers — avoid this trap.

### 12.3 Practical recommendation

- ≤7 points, sentiment item: either fully labeled or endpoints + midpoint — pick one and be consistent.
- >7 points (e.g., 11-point NPS): label endpoints; optionally label midpoint; do not invent vague labels for intermediate points.
- Always show the numeric value alongside any verbal label.
- Avoid scales where intermediate labels create hairsplitting distinctions ("fairly often" vs. "often").

## 13. Endpoints

- Match the *intensity* of the two endpoint labels (e.g., "Strongly Disagree" ↔ "Strongly Agree", not "Disagree" ↔ "Strongly Agree").
- More-absolute endpoints (e.g., "Completely Disagree") produce more extreme responding than less-absolute endpoints.
- For bipolar scales, ensure the two endpoints are true semantic opposites for your respondents — test with target users when in doubt.

## 14. Item Tone in Multi-Item Scales

- Default to a **consistently positive tone** across all items in a composite scale.
- Alternating positive/negative tone was historically used to disrupt acquiescence; in UX research it produces more problems than it solves:
  - Respondents miss the negation and answer the inverted item the same direction as the others.
  - Researchers forget to reverse-score on analysis.
  - Factor structure is distorted by method variance from the negated items.
- Exception: when the construct is inherently negative (clutter, frustration), tone-match the construct — but expect some respondents to agree with negative statements they mean to disagree with.

## 15. Question Order Within the Survey

Order is part of question design — context changes meaning.

### 15.1 General–specific order

- Asking a **general item first** (overall satisfaction) before specifics typically produces lower correlations between general and specific, and gives a less biased general estimate; the general mean is roughly 2% lower than when asked after specifics.
- Asking **specifics first** raises the general rating (the specifics serve as a kind of summary judgment scaffolding).
- For unbiased general estimates: ask general first.
- For explanatory power and "natural" flow in domains where respondents think bottom-up (e.g., complex products): specifics first is defensible.
- Pick one order and keep it constant for tracking.

### 15.2 Priming

- An earlier item can activate beliefs that shift answers to later items; sensitive topics are most susceptible.
- Priming effects are larger for item-by-item presentation than for grid presentation of the same items.

### 15.3 Demographics and sensitive items

- Place demographic and sensitive items at the **end** unless they are needed for screening or branching.
- Starting with demographics primes the gender/age/race/income lens and depresses response rate.
- If demographics must come first for branching, use only the necessary items, not the full demographic block.

### 15.4 Opening the survey

- Open with the **Burning Issue** or the most engaging substantive item — builds momentum.
- Avoid intrusive or surprising openers; even a sex-and-vacation question should be preceded by general vacation questions.
- Group items by topic, moving from least to most intrusive within a topic.

## 16. Grids and Matrices

### 16.1 When to use a grid

- Use grids only for items that share both a stem frame and a response scale (e.g., a set of agreement items rating different features).
- Grids save space and reduce priming between items but encourage **straightlining** when respondents disengage.

### 16.2 Grid design rules

- Keep grids small — somewhere between 5 and 10 rows is a reasonable upper bound; larger grids increase dropout sharply.
- Group thematically and break grids across pages rather than one giant grid on one page.
- Splitting one grid across multiple pages can paradoxically *increase* straightlining as respondents try to look non-uniform — keep related items grouped on one page when feasible.
- For ≥9 response columns, data quality degrades; prefer item-by-item presentation for long-scale items.
- On mobile, prefer item-by-item; grids degrade badly on narrow viewports.

### 16.3 Grid vs. one-at-a-time tradeoffs

- One-at-a-time slightly improves internal reliability and reduces straightlining but increases completion time by ~50%.
- Grid means run about 1% higher than one-at-a-time means for the same items — small and not always meaningful, but worth noting when comparing.

## 17. Visual Presentation of Response Options

- List options in a **single vertical column**; multi-column layouts produce inconsistent scanning (some respondents go top-to-bottom-then-right, others right-then-down).
- Use multi-column only when a single column would force scrolling that cuts options out of view.
- Horizontal vs. vertical scale orientation produces only ~2% mean difference — not practically significant; choose for layout fit.
- For rating scales presented vertically, the option-at-top can attract slightly more responses, but the top-first bias is inconsistent and weak; ignore in practice.
- Hide or de-emphasize numeric anchors only if labels are sufficient; otherwise show both.

## 18. Making "Required" vs. "Optional" Decisions

- Default to optional questions; required questions cost some completions and produce false data from people who could not honestly answer.
- A "Don't know" / "Not applicable" / "Prefer not to answer" option lets you keep the question required while accepting honest non-answers — at the cost of slightly more reading per item.
- If a question is genuinely required for the analysis, make it required *and* offer the opt-out option, then warn (not nag) on skip.

## 19. Quick Defaults

When no specific guidance applies, these defaults are safe.

- **Format**: closed-ended with one open-ended follow-up for the "why" on key ratings.
- **Stem**: <25 words, one idea, active voice, common words, no vague quantifiers.
- **Reference period**: shortest that fits the research question; anchor to a landmark when possible.
- **Categorical**: SATA for multi-select; radio buttons for mutually exclusive; always include "Other [text]" if the list might be incomplete.
- **Rating scale**: 5-point, fully labeled, all-positive tone, vertical layout, single column.
- **Likelihood-to-recommend / intent**: 11-point with endpoints (and optionally midpoint) labeled.
- **Order**: Burning Issue first → main measurement block → demographics last.
- **Grids**: ≤10 rows, grouped thematically, never on mobile-first surveys.
- **Standardized items** (SUS, SEQ, UX-Lite, NPS): use as-is; do not modify beyond cosmetic word swaps.
