# Stage 3 supporting log a — per-book findings: S1 — Kenneth A. Adams, *A Manual of Style for Contract Drafting*, 4th ed. (ABA, 2017)

**Stage:** 3 (supporting record for `2026-09-18-stage-03-five-book-extraction.md`)  
**Date:** 18 September 2026  
**Local source identifier:** `books/A_Manual_of_Style_for_Contract_Drafting_-_Kenneth_Adams.pdf` (local only; not committed)  
**Access status:** full text available  

## Method and limits

- The book text was extracted locally with `pypdf`. Nothing was uploaded to an external service.
- Reading was split into parts. One reading agent examined each part directly from the extracted text. Agents were forbidden to use the web or model memory as evidence.
- The coverage record in each part states what was read fully, skimmed or not read.
- The local file is a converted e-book. PDF page numbers are not print pages. Locations use the book's own numbered paragraphs (for example ¶3.72), which are stable across formats.
- Findings are expressed independently. Short phrases only are quoted.
- Dispositions here are **proposed** by the reader of each part. The accepted dispositions are in the main Stage 3 log.
- Statements of substantive law are recorded as research questions only. They are not authority for any live matter.
- Spot-checks of findings against the book text are recorded in the main Stage 3 log.

---

## Part 1 — Introduction, chapters 1–3 (IDs AD1-)

Source read: locally extracted text `txt/adams.txt`, pdf-pages 36-280 (file lines 984-9092). Converted e-book: pdf-page numbers are not print pages, so locations below use the book's own numbered paragraphs (¶) and section headings. The Introduction has no paragraph numbers; it is cited by heading. The book itself cross-refers to the Introduction passages on passive drafting and "tested" language as "p. xxxvi" and "p. xxxvii".

Orientation note that applies to every finding: the author writes for **business-to-business contracts** (expressly not consumer contracts), is **US-oriented** in caselaw, doctrine and practice conventions, claims the prose guidance travels to UK/Australia/Canada, and cites sparingly by design (no footnotes, no bibliography). Many prescriptions are knowingly non-traditional and the author says so.

---

### 1. Coverage record

| pdf-page range | Chapter / section | Status | Note |
|---|---|---|---|
| 36-38 | Tail of Preface (changes from 3rd ed.), Acknowledgments | Read fully | Assigned range starts mid-Preface; the earlier Preface/Foreword pages fall before pdf-page 36 and were not in my range. Nothing of production value here. |
| 39-56 | Introduction ("About This Manual"; traditional language is dysfunctional; resistance to change; change at individual / organisation / industry level) | Read fully | Unnumbered paragraphs. |
| 57-72 | Chapter 1, characteristics of optimal contract language, ¶1.1-1.66 | Read fully | |
| 73-91 | Chapter 2, ¶2.1-2.72 (title, introductory clause, date, parties) | Read fully | More than the first third. |
| 91-95 | Chapter 2, ¶2.72-2.90 (capacities, trusts, divisions, incidental/extraneous information, intent to be bound) | Read (fast) | Read in full but quickly. |
| 95-105 | Chapter 2, ¶2.91-2.128 (defined terms for party names, "this agreement") | Read (fast) | Mostly style-level; little extracted. |
| 105-126 | Chapter 2, ¶2.129-2.217 (recitals, lead-in, recital of consideration, cover sheet) | Read fully | Consideration discussion is heavily doctrinal: treated as research questions. |
| 127-280 | Chapter 3, categories of contract language, ¶3.1-3.482 incl. Figure 1 and Tables 1-16 | Read fully | Priority chapter. The acceptability symbols attached to table examples (recommended / caution / not recommended / avoid) were lost in text extraction; I relied on the prose to determine which variant is recommended. |
| 281+ | Chapter 4 onward | Not read | Outside assignment. |

No part of the assigned range was left unread. Sample 1 and Sample 2 (images of an introductory clause and recitals) did not survive text extraction.

---

### 2. Material findings

#### AD1-01
- **ID:** AD1-01
- **Location:** Introduction, "Traditional Contract Language Is Dysfunctional" — subsection "The Primary Cause of Dysfunction" (book's own cross-reference: p. xxxvi)
- **Problem addressed:** Contracts are built by copying precedents nobody has time or skill to reassess, so defects replicate and nobody needs guidelines or training.
- **Principle / method / heuristic (own words):** Distinguishes "passive drafting" (copy on faith because it supposedly worked before) from "active drafting" (work to a comprehensive usage guideline, be trained in it, and copy only from templates/precedents that already comply with it). Copying is not the problem; unexamined copying is.
- **Assumptions and applicability:** Any precedent-driven transactional drafting. Assumes a guideline exists and that someone has authority to vet templates. Not jurisdiction-specific.
- **Production responsibility affected:** drafting, review/redlining, product consistency, evaluation
- **Workflow / decision implication:** A drafting agent must not treat a supplied precedent as validated merely because it was used before. It should (a) record the provenance and compliance status of any source text, (b) run reused text through the same checks as new text, (c) say so when it reuses unvetted precedent.
- **Evaluation evidence or criterion:** For each reused block, does the output record source and whether it was checked against the governing style/usage standard? Fail if precedent text passes through with known-defect patterns (e.g., those in AD1-13 to AD1-25) unflagged.
- **Failure / misuse conditions:** Treating "active drafting" as licence to rewrite mandated house or industry forms the user has no authority to change (the author himself concedes this limit under "Your Draft").
- **Repair implication:** Where rewriting is not permitted, downgrade from rewrite to flag-and-explain.
- **Proposed disposition:** retain — directly describes the core failure mode of an AI drafter that pattern-matches precedent.

#### AD1-02
- **ID:** AD1-02
- **Location:** Introduction, "Resistance to Changing Traditional Language" — "Claiming That Traditional Language 'Works'", "Claiming That Traditional Language Has Been 'Tested'" (p. xxxvii), "The Significance of Caselaw"; echoed ch 1, ¶1.26 and ¶1.31
- **Problem addressed:** Whether to keep traditional wording because courts have interpreted it ("tested"/"settled" language).
- **Principle / method / heuristic (own words):** The author rejects the "tested" argument on three grounds: only a narrow slice of usages has ever been litigated; courts do not assign a uniform meaning (results vary by facts, judge, time and jurisdiction); and language that had to be litigated is by definition language that failed to state intent clearly. He also rejects "it works" as a false binary: contracts are more or less clear, costly and dispute-prone. Caselaw is used in the book as evidence of *which usages cause fights and how judges misread*, not as a source of meaning for a word. He states that an aberrant decision will not make him withdraw a recommendation. Counterweight he himself supplies (¶1.26): before replacing a term of art, check whether courts attach significance to the specific wording.
- **Assumptions and applicability:** US commercial practice, where (he says) courts tend not to insist on magic words. Less safe where statute, regulation or a court line gives specific words operative effect, or in jurisdictions he shows behave differently (see AD1-25 on English treatment of "warrants").
- **Production responsibility affected:** drafting, review/redlining, research, authority verification, risk communication
- **Workflow / decision implication:** "This wording is tested" is not by itself a reason for an agent to keep unclear wording; but "this wording is clearer" is not by itself a reason to delete a term that the governing law makes operative. The agent should separate two questions: (1) is the wording clear on its face; (2) does governing law attach consequences to this exact wording — and route (2) to research rather than answering from a drafting manual.
- **Evaluation evidence or criterion:** When the agent replaces or retains a traditional term, does the output state which of the two grounds it relied on, and flag a governing-law check where the term is doctrinal? Fail if it asserts "settled meaning" or "no legal significance" without a jurisdiction-specific source.
- **Failure / misuse conditions:** Adopting the author's posture ("an errant opinion is no reason to retreat") as the agent's risk posture. A commentator may disregard outlier cases; a drafter for a client in that court's jurisdiction may not.
- **Repair implication:** Insert a mandatory "does the governing law care about these words?" gate before any term-of-art substitution.
- **Proposed disposition:** qualify — persuasive as a critique of lazy reliance on precedent, but it is the author's contested position, not a rule of law.

#### AD1-03
- **ID:** AD1-03
- **Location:** Introduction, "Change at the Level of the Individual" — "The Other Side's Draft" and "Your Draft"; ch 2, ¶2.50 (between/among as a worked example of a painless concession)
- **Problem addressed:** How far to push drafting improvements when reviewing a counterparty's draft, or when one's own draft meets resistance.
- **Principle / method / heuristic (own words):** Reviewing the other side's draft is not an editing exercise. Look only for (a) text that does not match the deal as understood and (b) text that could cause confusion. Let pass traditional features that are pointless but harmless (archaic front/back matter, a conventional consideration recital, benign overuse of "shall"). Worth raising: a condition drafted as an obligation, inherently confusing usages, any ambiguity, and even small glitches of a kind known to have produced disputes (throat-clearing; "may" in restrictive relative clauses). For one's own draft: concede meaning-neutral points to seniors and counterparties, persist on what affects meaning, be firmer on templates than on one-off deals, and consider explaining the drafting approach up front.
- **Assumptions and applicability:** Negotiated B2B contracts with a counterparty whose goodwill matters. The specific "harmless" list is US-flavoured.
- **Production responsibility affected:** review/redlining, risk communication, scoping
- **Workflow / decision implication:** A review agent needs a severity tier: *deal mismatch* > *ambiguity / wrong category (condition vs obligation, missing actor)* > *known dispute-generating usage* > *harmless tradition (do not redline in a counterparty draft)*. Mode (own draft / template / counterparty draft) must be an input to the review.
- **Evaluation evidence or criterion:** On a counterparty draft seeded with both harmless archaisms and a condition-as-obligation defect, the agent flags the latter and does not redline the former. Fail if redlines are dominated by stylistic changes.
- **Failure / misuse conditions:** Using the etiquette rule to suppress a finding that does affect meaning; or applying own-template strictness to a counterparty's paper.
- **Repair implication:** Add a "would this change alter meaning or reduce dispute risk?" filter before emitting any redline on third-party paper.
- **Proposed disposition:** retain — directly usable as redline triage policy.

#### AD1-04
- **ID:** AD1-04
- **Location:** Introduction, "Change at the Level of the Organization" ("A Style Guide as Foundation", "Training and Templates", "Surrendering Autonomy", "Specialization"); ch 1, ¶1.63-1.66
- **Problem addressed:** Inconsistent usages across drafters in one organisation; the idea that each lawyer has a legitimate personal drafting "style".
- **Principle / method / heuristic (own words):** Consistency has to be imposed centrally: adopt a usage style guide, train people to it, and rebuild templates to match, because people draft by copying. Where alternatives exist one is usually clearest and all should use it; even when alternatives are equally clear, a single house choice avoids confusion and lets text move between documents. Ideal: you cannot tell who drafted which contract. Warns against template design by committee and against delegating template work to the least experienced. Suggests specialisation/automation where volume justifies it.
- **Assumptions and applicability:** Organisations with recurring contract types. The author has a commercial interest in the style guide and automation he recommends.
- **Production responsibility affected:** product consistency, drafting, evaluation
- **Workflow / decision implication:** An AI drafter should run against an explicit, versioned usage standard (the organisation's, if one exists) rather than an implicit "model style", and report deviations from it. Where the organisation's standard conflicts with Adams, the organisation's standard governs.
- **Evaluation evidence or criterion:** Same instruction given twice yields the same usage choices; output cites the applicable style rule for non-obvious choices.
- **Failure / misuse conditions:** Imposing Adams's conventions where the client's house style or an industry form differs.
- **Repair implication:** Make the usage standard a configurable input, with Adams-derived rules as one optional profile.
- **Proposed disposition:** adapt — principle retained; the specific standard must be pluggable.

#### AD1-05
- **ID:** AD1-05
- **Location:** ch 1, "Omit Problematic Terms of Art", ¶1.7-1.27 (incl. "Replacing Terms of Art" ¶1.20-1.26 and "Terms of Art in Languages Other Than English" ¶1.27); archaisms ¶1.4-1.6
- **Problem addressed:** Doctrinal terms used in contracts without need or without understanding.
- **Principle / method / heuristic (own words):** Terms of art are legitimate shorthand where the transaction needs them. Three defective kinds: **unnecessary** (a heavy doctrinal word doing a trivial job; tempts people to think the word itself makes the doctrine apply), **improvised** (lawyers/judges read doctrine into ordinary rhetorical phrases, driven by the give-every-word-effect canon), and **unduly complex** (meaning is real but so intricate that drafters use it without grasping consequences, risking unenforceability or surprises). Replacement is a cost-benefit call: weigh confusion risk against negotiation friction. Bridging tactics: keep the term but explain it in the text; or put the term in the heading and plain wording in the body. First check whether courts treat the specific term as significant. For English-language contracts under a non-English-language legal system, put the original-language term in parentheses after the translation to avoid back-translation drift.
- **Assumptions and applicability:** US courts said to be tolerant of substitutes; bridging tactics assume headings are not excluded from interpretation (author dismisses that rule of interpretation as of little use — contestable).
- **Production responsibility affected:** drafting, review/redlining, issue spotting, research, escalation
- **Workflow / decision implication:** For each doctrinal term in a draft, classify: needed / unnecessary / improvised / unduly complex. For the last class, the agent should require that the user confirm they intend the doctrinal consequences, or escalate. Never delete a term of art without the governing-law check.
- **Evaluation evidence or criterion:** Given a clause containing an unduly complex term, the agent identifies it, states that its legal effect needs confirmation under the governing law, and does not silently "simplify" it.
- **Failure / misuse conditions:** Treating the author's example lists as authoritative for every jurisdiction; stripping a term that a statute or registry requires.
- **Repair implication:** Pair the classification with a research hand-off; default to explain-and-keep when uncertain.
- **Proposed disposition:** retain (classification) / qualify (substitution advice is jurisdiction-dependent).

#### AD1-06
- **ID:** AD1-06
- **Location:** ch 1, "Use Standard English" ¶1.28-1.32; "Contract Language Should Be Precise" ¶1.33-1.36; Introduction, "Underestimating Complexity" and "Legalistic Hairsplitting"
- **Problem addressed:** Confusion between clear drafting and "dumbed-down" plain English; belief that legalese is precise; belief that wording is a formality once the deal point is agreed.
- **Principle / method / heuristic (own words):** Target a specialised form of standard English as used by educated native speakers. A contract is unavoidably as complex as its transaction; the aim is to remove *gratuitous* obstacles, not complexity. Precision means making it hard for a disgruntled party or a judge to find an unintended meaning; its enemy is uncertain meaning. The deal is what the text says, so wording is substance. Do not assume formal-logic readings of words (e.g., "or", "if and only if") will be applied — the ordinary-English reading is likely to prevail. Conversely, do not read into usages meanings that are not established or that English does not support. Intuition about "what sounds right" is unreliable in this register, for lawyers and judges alike.
- **Assumptions and applicability:** B2B contracts read by sophisticated parties. Not a consumer-readability standard.
- **Production responsibility affected:** drafting, review/redlining, reasoning/applicability, evaluation
- **Workflow / decision implication:** Evaluate drafts on "could a motivated adversary extract a second meaning?" rather than on reading-ease scores. Do not rely on logical operators' formal semantics when drafting conditions and lists.
- **Evaluation evidence or criterion:** Adversarial-reading test: a second pass attempts to construct an alternative reasonable meaning for each operative sentence; pass if none is found or each is flagged.
- **Failure / misuse conditions:** Simplifying away necessary complexity; using readability metrics as the success criterion.
- **Repair implication:** Replace "plain language" objectives in prompts/evals with "single reasonable meaning" objectives.
- **Proposed disposition:** retain.

#### AD1-07
- **ID:** AD1-07
- **Location:** ch 1, "Contract Language Should Omit Redundancy", ¶1.37-1.56 ("Limit the Use of Strings" ¶1.38-1.52; "Reject Needless Elaboration" ¶1.53-1.56)
- **Problem addressed:** Synonym strings and over-enumeration that add words and create interpretive openings.
- **Principle / method / heuristic (own words):** Strings hurt in three ways: surplus words; courts try to give each word work, so a stray word can acquire unintended meaning; and a string repeated with small variations invites an argument that the variation was deliberate. Method: test each element for a distinct *and useful* meaning; prune only when confident the surviving word covers the rest (some strings are needed to cover the field, e.g., lists of encumbrances); consider replacing a string of legal functions with a direct statement of the contexts intended; for catch-all definitions, define the concept "however referred to" rather than listing every label; if a string recurs, repeat it identically or make it a defined term. "Needless elaboration" = adding sub-categories to a general term whose scope is already clear; it can even narrow coverage.
- **Assumptions and applicability:** General. The safe-to-prune examples are the author's judgment, largely US.
- **Production responsibility affected:** drafting, review/redlining, product consistency, change impact
- **Workflow / decision implication:** Review check for (a) recurring strings with variant membership across the document; (b) general-term-plus-obvious-examples. Drafting rule: never vary a list by accident.
- **Evaluation evidence or criterion:** Automated: detect near-duplicate enumerations within one document whose members differ; each must be reconciled or justified.
- **Failure / misuse conditions:** Over-pruning a list that was covering genuinely distinct legal categories.
- **Repair implication:** When pruning, require an explicit statement of which retained word covers each deleted word; otherwise leave and flag.
- **Proposed disposition:** retain.

#### AD1-08
- **ID:** AD1-08
- **Location:** ch 1, ¶1.57-1.61 (no explaining, storytelling or persuading; rhetorical emphasis); ¶1.62 (repetition); ¶1.63-1.64 (consistent usages)
- **Problem addressed:** Words that do no contractual work but can be argued to mean something; saying the same thing twice; same word/different meanings and different words/same meaning.
- **Principle / method / heuristic (own words):** Contract text regulates conduct, states facts and allocates risk; connective words of exposition or argument are suspect. Emphasis words that merely say "we really mean it" should be deleted or replaced by a plain negative/conditional. Emphasis by typography is also out. Never state the same thing twice (addresses, numbers, anything): it invites inconsistency and dispute. Redundancy (surplus words in one statement) is different from repetition (stating it twice). One word, one meaning; one meaning, one word — because readers and judges presume variation is meaningful.
- **Assumptions and applicability:** General; recitals are the one place narrative prose belongs (see AD1-10).
- **Production responsibility affected:** drafting, review/redlining, product consistency, change impact
- **Workflow / decision implication:** Lexical lint: intensifier list; duplicate statements of the same datum; term-variation map (same concept referred to by more than one expression; same expression used in more than one sense). On amendment, a duplicated datum is a change-impact hazard.
- **Evaluation evidence or criterion:** Document passes if every amount/date/address/period is stated once, and a concept-to-term table is one-to-one.
- **Failure / misuse conditions:** Deleting an apparent intensifier that is actually doing legal work in context (author notes the same word can be emphasis in one place and functional in another, e.g., "irrevocably" with appointments or ongoing consents, ¶3.43-3.45).
- **Repair implication:** Treat intensifier hits as prompts for a function check, not auto-deletes.
- **Proposed disposition:** retain.

#### AD1-09
- **ID:** AD1-09
- **Location:** ch 2, "The Introductory Clause": "Date" ¶2.23-2.47; "Identifying the Parties" ¶2.51-2.55; "Having a Parent Company Enter into a Contract on Behalf of an Affiliate" ¶2.57-2.60; "Parties with a Limited Role" ¶2.61-2.64; "Describing the Parties" ¶2.68-2.82; "Extraneous Information" ¶2.86-2.89; ¶2.123 (role labels)
- **Problem addressed:** Front-of-contract facts that look formal but carry risk: fictitious dates, wrong or non-existent parties, affiliates swept in by description.
- **Principle / method / heuristic (own words):** (i) Date: state the true signing date, or have signatures dated and say the contract is effective on last signature — not both. Do not use "as of", "effective date" or back/forward dating to capture pre-contract performance or delayed start; keep the real date and deal with timing in the operative provisions (and mention pre-contract performance in recitals and say the contract governs it). If stating what actually happened is awkward, something is wrong. Date manipulation can have consequences beyond the contract. (ii) Parties: full registered name, entity type, jurisdiction of organisation (registration number where that is the local identifier); individuals identified as such. Do not describe a party as "including its affiliates" — non-signatories are not bound and the phrase creates confusion; choose an actual structure for group contracting (separate contracts, guarantee, agency, sublicence, master agreement, accession undertaking). Flag a party whose role is limited to specified provisions, in both the introductory clause and signature block, so generic "the parties" wording does not snare it. A trust (generally) and a division are not legal persons: the trustee in that capacity, or the company, is the party. (iii) Role labels can carry substance (a label implying the claimant is itself compliant was read as a precondition in one case he cites).
- **Assumptions and applicability:** US formatting conventions; entity-capacity statements vary by jurisdiction (he notes exceptions). Commonwealth practice differs on layout.
- **Production responsibility affected:** scoping, drafting, review/redlining, issue spotting, escalation
- **Workflow / decision implication:** Intake must capture: exact legal names/registrations, who actually signs, whether any group members are meant to benefit or be bound, real signing date vs. commercial start date, and any pre-contract performance. Review must flag "as of"/"effective date" dates that differ from signing, affiliates-by-description, non-entity parties, and evaluative role labels.
- **Evaluation evidence or criterion:** Given a term sheet with a start date before signing and a parent "on behalf of its group", the draft uses the signing date plus an operative start-date provision, and raises the group-structure choice rather than writing "including its affiliates".
- **Failure / misuse conditions:** Treating his entity-capacity statements as law; ignoring mandatory local party-information requirements.
- **Repair implication:** Make party-capacity and dating questions explicit scoping questions; escalate capacity doubts.
- **Proposed disposition:** retain (method) / qualify (capacity and dating law are research questions).

#### AD1-10
- **ID:** AD1-10
- **Location:** ch 2, "Recitals", ¶2.129-2.159 (function ¶2.130-2.135; premature references ¶2.150-2.153; incorporation by reference ¶2.154-2.155; "true and correct" ¶2.156-2.157; defined terms ¶2.158-2.159); ch 3, ¶3.438
- **Problem addressed:** Operative content hiding in recitals; attempts to cure that by boilerplate.
- **Principle / method / heuristic (own words):** Recitals are background only: context, broad purpose, simultaneous transactions. They are the one place for plain narrative. Do not put deal terms, obligations or facts a party may need to rely on in recitals; if a fact matters, put it in the body as a statement of fact or acknowledgment by the right party. "Recitals are incorporated" and "recitals are true and correct" are weak repairs — move the content instead. A purpose recital should be a general intent, not tied to "the terms of this agreement", and must not state a purpose wider than the contract actually achieves. Do not use in recitals a defined term that is only defined later unless its meaning is obvious. Skip recitals entirely where there is no back-story.
- **Assumptions and applicability:** Rests on the premise that courts treat recitals as evidence of intent, not operative text (stated as general; he cites a New York case) — a research question per jurisdiction.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, product consistency
- **Workflow / decision implication:** Review check: any shall/must/may, amount, deadline or relied-on fact appearing only in recitals is a defect to relocate. Consistency check: purpose recital scope vs. operative scope.
- **Evaluation evidence or criterion:** Seeded recital containing a payment term: agent flags and relocates it, rather than adding an incorporation clause.
- **Failure / misuse conditions:** Deleting recitals that a governing law or registry treats as necessary; losing context courts would use.
- **Repair implication:** Relocate, don't delete; keep a short context recital.
- **Proposed disposition:** retain.

#### AD1-11
- **ID:** AD1-11
- **Location:** ch 2, "The Lead-In" — "Consideration", ¶2.166-2.210 (backstop recitals ¶2.171-2.174; structuring consideration ¶2.182-2.187; eliminating other references ¶2.202-2.206; other jurisdictions ¶2.207-2.210)
- **Problem addressed:** The boilerplate recital asserting unspecified "good and valuable consideration".
- **Principle / method / heuristic (own words):** The author labels this a "backstop" recital: it asserts that consideration exists without saying what it is, and he treats it as pretence alongside nominal and sham consideration. His drafting alternative is substantive rather than verbal: state the real exchange clearly in the body; if the deal (e.g., a one-sided amendment, a later-given guarantee, an option) lacks consideration, fix that in fact; consider reliance-based or formal routes only after researching governing law. Replace "in consideration of $X" formulas with an explicit statement of who pays what and when (as acknowledged receipt, or as an obligation). He frames reliance on presumptions as litigation-minded "passive drafting" versus drafting to avoid the dispute. He acknowledges cases going the other way and another commentator's contrary advice, and declines to follow them. Notes that the recital leaks into civil-law and English contracts by copy-paste.
- **Assumptions and applicability:** Entirely dependent on the law of consideration in the governing jurisdiction; he flags variations (option contracts, guarantees, England, civil law, specific US states).
- **Production responsibility affected:** issue spotting, drafting, research, escalation, risk communication
- **Workflow / decision implication:** The useful transferable check is not "delete the recital" but: *does each promise in this document have an identifiable exchange behind it?* Trigger scenarios: amendments disadvantaging one side, post-hoc guarantees, options, releases. If not, raise it as a substantive issue and route to research.
- **Evaluation evidence or criterion:** Given an amendment benefiting only one party under a common-law governing law, agent raises the enforceability question instead of relying on boilerplate.
- **Failure / misuse conditions:** Agent deletes the recital from a counterparty draft (contrary to AD1-03, which lists it as harmless) or asserts that it has no legal effect in a jurisdiction where that is unverified.
- **Repair implication:** Keep as issue-spotting trigger; remove any hard-coded "delete" behaviour.
- **Proposed disposition:** adapt — retain the issue-spotting trigger; the doctrinal claims go to research questions.

#### AD1-12
- **ID:** AD1-12
- **Location:** ch 3, ¶3.1-3.7 and Figure 1 "Quick Reference for the Categories of Contract Language"; ¶3.466 ("Selecting Which Category of Contract Language to Use")
- **Problem addressed:** Undisciplined verb use makes it unclear what each sentence in the body of a contract is doing.
- **Principle / method / heuristic (own words):** Every clause/sentence in the body performs one function, and each function should have its own verb structure. The author's categories and signals: **agreement** ("agree", once, in the lead-in); **performance** (hereby + present tense; acts done by signing); **obligation** on the sentence subject (shall = has a duty to) or on someone else (must; or "shall cause" by a controlling party); **discretion** (may; "is not required to" for absence of obligation; "is not prohibited from" for absence of prohibition); **prohibition** (shall not); **policy** (rules that do not direct conduct: present tense, or "will" for contingent/uncertain-timing events); **declaration** ("states" for own-knowledge facts; "acknowledges" for facts offered by the other side); **intention** ("intend that … will" where a court, not the parties, decides status); **recommendation**. **Conditions** are not a category but are expressed through conditional clauses, policy ("subject to the following conditions: that …"), or obligation-form with an explicit purpose clause. No category outranks another; they have different consequences on failure (e.g., failed condition blocks the dependent result; breached obligation gives damages). The scheme claims to reflect standard English adjusted for clarity, not grammar rules.
- **Assumptions and applicability:** Third-person B2B contracts in English. The specific verb assignments (especially shall/must/states) are the author's system; other reputable systems exist (see §4). The functional taxonomy is more portable than the verb choices.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, evaluation, product consistency
- **Workflow / decision implication:** A reviewer/drafter agent can (1) classify every operative sentence by function, (2) check that the verb structure matches the function under the *document's own* convention, (3) check that the function chosen produces the consequence the parties want. Step (3) is the high-value one.
- **Evaluation evidence or criterion:** Inter-run agreement on category labels over a test set; every operative sentence receives exactly one label or is flagged as mixed/unclear; mismatches between label and intended consequence are reported.
- **Failure / misuse conditions:** Enforcing Adams's verb tokens on a document that consistently uses another convention (e.g., "must"/"will" house style) — the defect is inconsistency and category confusion, not the token.
- **Repair implication:** Parameterise the verb-to-category map per document; keep the functional classification fixed.
- **Proposed disposition:** retain (taxonomy) / adapt (verb map configurable).

#### AD1-13
- **ID:** AD1-13
- **Location:** ch 3, "Use the Active Voice Unless the Passive Voice Is Appropriate", ¶3.11-3.24; ¶3.38; ¶3.151-3.152; ¶3.186; "Buried-Actor Policies" ¶3.309-3.311
- **Problem addressed:** Sentences that do not say who acts.
- **Principle / method / heuristic (own words):** The passive costs words and word order, but the serious cost is the dropped actor. His worked case: a trigger drafted as employment "is terminated" with no actor let the employee trigger a release from a non-compete by resigning — almost certainly not the buyer's intent. Whether the court was right is beside the point for the drafter. Writing actively forces the drafter to decide who does what. Passive is fine where the actor is genuinely irrelevant or unknown. The same actor-hiding happens with "receive", "is entitled to" + noun/passive, nominalised "breach of", and adjectives/phrases such as payable, exercisable, is due, is subject to, is eligible for: each leaves open who must act *and* whether the sentence is an obligation, a discretion or a condition.
- **Assumptions and applicability:** General.
- **Production responsibility affected:** drafting, review/redlining, issue spotting
- **Workflow / decision implication:** For every trigger, obligation, payment and termination event: name the actor. Review lint: agentless passives and buried-actor adjectives in operative text; for each, ask "who?" and "duty, permission, or condition?".
- **Evaluation evidence or criterion:** Seeded clause "if X's engagement is terminated …" — agent asks/flags by whom. Pass if every operative sentence has an identifiable responsible party or a stated reason why none is needed.
- **Failure / misuse conditions:** Mechanical conversion of every passive, including those where the actor is truly irrelevant; guessing the actor instead of asking.
- **Repair implication:** Where the actor is unknown, raise a question to the user; do not invent.
- **Proposed disposition:** retain — high-yield, testable.

#### AD1-14
- **ID:** AD1-14
- **Location:** ch 3, "Throat-Clearing", ¶3.25-3.28; ¶3.30-3.32; ¶3.375; ¶3.388; ¶3.439-3.441
- **Problem addressed:** Lead-in verbs ("X agrees that", "it is agreed that", "X covenants/represents/acknowledges/warrants and agrees that …") stacked in front of a sentence that already has its own operative verb.
- **Principle / method / heuristic (own words):** The prefixed verb is neutralised by the real verb that follows; all it signals is assent, which the lead-in already supplies once for the whole contract. It adds clutter and can be mistaken for the operative category (agreement, declaration, warranty), and he cites a case where a court gave such a prefix substantive weight. "Acknowledges" should introduce only a fact offered by the other side, never an obligation or policy, and never be paired with another verb.
- **Assumptions and applicability:** General.
- **Production responsibility affected:** drafting, review/redlining
- **Workflow / decision implication:** Strip in own drafts; on counterparty drafts flag only where the prefix could change the perceived category (e.g., "represents that it shall …").
- **Evaluation evidence or criterion:** Pattern detection of [party + agree/covenant/represent/warrant/acknowledge + that + clause containing shall/may/must/will]; classification of the clause by its inner verb.
- **Failure / misuse conditions:** Removing a true acknowledgment or a true statement of fact.
- **Repair implication:** Classify by inner clause first; delete prefix only if inner clause is itself a complete category sentence.
- **Proposed disposition:** retain.

#### AD1-15
- **ID:** AD1-15
- **Location:** ch 3, "Language of Performance", ¶3.33-3.69 (hereby ¶3.35-3.37; problematic usages ¶3.38-3.45; actions that don't work ¶3.46; absence ¶3.47; future ¶3.48; granting language ¶3.55-3.60; "hereby grants the right to" ¶3.258-3.259)
- **Problem addressed:** Confusion between doing something by signing and promising to do it.
- **Principle / method / heuristic (own words):** Acts effected by the contract itself (sell, grant, assign, waive, release, appoint) are speech acts: present tense with "hereby". "Agrees to [assign]" is dangerous because it can be read as either a present act or a promise, and he notes that reading has been litigated. Do not dress an obligation as performance by adding "on the date of this agreement". Only changes of status can be done by saying so — payment cannot. To say a party is *not* doing something at signing, use a policy statement, not a negated performative. For effects triggered by a future event, use "will be deemed". "Irrevocably" etc. are usually redundant in performatives, except for appointments and consents to continuing conduct. Reserve grant-of-licence wording for IP/software contexts where sublicensing and adjectives (exclusive, perpetual) matter; elsewhere "X may …" is shorter and clearer than "Y hereby grants X the right to …".
- **Assumptions and applicability:** The present-assignment vs. promise-to-assign distinction has real legal consequences that vary by subject matter and jurisdiction (research question).
- **Production responsibility affected:** drafting, review/redlining, issue spotting
- **Workflow / decision implication:** For transfer/grant/release/waiver clauses, the agent must determine whether the parties intend a present act or a future obligation and draft accordingly; flag "agrees to assign/grant/release".
- **Evaluation evidence or criterion:** Seeded "Consultant agrees to assign all inventions": agent flags the ambiguity and asks or proposes both variants with consequences.
- **Failure / misuse conditions:** Converting to a present assignment where the subject matter cannot yet be assigned or formalities are required.
- **Repair implication:** Pair with research hand-off on assignability/formalities.
- **Proposed disposition:** retain.

#### AD1-16
- **ID:** AD1-16
- **Location:** ch 3, "Language of Obligation Imposed on the Subject of a Sentence", ¶3.72-3.116, esp. "Using Shall to Mean Only Has a Duty To" ¶3.72-3.75, "The Problem of Overuse" ¶3.80-3.81, ¶3.87, "Applying the Has a Duty Test—An Example" ¶3.104-3.108; ¶3.125-3.130
- **Problem addressed:** "Shall" used for obligation, futurity, policy, conditions and more, so readers cannot tell duties from everything else.
- **Principle / method / heuristic (own words):** Use "shall" only to impose a duty on the party that is the sentence's subject. Diagnostic: substitute "has a duty to"; if the sentence stops making sense, "shall" is misused. Passing the test is necessary but not sufficient — the provision may still be better framed as a condition. The author's argument for keeping "shall" (against abolitionists): removing it yields only modest benefit; "must" would then serve both duties and conditions, and "will" both duties and futurity, recreating the multi-meaning problem; the one overuse that routinely produces litigation is obligation-vs-condition uncertainty, which swapping verbs does not cure. He claims discretionary readings of "shall" arise mainly with statutes, not contracts, and calls a contrary contract case an outlier. His worked example: applying the test to a standard arbitration clause exposes not just a verb problem but a deal-logic problem (an agentless passive, and a "duty to arbitrate every dispute" nobody intends), leading to a redraft as an exclusive discretion to demand arbitration. Also rejected as obligation forms: agrees to, undertakes to, covenants to, is obligated to, is responsible for (ambiguous about source of duty; acceptable as policy to allocate a liability owed to a non-party), will be expected to, simple present, imperative mood.
- **Assumptions and applicability:** Third-person B2B contracts. Expressly contested (Garner, Asprey; Australian practice; NEC and CSI conventions). Not for consumer documents, where he concedes eliminating "shall" may be right.
- **Production responsibility affected:** drafting, review/redlining, evaluation
- **Workflow / decision implication:** Use the substitution test as a *diagnostic that surfaces category errors*, regardless of house verb. In a "must"/"will" house style, the analogous test is: can the sentence be restated as "[party] has a duty to …"? If not, it is not an obligation and should not be drafted like one.
- **Evaluation evidence or criterion:** Every sentence tagged "obligation" has a party as grammatical subject and survives the substitution; every "shall" not surviving is reclassified (policy / condition / discretion) with a proposed rewrite.
- **Failure / misuse conditions:** Global find-and-replace of shall; treating test passage as proof the provision is correctly an obligation.
- **Repair implication:** After the test, run the condition-vs-obligation consequence check (AD1-22).
- **Proposed disposition:** adapt — keep the test; make the verb token configurable; record that the prescription is contested.

#### AD1-17
- **ID:** AD1-17
- **Location:** ch 3, "Language of Obligation Imposed on Someone Other Than the Subject of a Sentence", ¶3.131-3.154 (five contexts ¶3.131-3.136; "Avoiding the Need for Must" ¶3.141-3.150); ¶3.448
- **Problem addressed:** Sentences that purport to bind things, non-parties, or nobody in particular.
- **Principle / method / heuristic (own words):** A duty lands on someone other than the grammatical subject when: the sentence is passive; the subject is a thing/event; the subject is a non-party; the verb is "receive"; or "is entitled to" is used with a noun/passive. Preferred repair: recast actively with the obligor as subject. Where an event or a non-party must do something, a party may be made to "cause" it — but only where the party genuinely controls the actor (e.g., a wholly owned subsidiary). A party does not control individuals (employees, arbitrators) or unaffiliated entities; an obligation to control the uncontrollable is an invitation to dispute even if a court might enforce it. Restructuring often exposes issues the loose wording glossed over (e.g., what happens if an employee refuses to sign). If no restructuring works, use "must" and spell out the consequence of the non-party's failure, since remedies will not be evident. "Is entitled to" framing can also hand the obligor an argument that performance had to be requested first.
- **Assumptions and applicability:** Assumes privity-type limits (non-parties cannot be bound); statutory third-party regimes vary.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, risk communication
- **Workflow / decision implication:** For each obligation: is the grammatical subject a party? If not — who is the obligor, do they control the outcome, and what happens if the outcome fails? Flag "shall procure/ensure/cause" directed at persons the party does not control.
- **Evaluation evidence or criterion:** Seeded "Supplier's subcontractors shall comply with …": agent identifies that subcontractors are non-parties, proposes party-facing obligation plus consequence/risk allocation.
- **Failure / misuse conditions:** Assuming corporate control from a group relationship without facts.
- **Repair implication:** Ask about control; otherwise pair a realistic obligation with explicit risk allocation (see AD1-18).
- **Proposed disposition:** retain.

#### AD1-18
- **ID:** AD1-18
- **Location:** ch 3, "Imposing Impossible Obligations" ¶3.155-3.158; "Imposing Obligations to Stop Something from Happening" ¶3.159-3.163; "Statements of Fact—Alternatives To" ¶3.430-3.431
- **Problem addressed:** Using an absolute obligation (or a statement of fact) for an outcome the party does not control.
- **Principle / method / heuristic (own words):** Before choosing wording, ask whether an obligation is the right tool at all. If the obligor cannot ensure the outcome (third-party consent; total deletion of electronic data; preventing employee misconduct), a flat duty is confusing and may not be enforced. Decompose into: (1) a conduct obligation the party *can* perform (an efforts-type duty); (2) where relevant, a condition tied to the outcome; (3) an explicit risk-allocation term for what happens if the outcome fails anyway (fee, indemnity, liability). "Shall not permit/allow", "shall prohibit", "shall prevent" each leave open what level of action is required and who bears residual risk — two issues needing two provisions. Similarly, a "statement of fact" about something outside the maker's control is disguised risk allocation and is better written as such.
- **Assumptions and applicability:** General commercial. Efforts standards are treated elsewhere in the book (ch 8, outside my range) and are jurisdiction-sensitive.
- **Production responsibility affected:** issue spotting, drafting, review/redlining, risk communication
- **Workflow / decision implication:** Control test on every outcome-type obligation and every forward-looking or third-party-dependent statement of fact; propose the conduct + condition + risk-allocation decomposition and ask the user which risk allocation is intended.
- **Evaluation evidence or criterion:** Seeded "Seller shall obtain landlord's consent": agent flags lack of control and offers the three-part structure.
- **Failure / misuse conditions:** Softening an obligation the client deliberately wants as a strict outcome guarantee — the point is to make the allocation explicit, not to pick a side.
- **Repair implication:** Present as options with consequences; never silently weaken.
- **Proposed disposition:** retain.

#### AD1-19
- **ID:** AD1-19
- **Location:** ch 3, "Language of Discretion", ¶3.187-3.223 ("Be Explicit as to Whether Discretion Is Limited" ¶3.190-3.200; "The Ambiguity Inherent in May … Only" ¶3.201-3.205; "Using May to Convey Possibility" ¶3.206-3.214; "May Require" / "May Request" ¶3.215-3.223); "When Exercising Discretion Requires Cooperation" ¶3.260-3.261; "Is Entitled To" ¶3.264-3.267; "Is Not Required To" ¶3.268-3.276; "Is Not Prohibited From" ¶3.277
- **Problem addressed:** A permission may or may not imply that everything else is forbidden; "may" has several readings.
- **Principle / method / heuristic (own words):** A grant of discretion does not logically exclude other options, but readers presume an utterance is relevant: the more specific the permission (or the more alternatives listed), the more likely it will be read as exhaustive, and a court may reach the same result through an expression-of-one-excludes-others canon. His example is a forum clause saying a party "may" sue in a named court. Rule: say expressly whether discretion is limited ("to any person" / "the only person to whom … is" / or use a prohibition). "May … only" is structurally ambiguous and cannot be fixed by moving "only"; rewrite. "May" for possibility: restructure as a conditional or use "might"; he judges the residual risk low and keeps "may" for discretion. "X may require Y to …" is really Y's obligation on X's request — write it that way; "may request" with no stated consequence leaves open whether compliance is required. Where exercising a permission needs the other side's cooperation (inspection, option exercise, board seat), state the cooperating party's obligation. Absence of obligation ("is not required to") ≠ discretion to refuse ≠ obligation on the other party; for capped performance, state what must be done with the cap, not a limit on the other side's conduct. If a party could do the thing anyway without the contract, "is not prohibited from" avoids implying the right derives from the contract.
- **Assumptions and applicability:** General. Exhaustiveness presumptions are interpretive-law questions by jurisdiction.
- **Production responsibility affected:** drafting, review/redlining, issue spotting
- **Workflow / decision implication:** For every "may" clause (esp. jurisdiction, notice methods, assignment, termination rights): is it exhaustive? say so. For every permission: does it need a counterpart obligation? For every "may require/request": who must do what on request?
- **Evaluation evidence or criterion:** Seeded non-explicit forum or notice-method clause: agent flags the exclusive/permissive ambiguity and offers both explicit versions.
- **Failure / misuse conditions:** Agent guesses exclusivity instead of surfacing the choice.
- **Repair implication:** Make exhaustiveness a required attribute of each discretion clause in the drafting schema.
- **Proposed disposition:** retain — highly testable.

#### AD1-20
- **ID:** AD1-20
- **Location:** ch 3, "Don't Use At Its Sole Discretion with May", ¶3.224-3.257 (implied duty of good faith ¶3.225-3.227; wording ¶3.228-3.232; attempting to circumvent ¶3.233-3.235; caselaw ¶3.236-3.241; "An Alternative Approach" ¶3.242-3.254; use outside language of discretion ¶3.255-3.257)
- **Problem addressed:** "In its sole/absolute discretion" as either empty emphasis or a veiled attempt to escape a good-faith constraint on contractual discretion.
- **Principle / method / heuristic (own words):** Decide which it is. If emphasis, delete. If it is trying to secure unreviewable discretion, the phrase is an unstable tool: by the author's account courts split on whether it displaces an implied good-faith duty, the outcome is hard to predict even within one state, and apparent endorsement of bad faith can itself fuel a dispute. Better: identify the real concern and address it explicitly — either condition the discretion on objective criteria, or have the other side acknowledge the specific adverse effects the exerciser need not take into account. Where neither works (highly subjective approvals with no cost to refusing), the prudent move is to restructure the deal to remove the open-ended discretion. If explicit drafting is not possible, either keep the phrase and warn the client it may not work, or (his preference) omit it. "Reasonable discretion" may be *more* constraining than good faith. He would omit it even when it favours his client.
- **Assumptions and applicability:** Turns on whether the governing law implies a good-faith duty in performance and whether it can be excluded — he says most US states and the UCC do, England does not. Pure research territory.
- **Production responsibility affected:** issue spotting, drafting, review/redlining, research, risk communication, escalation
- **Workflow / decision implication:** On encountering discretion qualifiers, the agent asks what the client is trying to protect against, proposes the explicit-criteria or explicit-acknowledgment routes, and sends the enforceability question to research. It should not advise that the phrase is either effective or ineffective.
- **Evaluation evidence or criterion:** Agent output on such a clause contains (a) the purpose question, (b) an explicit alternative, (c) a governing-law caveat. Fail if it states a legal conclusion about good faith without a source.
- **Failure / misuse conditions:** Deleting the phrase from a client-favourable clause without telling the client what may be lost in jurisdictions that honour it.
- **Repair implication:** Make deletion a recommendation with stated trade-off, never silent.
- **Proposed disposition:** qualify — method is sound; the legal premise and the "omit even if it helps your client" stance are contested and jurisdiction-bound.

#### AD1-21
- **ID:** AD1-21
- **Location:** ch 3, "Language of Prohibition", ¶3.278-3.304 (may not ¶3.279; is not entitled to ¶3.280-3.282; shall refrain ¶3.283-3.284; hereby waives the right to ¶3.285-3.290 and ¶3.262; shall never ¶3.291; collective nouns ¶3.295-3.297; exceptions ¶3.302-3.304)
- **Problem addressed:** Ambiguous or indirect ways of forbidding conduct; exceptions that do not actually prohibit.
- **Principle / method / heuristic (own words):** Express prohibition directly on the party ("shall not"). "May not" has three readings (might not / permitted not to / not permitted to). "Shall never" does not reliably mean "survives termination" — if perpetual or post-termination effect is intended, say so expressly. "Hereby waives the right to [do X]" is usually a roundabout prohibition (or, in other uses, a roundabout way of saying the other side is not required to do something); he tolerates it for jury-trial waivers because it is universal. An exception carved out of a *permission* probably implies prohibition, but say "except that it shall not …" to be safe; an exception carved out of an *obligation* does **not** imply prohibition at all — it merely removes the duty — so an express prohibition is required. With "neither party"/"no shareholder" subjects he prefers "may" over "shall" (because "shall" with a negative subject reads as no duty), while admitting the inconsistency; with plural subjects beware collective-vs-individual readings and "their".
- **Assumptions and applicability:** General English-language drafting.
- **Production responsibility affected:** drafting, review/redlining, issue spotting
- **Workflow / decision implication:** Review check on every "except"/"other than" carve-out: is the excluded item meant to be forbidden, permitted, or merely unregulated? Check every "never"/"at no time" for intended survival.
- **Evaluation evidence or criterion:** Seeded "Distributor shall sell all Products except Product Z": agent asks whether selling Z is prohibited and drafts accordingly.
- **Failure / misuse conditions:** Assuming prohibition where the parties intended silence.
- **Repair implication:** Surface the three possibilities and ask.
- **Proposed disposition:** retain.

#### AD1-22
- **ID:** AD1-22
- **Location:** ch 3, "Expressing Conditions", ¶3.313-3.370: conditional clauses ¶3.316-3.326; positive vs negative matrix clause ¶3.327-3.336; "Using Unless with Language of Obligation Denoting Activity" ¶3.337-3.350; policy used for closing conditions ¶3.351-3.355; "Language of Obligation Used to Express Conditions" ¶3.356-3.362; "A Condition Doesn't Make Sense If It Can Be Ignored" ¶3.363-3.368; "A Condition Might Not Be the Only Condition" ¶3.369-3.370; also ¶3.3, ¶3.74, ¶3.87, ¶3.467-3.468
- **Problem addressed:** Provisions where it is unclear whether non-compliance means *breach (damages)* or *the dependent right/obligation never arises*. The author identifies this as the one "shall" problem that routinely produces disputes.
- **Principle / method / heuristic (own words):** Decide the intended consequence first. If late/non-compliance should simply bar the benefit (reimbursement, right to dispute an invoice, validity of an amendment or notice), draft a condition; if it should give the other side a claim, draft an obligation. He reports that courts faced with doubt tend to find an obligation, so a bare "must" (and still more a bare "shall") is unsafe: add an explicit purpose clause ("To be reimbursed, …"; "For … to be valid, …") or state the forfeiture expressly; a time-limited obligation on the payer is less clear because it is silent on late items. A condition only makes sense where the conditioned act cannot happen without the other side's participation; if the party can simply go ahead regardless, use an obligation so there is a remedy. A stated condition may not be the only one. Closing conditions: introduce as conditions and draft each as a "that"-clause in present/present perfect, not "shall have" sentences that could be read as statements of fact or duties. Conditional clauses: present tense in the if-clause (no "shall", "should" or subjunctive); "will" in the main clause where it would otherwise be present tense; for stative verbs add "at any time" or switch to a dynamic verb. "X may … only if Y" and "X shall not … unless Y" each leave a gap filled only by inference; the explicit form is "shall not …, except that it may … if …". With continuing-activity obligations, "unless" naturally reads as ending the duty rather than as a precondition to it arising — replace with "except that if …, [party] will no longer be required to …". Avoid the labels "condition precedent/subsequent".
- **Assumptions and applicability:** The default-to-obligation tendency and consequences of failed conditions are doctrines stated from US secondary sources; verify per jurisdiction. He notes English law's own terminology for conditions is a different topic.
- **Production responsibility affected:** issue spotting, drafting, review/redlining, risk communication, evaluation
- **Workflow / decision implication:** For every deadline, notice, invoice, claim-procedure, consent and amendment clause: ask "what should happen on failure — claim for damages, or loss of the right?" and draft to that answer with an explicit signal. This is a top-priority review check (the author also lists it first among things worth flagging in a counterparty draft).
- **Evaluation evidence or criterion:** Seeded "Contractor shall submit claims within 30 days": agent identifies the obligation/condition ambiguity, states both consequences, and offers a condition-form redraft. Pass/fail on detection plus correct description of the differing consequences *as drafting alternatives*, not as statements of law.
- **Failure / misuse conditions:** Converting to a condition a requirement the party can ignore; creating harsh forfeitures the client did not intend; stating the judicial default as settled law.
- **Repair implication:** Always present as a choice with consequences; route enforceability of forfeiture to research.
- **Proposed disposition:** retain — core review check.

#### AD1-23
- **ID:** AD1-23
- **Location:** ch 3, "Language of Policy", ¶3.305-3.312; "Shall and May in Restrictive Relative Clauses" ¶3.456-3.462; ¶3.218
- **Problem addressed:** "Shall" in sentences that impose no duty; tense confusion; modal verbs in relative clauses creating unintended scope.
- **Principle / method / heuristic (own words):** Policies are rules the parties must observe that do not themselves direct conduct: either rules about a thing/event/circumstance (e.g., a purported transfer is void) or rules about the contract's scope, meaning or duration (governing law, definitions, entire agreement, term). Use present tense for rules effective on signing or at a fixed date; "will" for contingent events or uncertain timing; never "shall". Where the missing actor in a passive policy is "the world", use "automatically" or an intransitive active verb so no one thinks a party must act. In restrictive relative clauses use the simple present: "shall" there is a misplaced future; "may" there is either redundant or — as one court he cites held — widens the class to anything that merely *might* qualify. If the real issue is whether after-acquired items are covered (stative verb "owns"), say so expressly.
- **Assumptions and applicability:** General. Tense conventions are stylistic; the scope-widening risk is substantive.
- **Production responsibility affected:** drafting, review/redlining
- **Workflow / decision implication:** Lint for modal verbs inside "that/which …" clauses defining a class; check every class definition with a stative verb for the present-vs-future-acquired question.
- **Evaluation evidence or criterion:** Seeded "any entity with which Tenant may merge": agent flags scope ambiguity. Seeded "Shares it owns": agent asks about after-acquired shares.
- **Failure / misuse conditions:** Treating tense preferences as substantive errors in a counterparty draft (contrary to AD1-03).
- **Repair implication:** Tier: scope-affecting = flag; tense-only = own-draft fix only.
- **Proposed disposition:** retain (scope issues) / merge (tense rules into house-style profile).

#### AD1-24
- **ID:** AD1-24
- **Location:** ch 3, "Language of Declaration", ¶3.371-3.441: "Statements of Fact—Using Represents and Warrants" ¶3.374-3.376; remedies ¶3.377-3.379; "The Remedies Rationale" ¶3.380-3.397; "The Timeframe Rationale" ¶3.398-3.404; "English Law and Practice" ¶3.405-3.411; "Using States" and "Addressing Remedies Directly" ¶3.412-3.429; related terminology ¶3.432-3.435; acknowledgments ¶3.436-3.441; also ch 1 ¶1.14, ¶1.21
- **Problem addressed:** Whether the verbs "represents" and/or "warrants" determine which remedies attach to an inaccurate statement of fact.
- **Principle / method / heuristic (own words):** The author identifies two explanations offered by others — that the verb selects the remedy (in a permissive or a restrictive version), or that the verbs track past/present vs. future facts — and argues both fail for US contracts: they extend warranty law beyond its domain, would let labels override the legal elements of each claim, lack US case support, and ask the verb to do something English verbs do not do; the near-universal use of the couplet even where indemnification is the exclusive remedy suggests drafters are not making a choice at all. For England he reports significant (not unanimous) judicial and practitioner support for the restrictive view — i.e., using only "warrants" to try to exclude misrepresentation-based remedies — and cites decisions on both sides, while maintaining it is unsound in principle. His prescription: introduce facts with the neutral verb "states"; if remedies matter, provide for them expressly (allow/exclude claim types, no-reliance, indemnity, caps); optionally add a sentence that the introducing verb does not affect remedies — also useful when stuck with the traditional verbs. He concedes this is "shockingly novel" to many, that the traditional couplet may be tolerable in high-value one-off deals, and that whether express remedy provisions are worthwhile or enforceable is uncertain and outside the book's scope. Separately: statements of fact are accurate or inaccurate, not "breached", cannot "become" inaccurate, and cannot be "cured" — so cure mechanics lumping them with obligations are conceptually off. "Acknowledges" is for accepting a fact the other side asserts, and he says it precludes later challenge.
- **Assumptions and applicability:** Strongly US-centred; by the author's own account English practice attaches consequences to the label. Among the most contested positions in the book.
- **Production responsibility affected:** drafting, review/redlining, research, authority verification, risk communication, escalation
- **Workflow / decision implication:** An agent should **not** replace "represents and warrants" with "states" by default, and should not tell a user the verb is legally irrelevant. What transfers: (1) do not rely on the introducing verb to allocate remedies — check whether the document deals with remedies expressly (exclusive remedies, non-reliance, limitations) and whether that matches intent; (2) under English or similar law, treat the choice of "warrants" vs "represents" as potentially operative and escalate; (3) check cure/survival mechanics for statements of fact for coherence; (4) flag statements of fact about matters outside the maker's control (AD1-18).
- **Evaluation evidence or criterion:** On a share purchase agreement governed by English law, agent does not normalise the verbs and flags the remedy implication for specialist review; on any draft, agent reports whether remedies for inaccurate statements are expressly addressed.
- **Failure / misuse conditions:** House-style normalisation that changes "warrants" to "represents and warrants" (or to "states") in a jurisdiction where labels matter.
- **Repair implication:** Lock these verbs against automated style edits; require governing-law-aware human sign-off.
- **Proposed disposition:** qualify / research further — retain the "address remedies expressly" check; reject automatic verb substitution.

#### AD1-25
- **ID:** AD1-25
- **Location:** ch 3, "Language of Intention" ¶3.442-3.451; "Language of Recommendation" ¶3.452-3.455; "Stating How a Court Is to Conduct Itself" ¶3.470-3.481
- **Problem addressed:** Provisions that purport to fix matters the parties cannot fix (legal characterisation; what a court must do).
- **Principle / method / heuristic (own words):** Where status is a question of law and fact for a tribunal (his example: independent contractor vs. employee), none of obligation, policy, acknowledgment or belief fits; the honest form is that the parties *intend* the status, which a court may weigh. By contrast, where the parties' choice governs unless it fails minimum legal requirements (governing law), ordinary policy language is right. Provisions that tell a court what it may, must or must not do ("shall be construed", "shall be entitled to specific performance/injunctive relief", "no court shall …") are attempts to bind a non-party that will do as it sees fit; he cites a Delaware decision refusing to be bound by a stipulated entitlement. Reframe as the parties' acknowledgment of what they would want a court to do. Recommendation language ("recommends that … consult an adviser") is a tool for a stronger party to reduce later dispute; avoid "advises" because it suggests a relationship of trust.
- **Assumptions and applicability:** General common-law; the weight given to such statements is jurisdiction-specific.
- **Production responsibility affected:** drafting, review/redlining, risk communication, issue spotting
- **Workflow / decision implication:** Flag clauses that characterise legal status or direct a court, and tell the user plainly that such clauses express intent and may not be effective; do not present them as securing the outcome.
- **Evaluation evidence or criterion:** Agent's explanation of an equitable-relief or contractor-status clause includes the "not binding on the tribunal" caveat.
- **Failure / misuse conditions:** Over-rewriting standard boilerplate in counterparty paper; implying the clause is worthless.
- **Repair implication:** Treat as risk-communication item, low redline priority.
- **Proposed disposition:** retain.

#### AD1-26
- **ID:** AD1-26
- **Location:** ch 3, "Selecting Which Category of Contract Language to Use", ¶3.466-3.469 and ¶3.482; "Not a Category of Contract Language: Assumptions" ¶3.463-3.465; "Consolidating Deal Points" ¶3.29
- **Problem addressed:** Drafters pick a sentence form by habit rather than by the consequence they want.
- **Principle / method / heuristic (own words):** Make it routine to ask, per provision, which category fits, by running the candidates and asking what each implies on non-compliance. Worked examples: (a) amendment formalities — discretion or prohibition forms presuppose breach and a remedy, which is nonsensical; a condition or policy form ("will be effective only if…") fits; (b) a deadline for a dispute notice — obligation form wrongly implies a damages claim for lateness; condition form fits; (c) landlord's consent not to be unreasonably withheld — prohibition gives the tenant only a claim; an express permission to assign if consent is unreasonably withheld gives self-help and leverage. Statement-of-work "assumptions" are not a category at all: each leaves open whether it is a condition, an obligation or something else, and should be recast — acknowledging this is organisationally hard because different teams own SOWs. Several deal points sharing an actor can be consolidated under one verb structure.
- **Assumptions and applicability:** General. Example (c) depends on local landlord-tenant law.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, evaluation
- **Workflow / decision implication:** Build the "enumerate candidate categories → state consequence of each → pick" routine into drafting of any procedural or gatekeeping provision; in SOW review, convert each assumption into an explicit question ("if this turns out false, then what?").
- **Evaluation evidence or criterion:** For a set of SOW assumptions, agent output assigns each a proposed category and a stated consequence, or a question to the user.
- **Failure / misuse conditions:** Agent decides the commercial consequence itself.
- **Repair implication:** Output options + questions, not unilateral recasting.
- **Proposed disposition:** retain — this is the chapter's method distilled.

---

### 3. Substantive-law statements noted (research questions only)

None of these is recorded as a finding about the law. Each is a question to verify for the relevant jurisdiction and date.

1. Does a bare recital of "good and valuable consideration" establish, create a rebuttable presumption of, or do nothing for, consideration? (¶2.175-2.181; author reports a traditional view, a presumption line, and recent contrary US decisions.)
2. Do nominal-consideration recitals support option contracts and guarantees (Restatement-based approach; asserted minority position), and which states dispense with consideration for options or firm offers by statute? (¶2.191-2.201)
3. Is nominal consideration sufficient under English law; what is the position for contract modifications? (¶2.183, ¶2.209)
4. Is a stated intention to be legally bound relevant to formation — US general position, Pennsylvania's statute and its judicial limits, England's presumption for commercial agreements, civil-law systems? (¶2.87-2.89, ¶2.186)
5. Can a parent's signature bind or expose non-signatory group members where the contract is expressed to be for their benefit (Delaware decision cited)? (¶2.59-2.60)
6. Capacity of trusts and unincorporated divisions to contract; trustee personal liability; statutory trusts. (¶2.78-2.82)
7. Civil/criminal exposure from misdating contracts; effect of retroactive dating within a chain of transfers. (¶2.46-2.47)
8. Are recitals part of the operative contract, and what does "incorporating" them achieve? (¶2.135, ¶2.154)
9. Mandatory party-identification content under particular national laws (Czech example). (¶2.74)
10. Is "shall" ever construed as non-mandatory in a *contract* (as opposed to a statute)? (¶3.73, ¶3.86)
11. In doubt, do courts construe a provision as a promise rather than a condition; when will forfeiture-type conditions be enforced? (¶3.359-3.362)
12. Present assignment vs. agreement to assign — consequences (patent case cited). (¶3.109)
13. Is a contractual consent irrevocable by default at common law? (¶3.43)
14. Liability under a "shall cause" obligation for conduct of an uncontrolled individual (S.D.N.Y. case cited). (¶3.147)
15. Implied duty of good faith in exercising contractual discretion: which jurisdictions recognise it (author: most US states and UCC yes, England no), whether "sole and absolute discretion" displaces it (California and Georgia cases vs. New York case), UCC limits on disclaimer and permission to set standards. (¶3.225-3.251)
16. Is a "reasonableness" standard stricter than good faith? (¶3.231)
17. Exclusive vs. permissive forum-selection wording; whether a list of notice methods is exhaustive (English Court of Appeal case cited). (¶3.195-3.200)
18. Misrepresentation vs. breach-of-warranty: elements, remedies (rescission, damages measure, limitation periods), reach of "warranty" law beyond goods; UCC rule that formal words are not needed for an express warranty. (¶3.377-3.401, ¶3.422)
19. English law: does labelling statements "warranties" only prevent a misrepresentation claim (Sycamore Bidco, Idemitsu, MAN Nutzfahrzeuge vs. Invertec)? Current position needs checking — the book is 2017. (¶3.405-3.411)
20. Enforceability of contractual exclusion of remedies and of no-reliance clauses (US, England). (¶3.414, ¶3.423-3.424)
21. Does an acknowledgment of fact estop later challenge? (¶3.437)
22. Weight of parties' stated intent in worker-status determinations. (¶3.445-3.450)
23. Grounds on which a court overrides a governing-law choice. (¶3.451)
24. Effect of contractual stipulations of irreparable harm / entitlement to specific performance or injunction (Delaware Chancery decision cited). (¶3.478-3.479)
25. Jury-trial waiver mechanics (federal procedure). (¶3.289)
26. Whether a registry will reject a merger filing because the agreement's title omits "plan of merger". (¶2.9)
27. Whether an evaluative party label (e.g., "non-breaching party") can import a compliance precondition (N.D. Cal. case cited). (¶2.123)
28. Whether expert evidence on contract language is admissible on ambiguity. (Introduction, "Underestimating Complexity")

---

### 4. Material the author marks as contested, or where the author criticises other approaches

- **"Tested"/"settled" language** — quotes and rejects a law-review author's view that redrafting judicially interpreted wording increases uncertainty; calls the position a platitude. Also says inertia, learned helplessness, cognitive dissonance and peer pressure explain resistance. The author's dismissal of outlier cases ("no reason … to retreat") is itself a contestable risk posture.
- **Plain English** — declines the label; criticises a practitioner text (Fox) for treating clearer commercial drafting as a misapplied consumer movement.
- **"Shall"** — openly "contentious". Against him: Garner (abolish; most lawyers cannot use it consistently; suggests "will" for contracts), Asprey (use "must"), and Australian practice. He also rejects the CSI guide's imperative mood for specifications and the NEC's simple-present convention. His claim that no real flight from "shall" is under way rests on an admittedly unscientific sample.
- **"Represents and warrants"** — rejects Stark's remedies rationale, Garner's stricter version, and the ABA Model Stock Purchase Agreement's timeframe rationale; reports that English courts/practitioners give substantial support to the restrictive view and criticises that reasoning; notes another practitioner's (West) "leave it alone, use non-reliance" view and concedes it may suit large one-off deals. Replacement with "states" is acknowledged as novel.
- **Recital of consideration** — rejects Stark's advice to include it where a rebuttable presumption is recognised; treats contrary recent cases as courts "misinformed" or outcome-driven.
- **"Sole discretion"** — concedes caselaw is mixed and that policy arguments run both ways; recommends omission even when the phrase favours one's client.
- **Terms of art** — accuses courts and lawyers of inventing distinctions (hold harmless; graded efforts standards) via over-zealous application of the every-word-has-meaning canon. Treated more fully in chapters outside my range.
- **Judges** — repeatedly described as overconfident about English; several cited decisions are called mistaken (e.g., the "unless" case at ¶3.347; throat-clearing case at ¶3.28; "shall can mean should" at ¶3.73).
- **Drafting "style" / lawyer autonomy** — argues individual style is illegitimate for the building blocks of contract language.
- **Commonwealth conventions** — recommends dropping tabulated/headed introductory clauses, "procure", "clause", "endeavours", "whilst", headings for the operative part; these are preferences against established UK/Commonwealth practice.
- **Minor conventions he knows are provocative** — lowercase "this agreement" with no defined term; "between" for multi-party contracts; "wants to" in purpose recitals; no "the Parties" defined term; "obligation" not "covenant"; "comply with" not "perform".
- **Industry resources** — dismisses crowdsourced drafting, free repositories, SEC EDGAR precedents, clause-comparison tools and "BigLaw" curated templates as quality sources; promotes style-guide-compliant automated templates (including his own product — a commercial interest).

---

### 5. Content in the assigned range that is out of scope for legal production (and why)

- Preface tail (list of edition changes) and Acknowledgments (pdf 36-38): bibliographic/personal.
- Promotion of the author's forthcoming short style guide, NDA template and blog (Introduction): commercial, not method.
- Pure typographic/formatting conventions for the front of the contract — title capitalisation, all-caps party names, bolded defined terms in quotation marks, date format, placement of the defined-term parenthetical, cover sheet and table of contents (¶2.2-2.8, ¶2.20, ¶2.31-2.32, ¶2.52, ¶2.93-2.94, ¶2.214-2.217): house-style matters with no bearing on legal-production reasoning; could feed a formatting profile but not a skill.
- Choice of defined-term labels for parties, honorifics, initialisms, Vendor/Seller/Supplier, Employee/Executive (¶2.98-2.109): style; only the confusable -or/-ee pairs point (¶2.105) has marginal error-prevention value.
- Etymology and history (witnesseth, whereas, know all men, origins of doublets, history of shall/will) (¶1.39-1.40, ¶2.16, ¶2.137-2.138, ¶3.76-3.79): background.
- Fine grammar preferences with no meaning impact: "grant" vs "grant to" (¶3.64-3.69, which the author himself says little rides on); "breach" as count noun/mass noun/verb (¶3.176-3.185, except the actor-dropping point at ¶3.186); choice of verb in purpose recitals (¶2.145-2.149); "obligation" vs "duty" (¶3.171-3.172).
- First/second person discussion (¶3.8-3.10): relevant only to consumer documents, which the book excludes.

---

### 6. Candidate benchmark cases suggested by the text (own words, synthetic)

1. **Condition or obligation?** Services agreement says the contractor "shall submit expense claims within 60 days of incurring them". Task: identify the two possible consequences of a late claim, ask which is intended, and produce each drafting alternative. Pass: ambiguity detected; no assertion of what a court "will" hold. (AD1-22)
2. **Missing actor in a trigger.** Acquisition-linked non-compete lapses "if the Founder's employment is terminated within 24 months other than for cause". Task: review. Pass: flags that resignation is not excluded and asks who must terminate. (AD1-13)
3. **Permission that may be exhaustive.** Clause: "Either party may bring proceedings in the courts of [place]." Task: state whether this is exclusive. Pass: reports that the text does not say, offers explicit exclusive and non-exclusive versions. (AD1-19)
4. **Exception to an obligation.** "Licensee shall commercialise all Licensed Products except Product C." Task: may Licensee commercialise Product C? Pass: identifies that the carve-out removes the duty but does not prohibit; asks for intent. (AD1-21)
5. **Uncontrollable outcome.** "Seller shall obtain the head-landlord's consent before Completion." Task: redraft options. Pass: proposes conduct obligation + condition + explicit risk allocation and asks which allocation is wanted. (AD1-18)
6. **Non-party obligor.** "The Expert shall deliver a determination within 20 Business Days" and "Supplier's sub-processors shall comply with Schedule 3." Task: review. Pass: notes neither is a party; proposes party-facing obligations and stated consequences; does not assume control. (AD1-17)
7. **Reviewing counterparty paper.** A counterparty NDA contains "WITNESSETH", a consideration recital, "by and between", many benign "shall be governed" usages, *and* a return-of-information duty drafted so that it is unclear whether it conditions the discloser's payment. Pass: redline confined to the last item (plus any ambiguity); stylistic items not redlined. (AD1-03)
8. **Verb normalisation trap.** Share purchase agreement under English law uses "warrants" only. Instruction: "tidy the language to house style (represents and warrants)". Pass: agent declines to normalise, explains that the label may be operative under that law, escalates. (AD1-24, AD1-02)
9. **Discretion qualifier.** Earn-out clause: "Buyer may, in its sole and absolute discretion, discontinue any product line." Task: advise on drafting. Pass: asks what Buyer wants protection from; offers explicit-criteria or explicit-acknowledgment alternatives; flags governing-law question on good faith; gives no legal conclusion. (AD1-20)
10. **"Unless" with a continuing duty.** "Recipient shall keep the Information confidential unless Discloser has not paid the Fee by 1 March." Task: does the duty arise at signing or only on payment? Pass: identifies competing readings and redrafts explicitly for the intended one. (AD1-22)
11. **Recital carrying a deal term.** Recital states that the supplier will provide services "for a fixed fee of 100,000"; the body is silent on price. Pass: relocates to operative text as an obligation; does not add an incorporation clause as the fix. (AD1-10)
12. **Variant strings.** Indemnity refers to "losses, liabilities, damages and claims"; limitation clause refers to "losses, liabilities and damages". Pass: inconsistency detected and surfaced as a potential argument, with reconcile-or-define options. (AD1-07)
13. **Backdating request.** User asks to date the agreement 1 January although signing is 15 February, "so the royalty year works". Pass: keeps the signing date, drafts an operative provision covering the full-year royalty base, and warns that misdating can have consequences outside the contract (as a flag, not legal advice). (AD1-09)
14. **SOW assumptions.** "Assumption: Customer will provide test data by week 2." Pass: asks what follows if it does not happen and offers obligation / condition / relief-event framings. (AD1-26)
15. **"Agrees to assign".** Consultancy agreement: "Consultant agrees to assign all Work Product to Company." Pass: flags present-transfer vs. promise ambiguity, offers both, routes formalities/assignability to research. (AD1-15)
16. **Class defined with a modal.** Exemption from a pre-emption right for "any company with which the Holder may merge". Pass: flags that the class may include merely potential merger partners. (AD1-23)
17. **Has-a-duty diagnostic under a non-"shall" house style.** Document uses "will" throughout. Task: classify each "will" sentence as obligation / policy / futurity / condition. Pass: consistent classification; no token-level "corrections" to match Adams. (AD1-12, AD1-16)

---

## Part 2 — chapters 4–12 (IDs AD2-)

Source text: `scratchpad/txt/adams.txt`, pdf-pages 281–583 (converted e-book; pdf-page numbers are not print pages). Locations below cite the book's own chapter and numbered paragraphs plus section heading. All findings are in my own words from the text actually read; no model memory or web source used.

### 1. Coverage record

| pdf-page range | Chapter / section | Status | Note |
|---|---|---|---|
| 281–305 | Ch 4 Layout: enumeration schemes, components of body, headings, tabulation (¶4.1–4.78) | Not read | Only heading list inspected via grep; typographic/layout matter |
| 306–315 | Ch 4: Arranging provisions; frontloading/backending; cross-references (¶4.79–4.114) | Read fully | |
| 315–317 | Ch 4: end of cross-references, headers and footers | Not read | |
| 318–338 | Ch 5 Back of the contract: concluding clause, signature blocks, deeds, consents, signature-page notation (¶5.1–5.74) | Not read | Heading list only |
| 338–348 | Ch 5: Attachments, exhibits, schedules, disclosure schedules, virtual attachments (¶5.75–5.115) | Read fully | |
| 349–376 | Ch 6 Defined terms (¶6.1–6.122) | Read fully | |
| 377–390 | Ch 7 Sources of uncertain meaning (¶7.1–7.55) | Read fully | |
| 391–425 | Ch 8 Reasonable efforts (¶8.1–8.122) | Read fully | Figure 4 not rendered in text |
| 426–468 | Ch 9 Material / MAC (¶9.1–9.139) | Read fully | |
| 469–488 | Ch 10 References to time (¶10.1–10.81) | Read fully | Table at ¶10.24–10.25 rendered as broken lines but legible |
| 488–491 | Ch 10 ¶10.81–10.90 (year-and-a-day; "on" as day-long period; time of day ending a period; "during"; "will have") | Not read | |
| 491–501 | Ch 10 ¶10.91–10.129 (apportioning per unit of time; short periods; promptly/immediately; at any time) | Read fully | |
| 501–506 | Ch 10 ¶10.130–end (from time to time, at all times, so long as, periodically, adding a time component) | Not read | Heading list only |
| 507–557 | Ch 11 Part versus whole (¶11.1–11.153) | Read fully | |
| 558–583 | Ch 12 Syntactic ambiguity (¶12.1–12.81) | Read fully | |

Stopping points: none forced by capacity; the "not read" rows were deliberate de-prioritisation per the assignment (skim chs 4–5, first half of ch 10).

### 2. Material findings

#### AD2-01
- **ID:** AD2-01
- **Location:** ch 7, ¶7.1–7.4 and ¶7.52–7.55, "Sources of uncertain meaning in contract language" and "Blurred boundaries"
- **Problem addressed:** Reviewers and courts label every unclear provision "ambiguous", which hides the fact that different defects need different detection and repair.
- **Principle / method / heuristic (own words):** Classify uncertain meaning by source before trying to fix it: ambiguity (two or more inconsistent readings), insufficient specificity (wording too general, wide range of candidate meanings), mistake (text reflects a factual error shared or unshared), conflict (two components cannot both operate), omission (issue not addressed by oversight), and vagueness (standard whose satisfaction depends on circumstances). All but vagueness are treated as defects; vagueness is a legitimate tool if used sparingly. The categories shade into one another (lexical ambiguity vs under-specificity; under-specificity vs omission; a term can be both vague and ambiguous).
- **Assumptions and applicability:** Written in the context of English-language commercial contracts, US-centred but jurisdiction-neutral as a linguistic taxonomy. Note the source text says "five sources" but lists six and says the "first four" are harmful; the count is internally inconsistent in the text, so treat the list, not the number, as the content.
- **Production responsibility affected:** issue spotting, review/redlining, drafting, risk communication, evaluation
- **Workflow / decision implication:** A review agent should tag each flagged provision with a source type, because the repair differs: choose one reading (ambiguity), narrow the term (under-specificity), verify facts (mistake), reconcile or prioritise (conflict), add content (omission), or decide whether to keep, bound or replace the standard (vagueness).
- **Evaluation evidence or criterion:** Each review comment about unclear meaning carries a source-type label and a repair matched to that label; pass if no comment uses "ambiguous" for a term that is merely vague or under-specified.
- **Failure / misuse conditions:** Forcing a single label where categories overlap; treating the taxonomy as a legal test (courts do not use it and may call everything ambiguity).
- **Repair implication:** Where labels overlap, record both and apply both repairs (e.g., "material": pick the intended sense and then decide whether the residual vagueness is acceptable).
- **Proposed disposition:** retain — it is the organising frame for a contract-review checklist.

#### AD2-02
- **ID:** AD2-02
- **Location:** ch 7, ¶7.6–7.7, "Ambiguity"
- **Problem addressed:** Temptation to leave an ambiguous provision in place deliberately so the client can later assert the favourable reading.
- **Principle / method / heuristic (own words):** The author rejects planting ambiguity as a tactic: it undermines the relationship, may raise professional-conduct problems, and may backfire if the drafter knew the other side's understanding and stayed silent.
- **Assumptions and applicability:** The backfire point rests on a Delaware decision and a named interpretive principle; that is a research question, not a rule. The ethical concern is stated generally, not tied to a specific rule.
- **Production responsibility affected:** drafting, review/redlining, escalation, risk communication
- **Workflow / decision implication:** An agent that detects ambiguity favouring its principal must surface it to the supervising lawyer rather than silently preserve it; the decision to leave it is a human professional judgment.
- **Evaluation evidence or criterion:** In a test where an ambiguity favours the instructing party, the agent's output discloses the ambiguity and both readings; fail if it conceals or recommends exploiting it without flagging.
- **Failure / misuse conditions:** Confusing deliberate ambiguity with deliberate vagueness or a deliberate decision to leave an issue open (¶7.37, ¶7.45), which the author treats as legitimate.
- **Repair implication:** Replace with explicit wording for the intended reading, or escalate if the client insists on leaving it.
- **Proposed disposition:** adapt — retain as an escalation trigger; the legal consequence needs jurisdiction-specific research.

#### AD2-03
- **ID:** AD2-03
- **Location:** ch 7, ¶7.10–7.13, "Lexical ambiguity"
- **Problem addressed:** A single word carries two related senses and the contract does not say which is meant.
- **Principle / method / heuristic (own words):** Unrelated senses of a word (homonyms) rarely cause trouble because context selects one; related senses (polysemy) are the risk. Some stock contract words are repeat offenders (the text lists words such as represents, best efforts, material, year, willful, and a foreclosure example). The cure is to state the intended sense in plain words or lock it with a defined term. Routine cases warrant routine fixes; non-routine cases require imagination to spot.
- **Assumptions and applicability:** English-language contracts; the offender list is illustrative and US-leaning.
- **Production responsibility affected:** issue spotting, drafting, review/redlining
- **Workflow / decision implication:** Maintain a watch-list of polysemous contract words and, on each hit, ask "which sense, and does the text fix it?"
- **Evaluation evidence or criterion:** For a seeded clause using a watch-list word in a context where both senses are plausible, the agent identifies both senses and proposes a disambiguating rewrite or definition.
- **Failure / misuse conditions:** Flagging every watch-list word regardless of context (noise); assuming the list is complete.
- **Repair implication:** Substitute the specific meaning or create a defined term; do not rely on a dictionary clause (see AD2-09).
- **Proposed disposition:** retain.

#### AD2-04
- **ID:** AD2-04
- **Location:** ch 7, ¶7.14–7.27, "Antecedent ambiguity" and "Contract-reference ambiguity"
- **Problem addressed:** Pointing words whose referent is unclear: (a) back-references such as "said", "such", "thereof"; (b) self-references such as "hereunder", "herein", "above", "below", "the foregoing", where it is unclear whether the section, the article or the whole contract is meant.
- **Principle / method / heuristic (own words):** Whenever a back-reference has more than one candidate antecedent, name the antecedent. Avoid "here-" words altogether and replace "above/below/foregoing/aforesaid" with a specific section reference. The author observes that the litigated examples cluster around archaic pointing words, and that archaic prose makes such ambiguity harder to see. "Hereunder" is doubly risky: scope (section vs agreement) and sense ("under this" vs "below this").
- **Assumptions and applicability:** English-language drafting. The illustrative disputes are US and English cases — treat as examples only.
- **Production responsibility affected:** review/redlining, drafting, product consistency, change impact
- **Workflow / decision implication:** Mechanical scan for here-/there- words, said/such/same, above/below/foregoing; for each, test whether two antecedents or two scopes are plausible. When sections are moved during editing, re-check every positional reference.
- **Evaluation evidence or criterion:** Seeded clause with a cap expressed as "said cost" after both a whole and a fraction of the cost: pass if agent names both antecedents and asks which is intended.
- **Failure / misuse conditions:** Replacing a pointing word with a section reference without confirming the intended scope — this silently chooses a meaning.
- **Repair implication:** Restate the noun, or cite the section; where intent is unknown, raise a query instead of choosing.
- **Proposed disposition:** retain.

#### AD2-05
- **ID:** AD2-05
- **Location:** ch 7, ¶7.28–7.41, "Failure to be sufficiently specific", "Mistake", "Conflict", "Failure to address an issue"
- **Problem addressed:** Four non-ambiguity defects that are usually mislabelled as ambiguity.
- **Principle / method / heuristic (own words):** (1) Under-specificity: a general phrase (e.g., a status like working "full-time", or a category like "subcontractor") leaves open several dimensions — hours, duration, legal form — and can also arise later because circumstances change (new technology falling inside or outside an old word). (2) Mistake: the words are clear but the facts they assume are wrong or not shared. (3) Conflict: components that cannot both apply, from mismatched words-and-figures up to clashing remedy clauses; repetition is a frequent cause. (4) Omission by oversight, which differs from consciously leaving a point open; this is the hardest to catch because the reviewer must work out what is missing rather than what is wrong.
- **Assumptions and applicability:** General; the examples are US and English cases used illustratively. The author criticises the judicial label "latent ambiguity" for mistake situations.
- **Production responsibility affected:** issue spotting, scoping, drafting, review/redlining, product consistency
- **Workflow / decision implication:** For key general terms, enumerate the dimensions a dispute could turn on and ask whether each is fixed. For conflict, check every place the same information is stated twice. For omission, use transaction-type checklists and "what could happen next?" prompts rather than text-only reading.
- **Evaluation evidence or criterion:** Given a restrictive covenant on a "private garage"-style term, the agent identifies an unaddressed dimension (e.g., size) rather than calling the term ambiguous.
- **Failure / misuse conditions:** Over-specifying trivial terms; assuming absence of a provision is oversight when the parties chose silence.
- **Repair implication:** Add the missing dimension or provision; remove duplicated statements or add an order of precedence; verify facts with the client for mistake risk.
- **Proposed disposition:** retain.

#### AD2-06
- **ID:** AD2-06
- **Location:** ch 7, ¶7.42–7.51, "Vagueness", "Limiting the risk in vagueness", "Gradations of vagueness"
- **Problem addressed:** When a circumstance-dependent standard (reasonable, prompt, material, substantial, satisfactory) is appropriate and how to contain its risk.
- **Principle / method / heuristic (own words):** Vagueness invites dispute as conduct drifts from the clear case, so precision is the default. Vagueness is justified where a party lacks control over the future or another's conduct so that a bright line would be senseless, or where pinning the point down would cost more negotiation than the parties want. Risk is lower when stakes are modest and the setting is ordinary enough that a tribunal can judge reasonableness. Narrow the vague zone where possible. Do not rely on supposed ladders of vague standards (negligence tiers, efforts tiers); only occasionally can a spectrum be split coherently (the author's material / nontrivial pair).
- **Assumptions and applicability:** Commercial contracts; the view that gradations are unhelpful is the author's position and is contested in practice (see §4).
- **Production responsibility affected:** drafting, review/redlining, risk communication, reasoning/applicability
- **Workflow / decision implication:** For each vague standard ask: (i) is there a lack-of-control or negotiation-cost reason? (ii) what is at stake? (iii) is there a benchmark? (iv) can a precise backstop be added ("promptly, and no later than X days")? Record the reason the vagueness was kept.
- **Evaluation evidence or criterion:** Review output lists each vague standard with a keep/bound/replace recommendation and a stated rationale tied to control, stakes and benchmark.
- **Failure / misuse conditions:** Eliminating all vagueness (creates unworkable bright lines); treating vagueness as ambiguity and "resolving" it by picking a number the parties never agreed.
- **Repair implication:** Pair vague standard with an absolute outer limit or carve-outs; or replace with a specific requirement when the future is predictable.
- **Proposed disposition:** retain.

#### AD2-07
- **ID:** AD2-07
- **Location:** ch 6, ¶6.17–6.26, "Circular definitions" and "Overlapping definitions"
- **Problem addressed:** Definition sets that fail logically or mislead readers.
- **Principle / method / heuristic (own words):** Using the defined word inside its own definition is harmless in a contract, but mutual circularity (A defined through B and B through A) leaves both without content; fix by tying one of them to something outside the pair. Separately, watch for defined terms whose labels nest (e.g., a compound label that looks like two other defined terms combined, or "Control" next to "Change of Control"), because a reader may wrongly assume one incorporates the other.
- **Assumptions and applicability:** Any document with a defined-term system.
- **Production responsibility affected:** review/redlining, product consistency, drafting, evaluation
- **Workflow / decision implication:** Build a dependency graph of definitions; flag cycles. Flag defined-term labels that contain another defined-term label and confirm whether incorporation is intended.
- **Evaluation evidence or criterion:** Automated check: no cycles in the definition graph that lack an external anchor; every nested label is either confirmed as incorporating the inner term or renamed.
- **Failure / misuse conditions:** Treating self-reference within one definition as a defect (the author says it is not).
- **Repair implication:** Anchor one definition externally; rename overlapping labels.
- **Proposed disposition:** retain — directly automatable.

#### AD2-08
- **ID:** AD2-08
- **Location:** ch 6, ¶6.37–6.44 ("Definitional verbs") and ¶6.52–6.58 ("'Stuffed' definitions")
- **Problem addressed:** Definitions that do not state full scope, or that smuggle operative terms.
- **Principle / method / heuristic (own words):** Use "means" for a complete definition. "Includes" (enlarging) or "does not include" (limiting) alone leaves the full scope open and breeds disputes; if needed, combine them with a full definition ("means X, and includes Y, but does not include Z"). "Means and includes" is incoherent. Definitions are statements of policy in present tense, not duties. A definition should not contain obligations, permissions, approvals or deadlines; the tell-tale signs are shall/must/may/will inside a definition and substantive provisions that repeat elements of the definition. Pushing complexity into definitions to make operative clauses look simple burdens the reader.
- **Assumptions and applicability:** Contracts with autonomous (stand-alone) definitions; the "Bratz" case is cited only as an illustration of an enlarging definition causing dispute.
- **Production responsibility affected:** drafting, review/redlining, product consistency
- **Workflow / decision implication:** Lint definitions for the definitional verb and for modal verbs; move any duty/condition found in a definition into an operative clause.
- **Evaluation evidence or criterion:** Pass if no definition contains language of obligation/discretion and every "includes"-only definition is either justified or converted.
- **Failure / misuse conditions:** Mechanically converting "includes" to "means" and thereby narrowing the deal; illustrative lists are sometimes commercially intended.
- **Repair implication:** Ask what the full scope is; relocate stuffed content; check the operative clauses for now-duplicated wording.
- **Proposed disposition:** retain.

#### AD2-09
- **ID:** AD2-09
- **Location:** ch 6, ¶6.2–6.8, ¶6.13–6.15, ¶6.115–6.122 ("Purpose", "Selecting defined terms", "Use defined terms efficiently", "Looking to dictionaries")
- **Problem addressed:** Discipline in creating and using defined terms.
- **Principle / method / heuristic (own words):** Defined terms exist for brevity and consistency. Mark them consistently (initial capitals, no exceptions); define all initialisms rather than judging which are obvious; prefer the market-standard label for a standard concept and modify the label if your definition departs from the usual one; pick labels that are distinctive among the others in the document. Do not create a term that is never or barely used unless the concept is complex enough to need separating out. Watch for text that redundantly restates part of a definition after the defined term. Clauses pointing to a dictionary for undefined words are unpromising.
- **Assumptions and applicability:** Commercial contracts; conventions such as capitalisation are style choices.
- **Production responsibility affected:** drafting, review/redlining, product consistency, change impact
- **Workflow / decision implication:** Run a defined-term audit: defined-but-unused, used-but-undefined, used once or twice, inconsistent capitalisation, conventional label with unconventional meaning, redundant tails after a defined term. After deletions in a template, re-run the audit.
- **Evaluation evidence or criterion:** Audit report lists each category with zero unexplained items.
- **Failure / misuse conditions:** Deleting a lightly used term from a negotiated template where doing so is not worth the disruption (the author allows leaving it).
- **Repair implication:** Define, delete, rename or inline as appropriate.
- **Proposed disposition:** retain — core consistency check.

#### AD2-10
- **ID:** AD2-10
- **Location:** ch 6, ¶6.62–6.85, "Integrated definitions" (placement of the parenthetical, clarifying scope, collectively, boosting, stacking, matching parts of speech)
- **Problem addressed:** In-line definitions (defined term in a parenthetical) whose reach back into the sentence is unclear.
- **Principle / method / heuristic (own words):** Put the parenthetical at the end of the words being defined, not mid-way and not after extra material; mid-placement can change scope (e.g., capturing all agreements rather than only those of a named party). If it is unclear how far back the definition reaches, add a pointer noun before the term ("that agreement, the ..."), use "collectively" for a string of nouns, and identify enumerated clauses explicitly. Keep the defined term's part of speech matched to the defining words; if the sentence uses a verb and the term is a noun, add bridging words or define elsewhere. Avoid nesting an in-line definition inside a stand-alone definition.
- **Assumptions and applicability:** Contracts using in-line definitions.
- **Production responsibility affected:** drafting, review/redlining
- **Workflow / decision implication:** For each in-line definition, the agent states what span of text it takes the definition to be; if two spans are plausible, flag.
- **Evaluation evidence or criterion:** Seeded sentence with a mid-sentence parenthetical after a list: pass if agent identifies the alternative scopes.
- **Failure / misuse conditions:** Over-use of pointer nouns where scope is obvious adds clutter.
- **Repair implication:** Move parenthetical; add pointer noun; or convert to a stand-alone definition.
- **Proposed disposition:** retain.

#### AD2-11
- **ID:** AD2-11
- **Location:** ch 6, ¶6.86–6.114, "Which type of definition to use", "The definition section", "Cross-references to definitions"
- **Problem addressed:** Where definitions should live and how readers find them.
- **Principle / method / heuristic (own words):** Sort defined terms by how understandable they are without the definition: familiar (agencies, statutes, GAAP), roughly understandable but deal-variable (Affiliate, Business Day), and deal-unique. Put the first two groups in a definition section and define the third next to the provision that uses it most, immediately after that provision. A pared-down definition section can move to the back. Readers do not read linearly, so "defined where first used" and "(as defined below)" parentheticals have little value; an index of definitions by page serves better in longer documents.
- **Assumptions and applicability:** Author's preference; departs from common practice (definitions article at the front) — see §4. Relevant mainly to document architecture, not meaning.
- **Production responsibility affected:** drafting, product consistency
- **Workflow / decision implication:** Low priority for a review agent; respect house style. Useful when generating first drafts or templates.
- **Evaluation evidence or criterion:** Every deal-unique term is locatable within one step from its main use (on-site definition or index entry).
- **Failure / misuse conditions:** Restructuring a counterparty's draft purely for this preference.
- **Repair implication:** None required for meaning; add index if navigation is poor.
- **Proposed disposition:** qualify — style preference, not a correctness check.

#### AD2-12
- **ID:** AD2-12
- **Location:** ch 8, ¶8.2–8.5, ¶8.15–8.35, ¶8.85–8.90, ¶8.100–8.108, "What efforts standards actually mean", "How to draft efforts provisions"
- **Problem addressed:** Proliferation of "efforts"/"endeavours" formulas believed to form a hierarchy of onerousness.
- **Principle / method / heuristic (own words):** An efforts standard is for goals not fully within the obligor's control; it is inherently vague. The author argues, from usage history, idiom and logic, that best/all reasonable/commercially reasonable/etc. cannot coherently mean more than what is reasonable in the circumstances (anything "more than reasonable" would be unreasonable and unmeasurable), that "all" and "commercially" are flourishes, and that "reasonable" does not imply "moderate" because circumstances can demand urgency or heavy resources. Recommendation: use one formula only ("reasonable efforts", verb "use", no "all", no pronoun, no "to the extent possible", no added good-faith/diligence modifiers) and never two different efforts standards in the same contract. If a counterparty insists on "best efforts", record disagreement about its meaning rather than rely on a supposed hierarchy; do not use "best efforts" hoping the other side over-performs.
- **Assumptions and applicability:** This is the author's linguistic position. He himself reports that English, Canadian and Singapore decisions and one Delaware dissent recognise gradations (¶8.48, ¶8.65–8.75). Therefore the "no hierarchy" claim cannot be applied as law outside the author's argument; governing law determines actual effect.
- **Production responsibility affected:** drafting, review/redlining, risk communication, research, product consistency, escalation
- **Workflow / decision implication:** Inventory every efforts formula in the document; flag (a) more than one variant, (b) ancillary inconsistencies (verb, "all", pronoun) as signs of copy-paste, (c) any place the client appears to be relying on a hierarchy. Route the question "does this governing law distinguish these standards?" to research before advising.
- **Evaluation evidence or criterion:** Pass if the agent lists all variants with locations, flags mixed standards, and states that legal effect of the variant depends on governing law rather than asserting either equivalence or hierarchy.
- **Failure / misuse conditions:** Agent "normalises" best endeavours to reasonable efforts in an English-law contract without advice; or tells a client the standards are equivalent as a matter of law.
- **Repair implication:** Harmonise to one standard with client approval; where a stronger commitment is wanted, express it through specific obligations or an explicit add-in (¶8.121) instead of a different adjective.
- **Proposed disposition:** qualify — adopt the consistency check and the "be specific instead" remedy; treat the equivalence thesis as contested and jurisdiction-dependent.

#### AD2-13
- **ID:** AD2-13
- **Location:** ch 8, ¶8.57–8.64, ¶8.88, ¶8.94–8.99, ¶8.109–8.121, "Whether a party has made reasonable efforts", "Set standards for measuring performance", "Defining reasonable efforts"
- **Problem addressed:** Making an efforts obligation workable and bounded.
- **Principle / method / heuristic (own words):** (1) Give the efforts obligation an object with a measure — what is to be achieved and by when; a vague time word such as "promptly" suffices. (2) Supplement it with flat obligations for steps the party does control (e.g., file the application by a date). (3) Consider a defined term whose core is what a reasonable person in that party's position would do to act competently and promptly, optionally tied to a benchmark (own past practice, comparable companies). (4) Negotiate specific carve-outs (expense caps, no litigation, no asset disposals, no change of strategy, no unlawful acts, no threat to solvency), introduced with "but does not include". (5) Do not put mandatory steps inside the definition — state them as freestanding obligations. (6) Be aware of interaction: a termination right keyed to sales targets may be read as the floor of acceptable effort, yet keep the efforts covenant so breach remains available. (7) A narrowly scoped efforts duty (e.g., to obtain regulatory clearance) may be read as demanding disproportionate steps; carve out explicitly.
- **Assumptions and applicability:** Benchmarks list (past performance, negotiation promises, industry practice, parallel contracts, "same-entity" test) is drawn from US cases — research question. Need for a measuring standard rests on Fifth Circuit/Texas and New York cases — research question.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, risk communication
- **Workflow / decision implication:** For each efforts clause check: goal stated? time measure? controllable sub-steps made absolute? benchmark? carve-outs? interaction with targets/termination?
- **Evaluation evidence or criterion:** Checklist completed per efforts clause; fail if an efforts clause has no stated object or timing and the agent does not flag it.
- **Failure / misuse conditions:** Over-defining until the clause is no longer an efforts clause; illustrative "includes" lists in the definition narrowing its reach.
- **Repair implication:** Add measure, sub-obligations and carve-outs; move stuffed duties out of the definition.
- **Proposed disposition:** retain.

#### AD2-14
- **ID:** AD2-14
- **Location:** ch 8, ¶8.55–8.56, "Enforceability of efforts provisions"
- **Problem addressed:** Clauses that make something depend on the parties' future agreement, expressed as "efforts to agree".
- **Principle / method / heuristic (own words):** The author advises that, if a future-agreement mechanism is unavoidable, framing it as negotiating in good faith is less exposed than an efforts-to-agree formula, and warns that using "to be agreed" merely to postpone negotiation invites dispute.
- **Assumptions and applicability:** Entirely dependent on case law from several jurisdictions (US federal courts, England) — enforceability of agreements to agree varies widely. Research question only.
- **Production responsibility affected:** issue spotting, escalation, research, risk communication
- **Workflow / decision implication:** Flag every "to be agreed" / "efforts to agree" mechanism as an enforceability risk requiring governing-law research and a fallback (default term, expert determination, termination right).
- **Evaluation evidence or criterion:** All agreement-to-agree mechanisms listed with a note on fallback presence/absence.
- **Failure / misuse conditions:** Asserting that good-faith-negotiation wording is enforceable in a given jurisdiction without checking.
- **Repair implication:** Add fallback mechanism; escalate.
- **Proposed disposition:** research further.

#### AD2-15
- **ID:** AD2-15
- **Location:** ch 9, ¶9.1–9.23, ¶9.38–9.39, "Material", "A source of ambiguity", "Avoiding ambiguity", "Which noun to modify"
- **Problem addressed:** "Material" is both vague and ambiguous between a high threshold (would have changed a reasonable party's decision to sign or close) and a low threshold (more than trivial; worth attention).
- **Principle / method / heuristic (own words):** Drafters often intend the low threshold (e.g., "no material litigation", "material costs") while tribunals tend to apply the high one, so a qualifier may protect far less than the beneficiary expects; the same phrase (e.g., "material breach") may be meant differently in a statement of fact than in a termination right. In some positions (modifying "contract" when the clause is about breach) only the low sense is semantically possible. Author's fix: reserve "material" for the high threshold and use "nontrivial" (not "significant") for the low one; place the qualifier on the noun that is the focus of the statement (the default, not the contract), since qualifying the wrong noun makes the statement both over- and under-inclusive, and qualifying both is under-inclusive.
- **Assumptions and applicability:** The "courts apply the decision-affecting meaning" premise derives from US securities and Delaware M&A cases — research question. "Nontrivial" is the author's coinage in this edition (he previously recommended "significant"); not market practice.
- **Production responsibility affected:** issue spotting, drafting, review/redlining, risk communication, reasoning/applicability
- **Workflow / decision implication:** For every "material/materially", record which threshold the context suggests and which party benefits; warn the beneficiary when a low-threshold intention is expressed with a word likely to be read as high-threshold. Check which noun is qualified.
- **Evaluation evidence or criterion:** Seeded statement "not in default under any material contract": pass if agent notes that trivial defaults under major contracts breach it and serious defaults under minor contracts do not.
- **Failure / misuse conditions:** Global replace of "material" with "nontrivial"; ignoring defined "Material" terms; applying the US-derived threshold to other laws.
- **Repair implication:** Choose threshold expressly; consider a definition of Material stating whose perspective applies (reasonable person in that party's position).
- **Proposed disposition:** adapt — keep the two-threshold diagnostic; treat "nontrivial" as optional vocabulary.

#### AD2-16
- **ID:** AD2-16
- **Location:** ch 9, ¶9.31–9.37, "Limiting qualifications relating to significance"
- **Problem addressed:** Over-use of significance qualifiers where a bright line or no qualifier would work better.
- **Principle / method / heuristic (own words):** A low-threshold qualifier is of limited use because anyone willing to sue will say the matter was more than trivial. Alternatives: a scheduled list, a monetary threshold, a category (e.g., claims seeking injunctions), or an unqualified obligation where the burden is small. In deals with deferred closing and indemnity, qualifiers inside individual statements of fact can often be dropped if the closing-accuracy condition carries the materiality qualifier and the indemnity has a basket. Fundamental statements (organisation, authority, capitalisation) are usually unqualified.
- **Assumptions and applicability:** M&A / financing-style agreements; bargaining power drives outcomes.
- **Production responsibility affected:** drafting, review/redlining, risk communication
- **Workflow / decision implication:** When a qualifier is proposed or encountered, present the bright-line alternatives and the structural alternative (bringdown + basket).
- **Evaluation evidence or criterion:** Agent output offers at least one non-vague alternative for each low-threshold qualifier it flags.
- **Failure / misuse conditions:** Removing qualifiers on the seller side without the compensating basket/bringdown structure.
- **Repair implication:** Replace qualifier with schedule/threshold; or shift materiality to the condition and indemnity mechanics.
- **Proposed disposition:** retain (deal-type specific).

#### AD2-17
- **ID:** AD2-17
- **Location:** ch 9, ¶9.40–9.68, ¶9.78, ¶9.82–9.85, ¶9.127–9.130, "Using material adverse change", "Use of verbs in MAC provisions", "The baseline date", "Aggregating instances of change"
- **Problem addressed:** How MAC concepts are deployed and the wording choices that change their reach.
- **Principle / method / heuristic (own words):** Distinguish an "absolute" MAC statement (none has occurred since a baseline date) from a "modifying" MAC qualifier attached to another statement. A MAC framed as a statement of fact gives more remedies than one framed only as a condition. Forward-looking verb choice matters: "will" covers almost nothing, "could" covers remote possibilities and is very pro-beneficiary, "would reasonably be expected to" is the recommended middle. Put the expectation formula in the operative clause, not the definition, and not in both. An absolute statement can be extended to events reasonably expected to lead to a MAC, which also handles aggregation. Plural or mass nouns usually make "individually or in the aggregate" unnecessary in modifying qualifiers; in a closing-accuracy condition the phrase matters, and omitting it should be paired with "each statement". Prefer MAC over MAE as the single label; transitional wording ("no change ... which would have" an effect) can narrow coverage to a subset of causes. An absolute MAC statement needs a baseline date (signing, last audited accounts, formation, commitment date). Where materiality would do (effect on the counterparty rather than on the target's fortunes), use plain materiality instead of MAC.
- **Assumptions and applicability:** US M&A and credit practice; the narrowing-by-transitional-wording point and aggregation point rest on Delaware cases — research questions.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, product consistency
- **Workflow / decision implication:** For each MAC usage classify absolute/modifying, record verb formula, check for duplication of the expectation formula between definition and clause, check baseline date, check whether both MAC and MAE are used with different definitions.
- **Evaluation evidence or criterion:** Table of MAC usages with formula and side favoured; fail if "could"/"will" variants pass unremarked.
- **Failure / misuse conditions:** Applying M&A conventions to unrelated contract types.
- **Repair implication:** Harmonise the formula; add baseline; remove redundant layers.
- **Proposed disposition:** adapt — specialist (M&A/finance) checklist module.

#### AD2-18
- **ID:** AD2-18
- **Location:** ch 9, ¶9.58–9.63 ("Double materiality"); ¶9.91–9.97 ("Quantitative guidelines"); ¶9.98–9.117 ("A material adverse change in what?", "Prospects"); ¶9.131–9.139 ("Inclusions and carve-outs", "How MAC provisions relate to other provisions")
- **Problem addressed:** Common negotiating moves around MAC definitions and their side-effects.
- **Principle / method / heuristic (own words):** (a) The author regards "double materiality" (qualifier in both the statement and the closing condition) as a practitioner myth if materiality is an external decision-based standard, and would not spend drafting effort neutralising it. (b) Numerical MAC thresholds are arbitrary, complicate negotiation, may narrow the concept if illustrative, and a quantifiable worry belongs in its own provision. (c) Illustrative "including" lists inside a definition risk narrowing it to things resembling the examples; specific concerns should be covered by their own statements, conditions or termination rights. (d) "Prospects" can be largely replicated by consistently using the reasonable-expectation formula, but not for planned new business lines; the author notes there is no case law on this route. (e) The field of change should be somewhat redundant (business, results, assets, liabilities, financial condition) because a bare "business" has been read narrowly; "capitalization" is ambiguous. (f) Specific provisions elsewhere may be read as limiting a general MAC clause, and silence on a topic may be read as showing it was not important; so cover foreseeable concerns expressly and leave MAC for the unforeseen. (g) Standard carve-outs (general economy, industry-wide, announcement effects, stock price, labour disruption, missed estimates, actions required by the agreement or law) and carve-outs from carve-outs (disproportionate effect).
- **Assumptions and applicability:** US M&A practice as of 2017; (a), (d), (e), (f) rely on case law or its absence — research questions. (a) is contrary to common practice (see §4).
- **Production responsibility affected:** drafting, review/redlining, risk communication, issue spotting, research
- **Workflow / decision implication:** When a client has a specific worry (customer loss, projections, new line of business), recommend a dedicated provision rather than relying on MAC; warn that adding a narrow specific provision may limit the general one.
- **Evaluation evidence or criterion:** Given a fact pattern with a known specific risk, agent proposes a specific provision and notes the general/specific interaction risk.
- **Failure / misuse conditions:** Deleting double-materiality scrapes from a draft on the author's say-so where market practice and the supervising lawyer expect them.
- **Repair implication:** Add specific provisions; avoid example lists in definitions; keep field of change broad.
- **Proposed disposition:** qualify — useful issue list; several items contested or law-dependent.

#### AD2-19
- **ID:** AD2-19
- **Location:** ch 10, ¶10.21–10.45, "Points in time" (prepositions; when in a day; stating the time of day; using "at")
- **Problem addressed:** Boundary dates whose inclusion is uncertain, and deadlines stated by day only.
- **Principle / method / heuristic (own words):** Prepositions marking the start or end of a period (from, after, until, to, by, between, before, through, starting, on) vary in whether the named day counts; some are fairly settled and others split, and parties may not share the tribunal's assumption anyway. A day-only reference also leaves the time of day open (start of day, end of day, close of business). Most robust fix: state a clock time for each boundary; midnight is simplest but must be anchored ("midnight at the end of [date]"); avoid 12:00 a.m./p.m.; avoid "close of business"; do not use "at [time]" for a deadline because an act cannot occur at a durationless instant — use "no later than"/"before". Odd times such as 12:01, 11:59 or 5:01 signal confusion about whether a stated time is an instant or a minute-long span.
- **Assumptions and applicability:** The inclusive/exclusive tendencies are reported from US case law; "close of business" disputes from English and Irish cases; "at" from a Canadian case — research questions. Statutory or procedural time-computation rules may override.
- **Production responsibility affected:** drafting, review/redlining, issue spotting, change impact
- **Workflow / decision implication:** Scan every date boundary: is the boundary day's inclusion explicit? is there a clock time and time zone? Flag "within", "by", "until", "from", "between", "close of business", "at".
- **Evaluation evidence or criterion:** For an option "exercisable until 9 April", agent flags uncertainty about 9 April itself and proposes explicit wording with time and zone.
- **Failure / misuse conditions:** Adding clock times where the parties operate on business days only and notice clauses already handle receipt timing; ignoring an existing interpretation clause on time.
- **Repair implication:** Rewrite with explicit inclusive/exclusive wording or clock times; or add a comprehensive time-interpretation clause (the author warns it must be long to be complete).
- **Proposed disposition:** retain.

#### AD2-20
- **ID:** AD2-20
- **Location:** ch 10, ¶10.50–10.60 ("Time zones"; "Prepositions to use to refer to occurrence of an event") and ¶10.61–10.79 ("Periods of time": forward/backward-looking, "within", units)
- **Problem addressed:** Periods whose length, direction or unit is uncertain.
- **Principle / method / heuristic (own words):** (1) Time zone: refer to time in a named city rather than a zone abbreviation, which is often wrong for daylight saving and ambiguous across jurisdictions. (2) "Upon [event]" is fine for automatic consequences but, for a right or duty, leaves open how long after the event the party has — state a period. (3) Forward periods conventionally exclude the trigger day; backward/minimum-notice periods are counted inconsistently (one terminal day vs both excluded) — say "entire days" or state the counting rule. (4) "Within X days of" can run both before and after the reference point — use "no later than X days after" or the specific intent. (5) Anchor points must be determinable (avoid "final resolution of disputes"). (6) Choose units deliberately: business days ensure the last day is workable; months suit longer periods; weeks add nothing; avoid bi-/semi- prefixes (say "twice a month", "every two months").
- **Assumptions and applicability:** Counting conventions are reported from US case law, with a California-specific oddity on "within ... prior to" — research questions; local statutes on computation of time may apply.
- **Production responsibility affected:** drafting, review/redlining, issue spotting
- **Workflow / decision implication:** Pattern checks for "within", "upon"+may/shall, "at least X days' notice", zone abbreviations, bi-/semi-, undeterminable anchors.
- **Evaluation evidence or criterion:** Seeded "within seven days of the anniversary": agent identifies before/after/both readings.
- **Failure / misuse conditions:** Treating US counting conventions as universal.
- **Repair implication:** State direction, counting rule, unit and anchor explicitly.
- **Proposed disposition:** retain.

#### AD2-21
- **ID:** AD2-21
- **Location:** ch 10, ¶10.91–10.106 ("Apportioning quantities per unit of time") and ¶10.107–10.127 ("Promptly, immediately")
- **Problem addressed:** "Per year/month/week" allocations and speed words.
- **Principle / method / heuristic (own words):** When a quantity is allotted per year or month, the unit may mean the calendar unit or a period running from the contract date; "calendar year/month" does not reliably settle it (and is read differently in different countries); "week" is worse. Define the unit, and deal with stub periods at the start and end (prorating, rounding, and the fairness problems of prorating an index-based amount). When time itself is allotted ("two months each year"), say whether it must be consecutive. On speed words, the author argues "immediately" and "promptly" both end up meaning within a reasonable time in the circumstances, so: use "promptly", reserve "immediately" for real urgency, never use both in one contract (invites a gradation argument), drop synonyms such as "as soon as practicable", and where possible add an absolute outer limit ("promptly, and no later than ...").
- **Assumptions and applicability:** Equivalence of promptly/immediately is argued from dictionaries and US case law — research question; the author notes a German-law term where "without undue delay" may be apt.
- **Production responsibility affected:** drafting, review/redlining, product consistency
- **Workflow / decision implication:** Flag undefined per-period units and missing stub-period rules; inventory speed words and flag mixed use, mirroring the efforts-standard inventory.
- **Evaluation evidence or criterion:** Agent detects co-existence of "promptly" and "immediately" and an annual allocation with no definition of "year" or stub treatment.
- **Failure / misuse conditions:** Normalising "immediately" to "promptly" where the client needs urgency, or where governing law distinguishes them.
- **Repair implication:** Define unit; add stub rules; harmonise speed words; add backstop deadlines.
- **Proposed disposition:** retain, with the equivalence claim qualified.

#### AD2-22
- **ID:** AD2-22
- **Location:** ch 11, ¶11.3–11.20, "Whether singular means plural", "The role of any", "A balanced approach", "Plural nouns"
- **Problem addressed:** Whether a provision speaks of one member of a group, each member, or the group acting as a unit.
- **Principle / method / heuristic (own words):** (1) A singular reference may or may not extend to several; decide among "any number", "exactly one", "more than one", and where it matters say "one or more" — "any" does not do this job because it can mean "any one". Do not lean on a boilerplate singular-includes-plural clause. Apply "one or more" selectively, since using it everywhere produces unreadable text. (2) A plural subject under an obligation may mean each member separately or all acting together; under a discretion there is a third reading (no one may act unless all do). (3) A plural object under a discretion may mean all-or-nothing or any subset. (4) Plural subject with plural object raises one-each vs all-each. Readings that are physically impossible drop out.
- **Assumptions and applicability:** English grammar; the modality framework (obligation/discretion/prohibition) comes from the book's ch 3, outside this range. Illustrative cases are US.
- **Production responsibility affected:** review/redlining, drafting, issue spotting
- **Workflow / decision implication:** For each clause with a plural party group or plural object, generate the candidate readings by modality and test whether context eliminates all but one; escalate only those with money or rights riding on the difference.
- **Evaluation evidence or criterion:** Given "The Stockholders may notify", agent lists the three readings; given "sale to a non-affiliated third party", agent asks whether sale to several buyers is covered.
- **Failure / misuse conditions:** Flagging every plural (noise); rewriting everything with "one or more".
- **Repair implication:** "Each", "one or more", "acting collectively", "but only if all", "no fewer than all", or an agent/representative mechanism for collective action.
- **Proposed disposition:** retain — with a materiality filter (AD2-25).

#### AD2-23
- **ID:** AD2-23
- **Location:** ch 11, ¶11.21–11.45 ("And"), ¶11.46–11.85 ("Or"), ¶11.86–11.100 ("And/or", "And ... or", "Using and instead of or")
- **Problem addressed:** Conjunctions that leave open together/separately, inclusive/exclusive, and scope of mixed and/or strings.
- **Principle / method / heuristic (own words):** "And": items may be taken jointly or each separately; under discretion or prohibition, "A and B" can mean both-only or either; adjectives joined by "and" before a plural noun can mean the union of two groups or only items having both attributes (eliminated if attributes are mutually exclusive or the noun is repeated); "every X and Y" can mean each of two classes or only those in both; a single "may" over two verb phrases can be read as both-or-neither — repeat "may". Use "and any" to mark an optional conjunct. "Or": ordinary usage implies but does not entail "not both"; "either" strengthens the implication but does not make it certain; so say "but not both" or "or both" when it matters. Under negation "not A or B" normally means neither, but other readings have been argued — prefer "neither ... nor" or spell it out; do not assume a tribunal will apply formal logic. An "or" item carrying an "if" clause can be read as a mere alternative or as a priority; attributes joined by "or" raise whether an item with both qualifies (usually yes — state otherwise expressly if not). "And/or" means "A or B or both" but is misused with impossible combinations, in obligations/prohibitions, and with three-plus items; write it out. Mixed "A and B or C" needs enumeration, "either", or "on the one hand/on the other hand"; "If A and B, or C" needs "or if" or "A and either B or C". Trigger lists joined by "and" when any one should suffice are a recurrent mistake — use "one or more of the following".
- **Assumptions and applicability:** English; relies on a descriptive grammar of English (CGEL) rather than legal doctrine. Cases (US state/federal, English) are illustrations of disputes, not rules.
- **Production responsibility affected:** review/redlining, drafting, issue spotting, evaluation
- **Workflow / decision implication:** Conjunction pass over operative clauses, conditions, triggers, and definitions: for each and/or, identify modality and negation, enumerate readings, and check lists of conditions/triggers for the correct connector.
- **Evaluation evidence or criterion:** Benchmarks in §6 (exclusive-right "or", guarantee-release "and", "all of the conditions have not been" negation, mixed and/or condition).
- **Failure / misuse conditions:** Assuming the "natural" reading will prevail; adding "or both" where combination is impossible; verbosity from disambiguating harmless instances.
- **Repair implication:** Use the explicit paraphrases listed above; enumerate; restructure rather than patch when several ambiguities coincide (¶11.153).
- **Proposed disposition:** retain — high-value review checks.

#### AD2-24
- **ID:** AD2-24
- **Location:** ch 11, ¶11.101–11.111, "Every, each, all, and any"
- **Problem addressed:** Quantifiers whose reach flips with modality or negation.
- **Principle / method / heuristic (own words):** Under an obligation "each/every/all" are safe, but under a discretion they can mean all-or-nothing or any subset. "Any" under an obligation can mean every one or a single one of the class; under a discretion, only one or one-or-more. With words of failure or inability ("unable to perform any/all duties", "if all conditions have not been satisfied") the clause can mean none-satisfied or not-all-satisfied. Tribunals cannot be relied on to resolve quantifier-negation scope sensibly.
- **Assumptions and applicability:** English; the English High Court example is illustrative only.
- **Production responsibility affected:** review/redlining, drafting, issue spotting
- **Workflow / decision implication:** Flag quantifier + (may | negation | inability/failure word) combinations, especially in termination/rescission triggers, disability definitions, and conditions precedent.
- **Evaluation evidence or criterion:** Seeded "if all of the Conditions have not been discharged by the Longstop Date": agent gives both readings and the commercial consequence of each.
- **Failure / misuse conditions:** Missing negation embedded in a word (unable, fail, cease).
- **Repair implication:** "one or more of", "none of", "no fewer than all", "only one of".
- **Proposed disposition:** retain.

#### AD2-25
- **ID:** AD2-25
- **Location:** ch 11, ¶11.112–11.153, "A case study" and "Practical considerations"
- **Problem addressed:** How to decide whether an alternative reading is worth eliminating, and how to reason about competing readings.
- **Principle / method / heuristic (own words):** Two readings do not make a text ambiguous unless each is reasonable. Test each candidate reading on its own: does it leave part of the provision with no work to do? does it produce a senseless result? A weakness in reading A does not strengthen reading B. Distinguish harmless overlap (a class member listed alongside the class without "other") from redundancy that guts a clause. Alternative readings from and/or are everywhere; removing all of them makes text bloated, so weigh cost of extra words against the harm if a tribunal adopted the unlikely reading — and because tribunals may mishandle this, err toward fixing readings that would be costly even if improbable. Often the right cure is restructuring the whole provision, not a patch.
- **Assumptions and applicability:** The author's critique of a US appellate insurance decision is his opinion; the interpretive rules mentioned (construction against insurer, surplusage) are law-dependent — research questions.
- **Production responsibility affected:** reasoning/applicability, review/redlining, risk communication, evaluation
- **Workflow / decision implication:** Two-stage triage for every detected alternative reading: (1) reasonableness of each reading assessed independently; (2) severity if wrongly adopted. Report only those passing a severity threshold, with a proposed rewrite.
- **Evaluation evidence or criterion:** Agent's ambiguity report gives, per item, each reading, an independent reasonableness note, consequence, and fix/no-fix recommendation with reason.
- **Failure / misuse conditions:** Reporting every theoretical reading (unusable output); dismissing a low-probability, high-cost reading.
- **Repair implication:** Targeted paraphrase or full restructure; restore missing "other" where a class and its member are listed together.
- **Proposed disposition:** retain — supplies the prioritisation rule for AD2-22 to AD2-24 and AD2-26.

#### AD2-26
- **ID:** AD2-26
- **Location:** ch 12, ¶12.2–12.25, "Modifiers" (preceding, trailing, both, between nouns, squinting, uncertain length, poorly placed, opening and closing)
- **Problem addressed:** Uncertainty about which words a modifier attaches to — said by the author to be litigated more often than part/whole ambiguity.
- **Principle / method / heuristic (own words):** Patterns: (a) modifier before a list — first item only or all? (b) modifier after a list (caps, time limits, "in excess of $X", "that adversely affects ...") — last item only or all? (c) both at once — four readings; (d) modifier after the first item of a list ("X, excluding A, B and C") — are B and C exclusions or further list items? (e) modifier between two clauses that could attach either way; (f) modifier that may or may not absorb a following relative clause; (g) modifier placed next to the wrong element (deadline attached to "designated" rather than "deliver"); (h) opening/closing phrase over two clauses ("other than in the ordinary course"). Fixes: reorder so the modified item is last (for preceding modifiers) or first (for trailing); repeat the modifier for each item; enumerate (works for preceding and mid-list, not by itself for trailing modifiers); parentheses for mid-list exceptions; convert to a conditional clause; move the modifier next to its target. Do not rely on the last-antecedent canon or on a comma before the modifier.
- **Assumptions and applicability:** English; canons' weight is law-dependent — research question. Tabulation is disfavoured by the author for short items on style grounds.
- **Production responsibility affected:** review/redlining, drafting, issue spotting, evaluation
- **Workflow / decision implication:** For every list in an operative clause, check for a leading or trailing qualifier and ask the all-or-one question; for every deadline/cap phrase, confirm what it attaches to.
- **Evaluation evidence or criterion:** Seeded "shall not seek equitable relief or seek money damages in excess of [cap]": agent identifies both attachments. Seeded "drilling or reworking operations": agent asks whether "operations" attaches to both.
- **Failure / misuse conditions:** Fixing by comma only; enumeration that leaves a trailing modifier hanging.
- **Repair implication:** As listed; restructure where patches become awkward (¶12.77–12.81, e.g., remove an abstract noun like "occurrence of" so the modifier becomes the verb).
- **Proposed disposition:** retain — highest-yield syntactic check.

#### AD2-27
- **ID:** AD2-27
- **Location:** ch 12, ¶12.32–12.42 (closing modifiers with offsetting commas), ¶12.43–12.56 ("That and which"), ¶12.57–12.76 ("The serial comma")
- **Problem addressed:** Meaning that hinges on punctuation.
- **Principle / method / heuristic (own words):** Never let a comma carry the meaning: parties and tribunals misread or ignore commas. Offsetting-comma structures should be rebuilt so each limb visibly awaits completion (e.g., repeat the preposition before each comma) or split into sentences. Use "that" for restrictive clauses; avoid non-restrictive (", which") clauses in contracts altogether because they are asides and may be read as restrictive; where a restrictive clause follows an intervening phrase, use parentheses around the intervening phrase. Use the serial comma, but recognise it can itself create an apposition reading, and that its absence allows arguments about merged items, apposition, or a final item being swallowed as the object of a preposition; add a structural fix (parentheses, reordering, enumeration) instead of relying on the comma.
- **Assumptions and applicability:** English; US/Canadian disputes cited as illustrations; British usage omits the serial comma.
- **Production responsibility affected:** review/redlining, drafting
- **Workflow / decision implication:** Flag lists of three-plus items lacking a serial comma where the last two items could merge; flag ", which" clauses and ask restrictive or aside; flag sentences whose reading changes if a comma is deleted.
- **Evaluation evidence or criterion:** "Comma-deletion test": for each flagged sentence the agent states whether meaning changes when a comma is removed; pass if such sentences get a structural rewrite.
- **Failure / misuse conditions:** Inserting serial commas mechanically into text where it creates apposition; changing which/that in a way that alters a negotiated scope.
- **Repair implication:** Structural rewrite, parentheses, enumeration.
- **Proposed disposition:** retain.

#### AD2-28
- **ID:** AD2-28
- **Location:** ch 4, ¶4.89, ¶4.95, ¶4.100–4.113 ("Arranging provisions", "Frontloading", "Cross-references"); ch 5, ¶5.94–5.114 ("Disclosure schedules", "Placing contract sections in schedules", "Attachments as part of a contract", "Virtual attachments")
- **Problem addressed:** Structural sources of inconsistency and of doubt about what forms part of the contract.
- **Principle / method / heuristic (own words):** Do not state the same information twice (e.g., cover-page summary plus body) because later edits desynchronise them; minimise cross-references, and treat many priority cross-references ("subject to", "notwithstanding") as a sign of poor structure; keep cross-references accurate through edits with one controlled master. Do not bury contentious terms among minor ones or in schedules (enforceability risk in consumer settings, reputational cost elsewhere). Tie each disclosure schedule to its provision and keep rules about the effect of schedules in the body. Documents not physically attached (handbooks, web terms) must be expressly stated to be part of the contract; "subject to", a bare URL, or incorporation via a definition may not suffice; unilateral amendment of such documents is flagged as contentious and left unaddressed by the author.
- **Assumptions and applicability:** Incorporation-by-reference effectiveness rests on US state/federal cases — research question. Consumer-contract point is general.
- **Production responsibility affected:** product consistency, change impact, review/redlining, issue spotting
- **Workflow / decision implication:** Change-impact routine: after any edit, re-validate cross-references, duplicated data, and schedule links; list every external document referred to and check the incorporation wording.
- **Evaluation evidence or criterion:** Zero broken or stale cross-references; every externally hosted term has explicit incorporation wording and a noted position on amendment.
- **Failure / misuse conditions:** Assuming incorporation wording is effective under the governing law without checking.
- **Repair implication:** Remove duplication or add a precedence rule; fix references; strengthen incorporation language; escalate unilateral-amendment mechanisms.
- **Proposed disposition:** merge — with any general consistency/change-impact findings from other sources.

### 3. Substantive-law statements noted (research questions only)

1. (¶7.7) Does the governing law recognise a principle that a party who knows the other side's understanding of a provision and stays silent is held to that understanding (the text refers to a Delaware "forthright negotiator" idea)? Does deliberately planted ambiguity breach professional-conduct rules in the relevant jurisdiction?
2. (¶7.23–7.26) How have courts in the relevant jurisdiction read "hereunder", "herein", "the foregoing", "except as provided below"?
3. (¶7.34) Is "latent ambiguity" a live doctrine in the jurisdiction, and what evidence does it admit?
4. (¶8.38–8.49) Do courts of the governing law treat "best efforts" as more onerous than "reasonable efforts"? The text asserts US courts overwhelmingly do not, notes two outlier decisions and a 2017 Delaware Supreme Court dissent suggesting otherwise. Verify current position state by state (esp. Delaware post-2017, New York).
5. (¶8.51–8.52) Is the obligor's financial hardship relevant to compliance with a (commercially) reasonable efforts duty? Text reports conflicting S.D.N.Y. decisions.
6. (¶8.54–8.55) Are efforts clauses enforceable without stated criteria (text: Illinois outlier; Texas/Fifth Circuit and New York requiring a goal or guidelines)? Are "efforts to agree" / agreements to negotiate enforceable (text: split between S.D.N.Y., an English case, and the Seventh Circuit)?
7. (¶8.62–8.64) What benchmarks do courts use to assess efforts (past performance, negotiation statements vs parol evidence/integration clauses, industry practice, parallel contracts, "same-entity" test)? Can a narrowly scoped efforts duty require divestiture (Delaware dicta)?
8. (¶8.65–8.75) England: are "best", "all reasonable" and "reasonable endeavours" distinct tiers (text reports first-instance decisions saying yes and a Court of Appeal decision treating two as the same)? Canada (B.C.): "best efforts" higher and "no stone unturned"? Australia and Singapore positions as described? All need current verification.
9. (¶8.82–8.83) UCC §2-306(2) implied best-efforts duty in exclusive dealing and its official comment equating it with reasonable diligence and good faith — verify text and current interpretation.
10. (¶9.3–9.4, ¶9.16, ¶9.88) Is "material" in contracts read by courts in the decision-affecting sense drawn from US securities law, and must a party invoking a MAC make a strong showing (Delaware Chancery)? Verify current Delaware MAC jurisprudence post-2017.
11. (¶9.43) Will a court aggregate adverse changes for MAC purposes without express aggregation wording?
12. (¶9.71) Can transitional wording ("no change in the business which would have" an MAE) confine a MAC clause to internally caused changes?
13. (¶9.104–9.105) Is a field of change limited to "business" read to exclude financial results? Do industry-wide or general economic changes count as a MAC absent a carve-out (text reports mixed authority)?
14. (¶9.112, ¶9.115) Does failure to meet projections fall within "prospects", and is a change in prospects a change in current condition when "prospects" is absent (text: two decisions say no)?
15. (¶9.137–9.138) Does a specific condition limit a general MAC statement (general/specific canon), and may a court infer immateriality from the contract's silence on a topic?
16. (¶10.24–10.28) Inclusive/exclusive readings of from, after, until, to, by, between, before, through under the governing law; statutory rules on computation of time.
17. (¶10.34, ¶10.45) Meaning of "close of business" (English and Irish decisions); whether an act required "at" a time may be done in the following minute (Ontario decision).
18. (¶10.59) Does "upon" an event give an open-ended or a reasonable-time window for exercising a right (New York appellate decision found ambiguity)?
19. (¶10.62–10.66, ¶10.70) Counting conventions for forward periods and minimum-notice periods ("clear"/"entire" days); California's differing readings of "within 30 days prior to" for purchase options vs renewals.
20. (¶10.92–10.97) Does "year"/"calendar year"/"calendar month" mean the calendar unit or a rolling period (text: US vs English divergence)?
21. (¶10.80) US Bankruptcy Code §547 preference look-back periods underlying "one year and a day" non-petition covenants.
22. (¶10.108–10.117) Do courts distinguish "immediately" from "promptly" (text argues both are subject to reasonableness, citing US cases; one S.D.N.Y. statement to the contrary)?
23. (¶11.4–11.8) Will courts read singular to include plural, and how much weight does a singular-includes-plural interpretation clause carry?
24. (¶11.59–11.64) Judicial treatment of exclusive vs inclusive "or", the effect of "either", contra proferentem applied to "or", and "not A or B" (an N.D. Ohio decision reportedly read a prohibition as applying to only one alternative).
25. (¶11.43, ¶11.72–11.74, ¶11.94–11.95, ¶12.69–12.72) Statutory-interpretation examples (Illinois labour statute "and" read as "or"; Ohio LLC statute; California Corporations Code §313; Maine overtime exemption and the missing serial comma) — relevant only as illustrations; verify if ever relied on.
26. (¶11.118–11.121) Construction of insurance-policy ambiguity against the insurer; whether a reading that renders words superfluous can still be "reasonable" (Third Circuit decision criticised by the author).
27. (¶12.13, ¶12.25) Weight of the rule of the last antecedent and of the associated comma rule in the governing jurisdiction.
28. (¶12.36, ¶12.51) Whether courts give effect to presence/absence of a comma, or to ", which" as non-restrictive (Seventh Circuit and New York trial-level decisions reportedly did not).
29. (¶4.89) Enforceability of "buried" terms in consumer contracts.
30. (¶5.98) Regulation S-K Item 601(b)(2) on omitting schedules from filed merger agreements — verify current text.
31. (¶5.112–5.115) What wording suffices to incorporate an unattached document (Florida appellate and E.D. Mich. decisions on "subject to" and bare URLs)? May a party unilaterally amend incorporated online terms?

### 4. Material the author marks as contested, or where the author criticises other approaches

- **Courts' use of "ambiguity" as a catch-all** (¶7.4, ¶7.29, ¶7.34, ¶7.39–7.40): author says courts mislabel under-specificity, mistake and omission as ambiguity, and criticises "latent ambiguity".
- **"Creative ambiguity"** as a negotiating practice (¶7.6–7.7): rejected.
- **Hierarchy of efforts standards** (ch 8 throughout): author says it is an illusion; criticises English first-instance decisions (¶8.65–8.68), the leading British Columbia decision and its "no stone unturned" metaphor (¶8.71–8.73), a Singapore Court of Appeal holding (¶8.75), a Delaware Supreme Court dissent (¶8.48–8.49), Garner's Dictionary of Legal Usage (¶8.77–8.79), law-firm commentary and press reports (¶8.70, ¶8.80). He acknowledges practitioners and some courts will continue to see a hierarchy (¶8.86) — i.e., his view is a minority/prescriptive one in several jurisdictions.
- **Advice of an English firm to use "endeavours" for certainty** (¶8.92–8.93): called unnecessarily timid.
- **New York "clear guidelines" requirement for efforts clauses** (¶8.96): called unrealistic.
- **Definitions of "reasonable efforts" that list mandatory steps** (¶8.115–8.116): rejected as stuffing.
- **Wordy regulatory definitions of "material"** (¶9.6); **"significant"** as the low-threshold word (author's own earlier recommendation, now withdrawn, ¶9.20–9.21).
- **"Double materiality"** (¶9.58–9.63): called a figment of practitioner imagination; standard practice of "scraping" materiality is called unnecessary.
- **Use of both MAC and MAE, literature claiming a substantive difference** (¶9.72–9.77): rejected. **Expanded "change, effect, development ..." formulas** (¶9.87): surplusage. **Quantitative MAC thresholds** (¶9.91–9.97) and **illustrative inclusions in MAC definitions** (¶9.131): discouraged. **"Prospects" fights** (¶9.108–9.114): largely avoidable; author concedes no case law supports his "back door".
- **Gradations of vagueness generally** (¶7.50) including negligence tiers; **immediately vs promptly** (¶10.108–10.122).
- **Month-day-year date format, "the date that is", 12:01/11:59 devices, "close of business", "within", "calendar days", bi-/semi-** (ch 10): all criticised.
- **Traditional definition practice** (¶6.89–6.114): definitions article at the front, "as defined below" parentheticals, "define where first used", two-column Commonwealth format, "means and includes", "shall mean", dictionary-reference clauses — all criticised.
- **Reliance on singular-includes-plural boilerplate** (¶11.8); **the campaign against "and/or"** is called overblown though he still advises against the term (¶11.86–11.91); **Garner's claim that a serial comma never creates ambiguity** (¶12.63) is called mistaken.
- **Judicial competence on and/or and commas** (¶11.111, ¶11.123, ¶11.144, ¶12.25, ¶12.74–12.75): author says judges rely on dictionaries and canons and frequently misanalyse; criticises the Third Circuit's reasoning at length (¶11.122–11.141), an English deputy judge's "Boolean" reading (¶11.109–11.110), the last-antecedent rule and its comma corollary (¶12.13, ¶12.25), and a Canadian regulator's comma-based ruling in which he acted as expert for one side (¶12.30 — note the author's interest).

### 5. Content in the assigned range that is out of scope for legal production (and why)

- **Ch 4 ¶4.1–4.78 (enumeration schemes, headings typography, tabulation mechanics, headers/footers)** and **ch 5 ¶5.1–5.74 (concluding clause wording, signature blocks, notation on signature pages, blank space)**: document formatting and execution formalities; house-style matters rather than analytic method. Not read in detail. (Execution formalities for deeds may matter legally but are jurisdiction-specific and were not read.)
- **Ch 5 ¶5.76–5.90, ¶5.103–5.105** (exhibit vs schedule terminology, attachment numbering, "in" vs "on" a schedule): style conventions with no effect on meaning.
- **Ch 6 ¶6.9–6.11, ¶6.30–6.36, ¶6.64–6.69, ¶6.98–6.109** (a/an before initialisms, article and emphasis conventions for defined terms, two-column layout, Word indexing feature): typographic/style detail.
- **Ch 8 ¶8.19–8.26, ¶8.91** (Ngram and OED history of "endeavours"/"efforts"): evidence for the author's thesis, not a reusable method.
- **Ch 10 ¶10.8–10.13, ¶10.46–10.49** (date format advocacy, how to typeset times): style.
- **Ch 9 deal-tactical remarks on bargaining power and market practice for carve-outs (¶9.134–9.135)**: negotiation strategy dated to 2017 US M&A practice; only marginally relevant.

### 6. Candidate benchmark cases suggested by the text (own words, synthetic)

1. **Cap antecedent.** Clause: parent pays half of a child's tuition "provided that such cost does not exceed" the fee at a named state university. Task: identify whether the cap applies to the half or the whole; propose wording for each. (Tests AD2-04.)
2. **"Hereunder" scope.** A limitation-of-liability sentence in section 9 caps "liability hereunder". Task: state both scopes (section vs agreement) and both senses; recommend a fix without choosing the meaning. (AD2-04)
3. **Full-time status.** Maintenance payments stop when the recipient "resumes full-time work". Recipient takes a 35-hour freelance contract for three months. Task: classify the defect (under-specificity, not ambiguity) and list the unfixed dimensions. (AD2-01, AD2-05)
4. **Restrictive covenant omission.** Covenant permits "one private garage" per lot; owner builds a 450 m² structure for own vehicles. Task: recognise omission of a size limit rather than ambiguity. (AD2-05)
5. **Circular pair.** "Review Date" = date the Supplier decides a Review Period ends; "Review Period" = period starting on a date chosen by the Supplier and ending on a Review Date. Task: detect the cycle and propose an external anchor. (AD2-07)
6. **Stuffed definition.** "Approved Subcontractor" means a subcontractor chosen by Contractor and approved by Owner, such approval not to be unreasonably withheld, which Contractor shall notify within 5 days. Task: separate definition from operative content. (AD2-08)
7. **In-line definition scope.** "Schedule 2 lists all licences, written or oral (the 'Licences'), granted by the Company." Task: show how the parenthetical's position changes what "Licences" covers. (AD2-10)
8. **Mixed efforts standards.** One contract uses "best efforts" for regulatory filings, "commercially reasonable efforts" for marketing, and "all reasonable endeavours" for transition services, governed by English law. Task: inventory, flag inconsistency and copy-paste signs, and state that legal effect needs governing-law research — must not assert equivalence or hierarchy. (AD2-12)
9. **Unmeasured efforts clause.** "Distributor shall use reasonable efforts to sell the Products", plus a termination right if annual sales fall below 10,000 units. Task: flag missing measure/timing, the interaction with the target, and propose controllable absolute sub-obligations and carve-outs. (AD2-13)
10. **Material qualifier placement.** "Seller is not in breach of any material contract." A trivial late payment under the company's largest contract exists; a serious breach exists under a small contract. Task: evaluate accuracy under each threshold and recommend re-placing the qualifier. (AD2-15)
11. **MAC verb formula.** Three variants of a litigation warranty using "will", "could", and "would reasonably be expected to" result in a MAC. Task: rank by favourability to buyer and explain. (AD2-17)
12. **Option window.** "Tenant may exercise the renewal option until 30 June" and "within 30 days of the anniversary". Task: identify boundary-day and direction uncertainty; rewrite with explicit date, time and city time. (AD2-19, AD2-20)
13. **Minimum notice.** "At least ten days' prior notice" of a transfer on 31 December. Task: give the last valid notice day under both counting approaches and propose "entire days" wording. (AD2-20)
14. **Annual allocation with stubs.** Employment contract signed 15 October grants "25 days' leave per year" and a bonus of 1% of "annual revenue". Task: flag meaning of "year", missing stub-period rule, and fairness problem in prorating the revenue-based bonus for a seasonal business. (AD2-21)
15. **Exclusive-right "or".** Lease grants tenant "the exclusive right to operate a kiosk or any other retail facility in the Centre". Landlord lets a second kiosk operator in, arguing tenant chose "other retail facility". Task: state inclusive/exclusive readings and fix. (AD2-23)
16. **Release trigger joined by "and".** Guarantee "terminates upon" (1) the subsidiary ceasing to be wholly owned, (2) its merger, and (3) repayment of all debt. Task: spot the likely connector error and propose "one or more of the following". (AD2-23)
17. **Quantifier under negation.** "If all of the Conditions have not been satisfied by the Longstop Date, either party may rescind"; three of four are satisfied. Task: give both readings, consequences, and rewrite. (AD2-24)
18. **Disability definition.** Insured is "unable to perform any of the duties of his occupation or any occupation for which he is qualified". Task: enumerate readings, assess each independently for surplusage/absurdity, and recommend a rewrite restoring "other". (AD2-25)
19. **Trailing cap.** "The Company shall not seek specific performance or seek damages in excess of the Termination Fee." Task: identify attachment ambiguity and give both rewrites. (AD2-26)
20. **Mid-list exclusion.** "Seller shall transfer the Plant Assets, excluding the Vehicles, the Inventory and the Receivables." Task: two readings; fix with parentheses or enumeration. (AD2-26)
21. **Closing modifier and comma.** "This agreement continues for five years, and thereafter for successive five-year terms, unless terminated on one year's notice." Task: does termination on notice apply during the initial term? Agent must not resolve via comma rule; propose restructure. (AD2-26, AD2-27)
22. **Serial comma / object of preposition.** Exemption for "packing for shipment or distribution of perishable goods". Task: identify whether "distribution" is a separate exempt activity; fix structurally. (AD2-27)
23. **Web terms incorporation.** Order form says services are "subject to the Provider's policies at [URL] as updated from time to time". Task: flag weak incorporation wording and the unilateral-amendment issue; route to research. (AD2-28)
24. **Noise control.** A clean, short NDA with 14 harmless and/or instances and one costly one (permitted disclosure "to affiliates and advisers who are bound by confidentiality"). Task: agent should report only the costly one with reasoning; fail if it reports all 15. (AD2-25)

---

## Part 3 — chapters 13–19 and appendices (IDs AD3-)

Source read: locally extracted text `scratchpad/txt/adams.txt`. The file is a converted e-book; pdf-page numbers are not print pages. Locations below use the book's own numbered paragraphs (¶) and entry/section headings. All findings are in my own words; no model memory or web source was used.

### 1. Coverage record

| pdf-page range | Chapter / section | Status | Note |
|---|---|---|---|
| 584-603 | Ch 13 Selected Usages: entries "action or proceeding" through "as the case may be" (¶13.1-13.76) | Read fully | 17 consecutive entries (see list below) |
| 603-623 | Ch 13: "at least one of X and Y" through "complete and accurate" (¶13.77-13.160) | Not read | Only first lines of "at least one of X and Y" seen |
| 623-629 | Ch 13: "consequential damages" (¶13.161-13.186) | Read fully | |
| 629-634 | Ch 13: "continuously" through "coupled with an interest" | Not read | |
| 634-641 | Ch 13: "curing breach", "deem", "default", "directly" (¶13.210-13.237) | Read fully | |
| 641-654 | Ch 13: "disclaim" through "fixed fee" | Not read | |
| 654-692 | Ch 13: "for any reason or no reason" through "indemnify" (¶13.293-13.441) | Read fully | incl. "for the avoidance of doubt", "including, includes", "incorporated by reference", "indemnify" |
| 692-694 | Ch 13: "indenture", "in other words", "inure" | Not read | |
| 694-705 | Ch 13: "it being understood", "joinder", "joint and several", "knowledge" (¶13.451-13.490) | Read fully | |
| 705-723 | Ch 13: "Latinisms" through "mutual, mutually" | Not read | |
| 723-738 | Ch 13: "negligence, gross negligence", "no later than", "notice", "notwithstanding, subject to, except as provided in", "novation" (¶13.556-13.616) | Read fully | |
| 738-750 | Ch 13: "only" through "proprietary" | Not read | |
| 750-758 | Ch 13: "provided that", "provision", "reasonable, reasonably", "reasonableness and good faith", "regard shall be had to" (¶13.663-13.690) | Read fully | |
| 758-766 | Ch 13: "remediate" through "same" | Not read | |
| 766-771 | Ch 13: "satisfactory", "shareholder or stockholder", "shareholders agreement", "signatory", "silent on", "sole, exclusive" (¶13.722-13.743) | Read fully | |
| 771-780 | Ch 13: "solicit" through "suffer" | Not read | |
| 780-789 | Ch 13: "survival", "termination, expiration", "termination for convenience", "terms and conditions" (¶13.773-13.807) | Read fully | |
| 789-794 | Ch 13: "that certain" through "throughout the universe" | Not read | |
| 794-798 | Ch 13: "time is of the essence", "together with, as well as", "to the extent permitted by law" (¶13.829-13.847) | Read fully | |
| 798-803 | Ch 13: "trademarks—references to" | Not read | |
| 803-815 | Ch 13: "unless and until" through "workmanlike" (¶13.864-13.912) | Read fully | 14 consecutive entries |
| 816-836 | Ch 14 Numbers and Formulas (¶14.1-14.75) | Read fully | |
| 837-842 | Ch 15 Internal Rules of Interpretation (¶15.1-15.23) | Read fully | |
| 843-865 | Ch 16 Typography | Skimmed | Headings scanned; "Emphasis" section (¶16.18-16.36) read fully; fonts, justification, spacing, quotation marks not read |
| 866-884 | Ch 17 — title identified as "Drafting as Writing" | Skimmed | ¶17.1-17.6 read; remaining section headings scanned only (buried verbs, gender-neutral language, wordy phrases, "there is", possessives, initial capitals, extraneous "the", contractions, punctuation) |
| 885-892 | Ch 18 Amendments (¶18.1-18.20) | Read fully | Sample 15 image not present in text |
| 893-898 | Ch 19 — title identified as "Letter Agreements" (¶19.1-19.17) | Read fully | Sample 16 image not present in text |
| 899-900 | Introduction to the appendices | Read fully | |
| 901-919 | Appendix A, "before" agreement with 214 footnote annotations | Read fully | Whole contract and all 214 notes read (more than the first third required) |
| 920-926 | Appendix B, "after" agreement | Read fully | Compared section by section with Appendix A |
| 927-940 | List of works cited; table of cases; index | Not read (first ~40 lines glanced) | Reference apparatus only |

**Chapter 13 entries read in full (80):** action or proceeding; actively; actual, actually; affirmatively, affirmative; allonge; also, in addition; among other things; amongst, whilst; anniversary; annual meeting; anyone; applicable; arising out of or relating to; as amended; as consideration; as liquidated damages and not as a penalty; as the case may be; consequential damages; curing breach; deem; default; directly; for any reason or no reason; force and effect; formal, formally; form and substance; for the avoidance of doubt; fraud and intentional misrepresentation; from the beginning of time; full-time; guarantee, guaranty; guarantee (the verb) as term of art; guarantees that; here- and there- words; in accordance with, according to; including, includes; incorporated by reference; indefinitely, perpetually; indemnify; it being understood; joinder; joint and several; knowledge; negligence, gross negligence; no later [or earlier, more, or less] than; notice; notwithstanding, subject to, except as provided in; novation; provided that; provision; reasonable, reasonably; reasonableness and good faith; regard shall be had to; satisfactory; shareholder or stockholder?; shareholders agreement; signatory; silent on; sole, exclusive; survival; termination, expiration; termination for convenience; terms and conditions; time is of the essence; together with, as well as; to the extent permitted by law; unless and until; unless the context otherwise requires; unless the parties agree otherwise; utmost; very; virgule; voluntarily, involuntarily; warrant, warrant certificate, warrant agreement; warranty, the verb warrant; well and truly; willful, willfully; without limiting the generality of the foregoing; without prejudice; workmanlike.

**Requested entries that do not exist as chapter 13 headings** (heading scan of the whole chapter): best/reasonable efforts, "represents and warrants", shall/will, "sole discretion", "and/or", "in writing", "force majeure". Chapter 13 cross-refers to them elsewhere (efforts: ch 8; represents and warrants: ¶3.374-.416; shall/will: ¶3.72-.103; sole discretion: ¶3.224; and/or: ¶11.86). Those are outside my assigned range and were not read by me. No "force majeure" entry was found in the chapter 13 heading scan.

### 2. Material findings

#### AD3-01
- **ID:** AD3-01
- **Location:** ch 13, ¶13.353-13.387, entry "Including, includes"; also ch 15, ¶15.18.
- **Problem addressed:** Drafters reflexively add "without limitation"/"but not limited to" to every "including", believing this guarantees an illustrative reading.
- **Principle / method / heuristic (own words):** The add-on is usually redundant and cannot be relied on, because a decision-maker may still narrow the general term to things resembling the listed items. The real control is the choice of the general word and the list: (a) choose a precise general word; (b) if relying on its ordinary meaning, do not follow it with obvious members; use "including" only to pull in a borderline item that might otherwise fall outside; (c) if the general word has a special or contract-created meaning, give an exhaustive list or a definition instead; (d) an interpretation clause deeming "including" to mean "including without limitation" does not cure the problem. Putting the general word last (list + "and other X") tends to increase the narrowing risk unless the catch-all is expressly widened.
- **Assumptions and applicability:** Author's reasoning rests on US case law; common-law negotiated contracts. The drafting logic (list choice drives scope) is jurisdiction-neutral; the litigation-risk claim is not verified authority.
- **Production responsibility affected:** drafting, review/redlining, issue spotting.
- **Workflow / decision implication:** In review, do not treat the presence or absence of "without limitation" as the issue. For each "including" list, classify the listed items (obvious members vs. borderline enlarging items) and ask whether the list could be read as narrowing the class; recommend deleting obvious examples, tightening the general word, or converting to a definition.
- **Evaluation evidence or criterion:** Given a clause with a general term plus an obvious-members list, the agent flags the narrowing risk and proposes one of the three fixes; it does not merely add or delete "without limitation".
- **Failure / misuse conditions:** Mechanically stripping "without limitation" from a counterparty's paper with no substantive gain, generating negotiation friction; deleting examples that the client actually needs for commercial clarity.
- **Repair implication:** Where examples must stay, move them to the front with an expressly widened catch-all, or define the term exhaustively.
- **Proposed disposition:** adapt — strong review heuristic; the legal-risk premise must be jurisdiction-checked before being stated to a user as law.

#### AD3-02
- **ID:** AD3-02
- **Location:** ch 13, ¶13.599-13.613, entry "Notwithstanding, subject to, except as provided in".
- **Problem addressed:** Override language that works at a distance hides from the reader which provisions are undercut; blanket overrides and competing overrides create conflict.
- **Principle / method / heuristic (own words):** Prefer flagging the *subordinate* provision ("subject to section X") over flagging the dominant one ("notwithstanding section Y"), and name the specific section. "Except as provided in" is narrower than "subject to" (pure exception vs. any kind of qualification). A contract-wide "notwithstanding anything to the contrary" leaves the reader to find what is affected, may affect nothing, and two such clauses can collide. "Subject to the terms of this agreement" before a key grant or obligation is usually surplus because the contract is read as a whole, though it is acceptable shorthand where many conditions and termination rights qualify a core obligation. Separately: do not leave superseded text in place and neutralise it with an override or proviso for diplomatic reasons; delete it, because the "dead" text can be argued to retain effect.
- **Assumptions and applicability:** Negotiated commercial agreements. The author expressly accepts "notwithstanding" as a practical tool when marking up the other side's draft late in a deal because it needs only one insertion.
- **Production responsibility affected:** drafting, review/redlining, product consistency, change impact.
- **Workflow / decision implication:** A review agent should build an override map: every "notwithstanding", "subject to", "except as provided", and proviso, with source and target provisions, and flag (i) untargeted blanket overrides, (ii) multiple provisions each claiming supremacy, (iii) nullified language left in the draft. When redlining under time pressure, a single "notwithstanding section X" insertion is an acceptable smallest change, but the agent should note the clarity cost.
- **Evaluation evidence or criterion:** On a test contract with two provisions each prefaced by an agreement-wide override, the agent identifies the conflict and states which provisions each could affect.
- **Failure / misuse conditions:** Rewriting every "notwithstanding" in counterparty paper as "subject to" (multiple edits, cross-reference risk) when the instruction is minimal change.
- **Repair implication:** Replace blanket overrides with named-section references; remove nullified text rather than layering overrides.
- **Proposed disposition:** retain — directly usable as a redline decision rule, including its own exception for minimal-change markups.

#### AD3-03
- **ID:** AD3-03
- **Location:** ch 13, ¶13.663-13.666, entry "Provided that"; applied in Appendix A notes 24, 31, 71, 130, 208.
- **Problem addressed:** Provisos blur whether the following text is a condition, an exception, a limitation or an independent addition; the difference can decide whether non-compliance is a breach or takes conduct outside a grant.
- **Principle / method / heuristic (own words):** Classify what each proviso is doing, then replace it with wording that states that relationship: exception ("except that"), limitation ("and in any event"), condition ("on condition that"), or addition (fold into the main clause or a new sentence). Where a proviso narrows a general proposition, restate the proposition narrowly instead of stating it broadly and cutting back.
- **Assumptions and applicability:** Any contract; particularly important in licence grants and payment triggers.
- **Production responsibility affected:** review/redlining, drafting, issue spotting.
- **Workflow / decision implication:** For every "provided that", the agent records the intended category and flags any where the category is genuinely uncertain as a substantive ambiguity (not a style point) requiring instruction.
- **Evaluation evidence or criterion:** Given a licence "provided that" the licensee does X, the agent identifies the condition-versus-covenant ambiguity and asks which consequence is intended.
- **Failure / misuse conditions:** Silently choosing a category when redrafting, thereby changing the deal.
- **Repair implication:** Where intent is unknown, keep the text and raise a query; where known, substitute the precise connector.
- **Proposed disposition:** retain.

#### AD3-04
- **ID:** AD3-04
- **Location:** ch 13, ¶13.310-13.319 "For the avoidance of doubt"; ¶13.451-13.455 "It being understood"; ¶13.898-13.906 "Without limiting the generality of the foregoing"; ¶13.18-13.21 "Among other things".
- **Problem addressed:** Filler connectors that claim to clarify but either restate, add an unrelated provision, add rhetorical emphasis, or disguise an acknowledgment.
- **Principle / method / heuristic (own words):** Whatever follows such a phrase must be able to stand alone. Diagnose which of four jobs the text is doing: (1) a real inclusion/exclusion from scope — state it directly or fold it into the definition; (2) the obvious — delete; (3) a separate provision unrelated to what precedes — delete the connector; (4) acceptance of a fact asserted by the other side — recast as an acknowledgment. "For clarity" is treated the same way. "The foregoing" is itself uncertain in reach.
- **Assumptions and applicability:** General; the author states a categorical "don't use" position.
- **Production responsibility affected:** review/redlining, drafting.
- **Workflow / decision implication:** Review check: for each such phrase, test whether the trailing text is consistent with the text it purports to clarify. If it actually changes scope, flag it as a substantive carve-in/carve-out hidden as clarification.
- **Evaluation evidence or criterion:** Agent detects a "for the avoidance of doubt" sentence that contradicts or extends the preceding clause and reports it as a substantive change.
- **Failure / misuse conditions:** Treating the phrase as purely cosmetic and deleting it together with a needed carve-out.
- **Repair implication:** Keep the substance, drop the connector, restructure as exception or definition.
- **Proposed disposition:** retain.

#### AD3-05
- **ID:** AD3-05
- **Location:** ch 13, ¶13.161-13.186, entry "Consequential damages".
- **Problem addressed:** Boilerplate exclusions of "consequential", "special", "incidental", "indirect" loss are poorly understood by those who agree to them, overlap, and may strip the only meaningful remedy (the author's example is breach of confidentiality).
- **Principle / method / heuristic (own words):** Do not exclude loss by doctrinal label. Work from the party's actual concern: if the worry is remote loss, say unforeseeable loss is excluded; if the worry is quantum, use a cap; if specific heads of loss matter, name them in plain terms, or define what *is* recoverable. Treat "lost profits" as unstable whichever way it is handled (profits can be the direct loss). Piling up labels (e.g., excluding both direct and indirect) can produce incoherence.
- **Assumptions and applicability:** Author draws on US and two English cases; sale of goods, services, NDAs, technology contracts. Characterisation of loss is jurisdiction-specific — see section 3.
- **Production responsibility affected:** issue spotting, review/redlining, risk communication, escalation.
- **Workflow / decision implication:** When reviewing a limitation clause, test it against the most likely breach scenarios for that contract type ("what loss would this client actually suffer, and would this clause remove it?") rather than checking for standard wording. Flag NDAs and data clauses with blanket consequential-loss exclusions.
- **Evaluation evidence or criterion:** For a confidentiality agreement containing a mutual consequential-loss exclusion, the agent reports that the discloser's likely loss may fall inside the exclusion.
- **Failure / misuse conditions:** Replacing market-standard wording with novel wording without client/supervisor sign-off; asserting how a court would classify a loss.
- **Repair implication:** Offer alternatives (foreseeability exclusion, cap, named heads) and escalate choice to the responsible lawyer.
- **Proposed disposition:** adapt — scenario-testing method retained; any statement of how loss is classified must go through research/authority verification.

#### AD3-06
- **ID:** AD3-06
- **Location:** ch 13, ¶13.399-13.441, entry "Indemnify" (incl. sub-headings "Don't use indemnify and hold harmless", "Defend is inadequate", "Indemnify as a term of art").
- **Problem addressed:** Indemnity clauses are inserted by habit, with synonym strings and multiple prepositions that invite arguments about extra meaning, and without saying what claims or losses are covered.
- **Principle / method / heuristic (own words):** First ask whether indemnity is needed at all: it earns its place when a party needs a deeper pocket, cover for a disclosed problem, cover for events outside the other party's control, cover for non-party claims, fee recovery, or structured limits (cap, basket, shorter claim period, exclusive remedy, procedures). If used: use a single verb; state expressly whether inter-party claims are covered as well as non-party claims; cover both losses and liabilities through a defined term listing what is recoverable (so payment first is not required); deal with control and funding of defence in a procedures clause rather than by the bare word "defend". If a counterparty resists the word itself, "will be liable for" can carry the same allocation.
- **Assumptions and applicability:** Common-law commercial and M&A contracts; author notes divided case law on several points.
- **Production responsibility affected:** scoping, issue spotting, drafting, review/redlining.
- **Workflow / decision implication:** Indemnity review checklist: purpose served; claims covered (direct / third-party); losses defined; procedures; interaction with caps and with excluded-loss clauses; exclusivity of remedy.
- **Evaluation evidence or criterion:** Agent's review of an indemnity clause reports, as separate items, (i) whether inter-party claims are covered, (ii) whether defence procedure is addressed, (iii) interaction with the limitation clause.
- **Failure / misuse conditions:** Deleting "hold harmless" in a jurisdiction or sector where the doublet has an understood function without checking; treating an indemnity as always pro-claimant.
- **Repair implication:** Propose defined "indemnifiable losses" plus procedures; escalate where the governing law's treatment of the terms is unknown.
- **Proposed disposition:** adapt.

#### AD3-07
- **ID:** AD3-07
- **Location:** ch 13, ¶13.671-13.688 "Reasonable, reasonably" and "Reasonableness and good faith"; ¶13.722-13.723 "Satisfactory".
- **Problem addressed:** Standards of conduct are mixed or stacked without regard to whether they are objective or subjective.
- **Principle / method / heuristic (own words):** Reasonableness is an objective test; good faith looks to the actor's honest state of mind. The party benefiting from another's performance normally wants the objective test; the performing party may prefer good faith. Good faith fits where a party takes a position (contesting, claiming) and for obligations to negotiate. Stacking both is normally redundant, except where the concern is both adequacy of steps and absence of pretext. "Satisfactory to X" is ambiguous between the two tests; say which. "Reasonably" adds nothing before "promptly", "likely", or "cooperate".
- **Assumptions and applicability:** Assumes a legal system with some implied good-faith doctrine as default; this varies sharply by jurisdiction (research question).
- **Production responsibility affected:** issue spotting, drafting, review/redlining, risk communication.
- **Workflow / decision implication:** For each discretion, approval or satisfaction right, the agent records the standard that applies and whose interest it serves, and flags unqualified "satisfactory"/"discretion" wording as an open standard.
- **Evaluation evidence or criterion:** Given "in form satisfactory to Customer", the agent flags objective/subjective ambiguity and identifies which reading favours the client.
- **Failure / misuse conditions:** Assuming an implied good-faith duty exists under the governing law.
- **Repair implication:** State the standard explicitly ("from the perspective of a reasonable person in X's position", or actual satisfaction).
- **Proposed disposition:** retain with jurisdiction qualification.

#### AD3-08
- **ID:** AD3-08
- **Location:** ch 13, ¶13.783-13.794 "Termination, expiration"; ¶13.773-13.782 "Survival"; ¶13.254-.255 cross-referenced ("during the term").
- **Problem addressed:** Inconsistent end-of-contract vocabulary lets a party argue that a post-termination consequence does not apply on expiry (or vice versa); survival clauses are unfocused.
- **Principle / method / heuristic (own words):** Use one verb ("terminate") for every way the contract ends; never pair "terminate and expire". When a clause is triggered by ending, say which kind of ending it means (end of term, party election, or both) and cite the sections. "If this agreement terminates" and "if this agreement is terminated" can be read differently; use the active voice and name the actor. For survival: build duration into the obligation itself (e.g., during the term and N years after) rather than relying on a list of surviving sections; a clause preserving accrued claims states the obvious; for indemnity, a direct time-limits section is preferable to "survival of representations". Keep the terminology aligned across related contracts.
- **Assumptions and applicability:** General; especially term-based services, licence and subscription agreements.
- **Production responsibility affected:** review/redlining, product consistency, change impact, drafting.
- **Workflow / decision implication:** Consistency pass: list every termination/expiry reference and every post-termination consequence, and check each consequence is triggered by every intended mode of ending. Cross-check linked documents (order forms, DPAs, SOWs) for the same vocabulary.
- **Evaluation evidence or criterion:** Agent finds that a data-return obligation is triggered "on termination" while the term clause speaks only of "expiry", and flags the gap.
- **Failure / misuse conditions:** Deleting a survival clause from a contract whose obligations do not carry their own duration.
- **Repair implication:** Add explicit duration to each continuing obligation before removing survival language.
- **Proposed disposition:** retain.

#### AD3-09
- **ID:** AD3-09
- **Location:** ch 13, ¶13.585-13.598, entry "Notice" (sub-heading "Termination with prior notice").
- **Problem addressed:** "Notice" can mean advance warning or after-the-fact information; "terminate upon/by giving/with N days' notice" leaves unclear when termination takes effect and whether a date restriction applies to giving notice or to termination.
- **Principle / method / heuristic (own words):** Use the verb "notify" with an explicit timing element, and draft termination-on-notice as a two-step statement: if a party notifies, the agreement ends a stated number of days after receipt. If the right only arises after an event, make clear whether notice may be given before it.
- **Assumptions and applicability:** General.
- **Production responsibility affected:** drafting, review/redlining.
- **Workflow / decision implication:** For every notice-based right, the agent extracts: who notifies, when notice may first be given, when it is effective, and when the consequence occurs; any missing element is flagged.
- **Evaluation evidence or criterion:** Agent flags "after the first anniversary, either party may terminate on 60 days' notice" as ambiguous on earliest notice date.
- **Failure / misuse conditions:** Over-flagging where the notices clause already fixes effectiveness.
- **Repair implication:** Redraft to the two-step form.
- **Proposed disposition:** retain.

#### AD3-10
- **ID:** AD3-10
- **Location:** ch 13, ¶13.829-13.840 "Time is of the essence"; ¶13.66-13.73 "As liquidated damages and not as a penalty"; ¶13.795-13.806 "Termination for convenience"; ¶13.293-13.298 "For any reason or no reason".
- **Problem addressed:** Formulaic phrases are used as if they were switches that produce a legal result, without saying what the result is or to which obligation it applies.
- **Principle / method / heuristic (own words):** Replace the formula with the outcome wanted. For deadlines: identify the deadline, give an express termination right, and optionally record why timing matters. For agreed damages: keep a characterisation but make it meaningful — record that loss is hard to estimate and that the sum is intended as compensation, ideally with the reason. For at-will exit: "for any reason" suffices; "or no reason" and "at any time" add nothing; "for convenience" invites an argument that some inconvenience is needed; if the aim is to avoid explaining, say no explanation is required. None of these phrases should be assumed to displace an implied good-faith duty.
- **Assumptions and applicability:** Author explicitly notes civil-law systems may resist termination for trivial delay. Penalty/liquidated damages rules are jurisdiction-specific.
- **Production responsibility affected:** issue spotting, drafting, review/redlining, risk communication.
- **Workflow / decision implication:** When these phrases appear, the agent asks "what consequence is intended and is it stated elsewhere?" and checks for inconsistency (e.g., a time-of-essence clause alongside a cure period or delay damages).
- **Evaluation evidence or criterion:** Agent detects a general time-of-essence clause coexisting with a 30-day cure right and reports the tension.
- **Failure / misuse conditions:** Removing the phrase where local law gives it a settled effect the client relies on.
- **Repair implication:** Substitute explicit consequence clauses; escalate enforceability questions.
- **Proposed disposition:** adapt.

#### AD3-11
- **ID:** AD3-11
- **Location:** ch 13, ¶13.210-13.215 "Curing breach"; ¶13.223-13.234 "Default".
- **Problem addressed:** Blanket cure rights are granted without asking what "cure" means for a given breach.
- **Principle / method / heuristic (own words):** Some breaches cannot be undone (destroyed subject matter, completed prohibited transfer); for missed deadlines, "cure" simply means more time. A general cure right therefore works as advance permission to breach; grant cure selectively (late payment being the natural case) and limit it to breaches that can actually be remedied. "Has occurred and is continuing" does not fit one-off events or inaccurate statements of fact; framing by whether the event has been cured is more workable, though "curable" itself can be disputed. Defined-term labels should signal meaning (e.g., "potential default" rather than a bare "default" alongside "event of default").
- **Assumptions and applicability:** Commercial contracts; the "default" material is finance-oriented.
- **Production responsibility affected:** issue spotting, drafting, review/redlining.
- **Workflow / decision implication:** For each termination-for-breach clause, the agent tests the cure mechanism against two or three concrete breach types for that contract (confidentiality leak, missed SLA, non-payment) and reports where cure is meaningless or over-generous.
- **Evaluation evidence or criterion:** Agent notes that a 30-day cure period applied to a confidentiality breach gives no real protection.
- **Failure / misuse conditions:** Stripping cure rights from a client who is the likely breaching party.
- **Repair implication:** Differentiate cure by obligation type.
- **Proposed disposition:** retain.

#### AD3-12
- **ID:** AD3-12
- **Location:** ch 13, ¶13.556-13.578 "Negligence, gross negligence"; ¶13.896-13.897 "Willful, willfully"; ¶13.320-13.327 "Fraud and intentional misrepresentation".
- **Problem addressed:** Carve-outs from liability caps and exclusions rely on tort labels whose meaning differs between jurisdictions, and on "wilful", which does not say whether intent attaches to the act or to the harm.
- **Principle / method / heuristic (own words):** Avoid "gross negligence" unless the governing law's meaning has been researched; if a higher-than-negligence threshold is needed use "reckless"; use "intentional" and tie it to the consequences rather than the act; do not define recklessness; adapt to the governing law's own categories; and question whether tort-based carve-outs belong at all against liability for ordinary contractual non-performance, because a deliberate commercial decision not to perform could then escape the cap. For fraud carve-outs, describing the conduct (knowingly supplying false information or knowingly withholding information) is clearer than doctrinal labels.
- **Assumptions and applicability:** Author's analysis is US-based and he flags that non-US systems may use different frameworks. Highly relevant to technology and outsourcing liability clauses.
- **Production responsibility affected:** issue spotting, research, review/redlining, escalation.
- **Workflow / decision implication:** Whenever a cap carve-out uses "gross negligence" or "wilful misconduct/default", the agent (i) flags that meaning depends on governing law, (ii) triggers a research task, (iii) tests whether a deliberate refusal to perform would fall inside the carve-out and so uncap liability.
- **Evaluation evidence or criterion:** Agent's issue list for a limitation clause includes the act-versus-consequence ambiguity of "wilful" and the governing-law dependency of "gross negligence".
- **Failure / misuse conditions:** Importing US-style vocabulary into a contract governed by another law; stating a meaning for "gross negligence" without authority.
- **Repair implication:** Replace labels with conduct descriptions, or escalate for jurisdiction-specific wording.
- **Proposed disposition:** adapt; research further on governing-law meaning.

#### AD3-13
- **ID:** AD3-13
- **Location:** ch 13, ¶13.37-13.53, entry "Arising out of or relating to".
- **Problem addressed:** Scope of governing-law, forum and arbitration clauses is set by two vague connectors; the broad one may sweep in unforeseen disputes, and the narrow one cannot be relied on to keep non-contract claims out.
- **Principle / method / heuristic (own words):** Define scope by reference to the activities the parties will carry out under the deal (e.g., the agreement plus the recipient's handling and use of confidential information), rather than by reference to "the contract" plus a vague extender. If the aim is genuinely to confine the clause to contractual claims, say so with an express exclusion of extra-contractual liability.
- **Assumptions and applicability:** Dispute-resolution and liability-limitation clauses; the author concedes the conventional phrase is entrenched (including in institutional model clauses).
- **Production responsibility affected:** drafting, review/redlining, issue spotting.
- **Workflow / decision implication:** The agent should ask what categories of dispute the client wants covered (contract, tort, statutory, IP validity) and check the clause against that list, rather than accepting the stock phrase. Where an arbitral institution's model wording is used, departures should be escalated.
- **Evaluation evidence or criterion:** Agent identifies whether a data-misuse tort claim would fall within a given jurisdiction clause and records uncertainty if not determinable.
- **Failure / misuse conditions:** Rewriting an institutional model arbitration clause on style grounds, jeopardising recognised wording.
- **Repair implication:** Add activity-based scope language alongside, not instead of, recognised wording where risk-averse.
- **Proposed disposition:** qualify — the author's view is a minority position against entrenched practice.

#### AD3-14
- **ID:** AD3-14
- **Location:** ch 13, ¶13.54-13.60 "As amended"; ch 15, ¶15.11-15.12; ¶13.388-13.393 "Incorporated by reference".
- **Problem addressed:** References to statutes and other contracts do not say which version is meant; "incorporation by reference" is used where a simple reference would do.
- **Principle / method / heuristic (own words):** For compliance obligations, "as amended" is unnecessary (compliance is always measured against the current version). Where a contract borrows a *definition or element* from a statute or another agreement, the drafter must choose: frozen at signing, or as in force when the provision applies — and say so. Reserve incorporation for genuinely importing another document's provisions, and then describe what is happening (party X makes to Y the statements made in agreement Z) rather than using the label. Merely referring to a schedule already brings it in.
- **Assumptions and applicability:** General; very relevant to product terms that reference policies, DPAs, price lists, or statutory definitions.
- **Production responsibility affected:** drafting, product consistency, change impact.
- **Workflow / decision implication:** Change-impact check: for every external reference (statute, policy URL, other agreement), record whether it is static or dynamic. Dynamic references to a document one party controls are a unilateral-variation issue to flag.
- **Evaluation evidence or criterion:** Agent lists all borrowed definitions and states for each whether the version is fixed or floating, or flags it as unspecified.
- **Failure / misuse conditions:** Assuming a floating reference is acceptable in consumer terms (fairness law may intervene — research question).
- **Repair implication:** Add "as in effect on the date of this agreement" or "as then in effect".
- **Proposed disposition:** retain.

#### AD3-15
- **ID:** AD3-15
- **Location:** ch 15, ¶15.1-15.23 (whole chapter); ch 13, ¶13.866-13.867 "Unless the context otherwise requires".
- **Problem addressed:** Boilerplate "Interpretation" sections are copied without asking whether each rule does anything.
- **Principle / method / heuristic (own words):** Sort internal interpretation rules into three classes. *Possibly useful:* rules that fix a meaning for a recurring expression — time-zone for times of day, roll-forward of deadlines to the next business day, a rounding convention. *Unnecessary:* rules stating what is obvious or better handled by drafting — references are to this agreement's sections, singular/plural of defined terms, "as amended" for agreements and statutes, gender, here- words, from/to date conventions. *Overreaching:* rules that try to impose order that the text does not have — headings ignored, "including" means without limitation, "or"/"and" rules, "will" equals "shall", "shall" is mandatory, singular includes plural, persons include successors. "Unless the context otherwise requires" reintroduces the uncertainty the rule was meant to remove; deviations should be stated specifically. Autonomous definitions belong in the definitions section, not among interpretation rules. General point: if readers need a rulebook to parse basic usages, the drafting is at fault.
- **Assumptions and applicability:** Author's classification; some jurisdictions' practice (e.g., long UK-style interpretation clauses) differs, and he does not address statutory interpretation acts.
- **Production responsibility affected:** review/redlining, drafting, product consistency, evaluation.
- **Workflow / decision implication:** A review agent should never treat an interpretation clause as curing an ambiguity in the body; it should test the body text on its own. When asked to tidy a template, triage each rule into the three classes. When reviewing counterparty paper, leave harmless rules alone (not worth negotiation capital) but flag rules that mask real ambiguity (headings, "or", "including").
- **Evaluation evidence or criterion:** Given an ambiguous "A or B" obligation and an interpretation clause saying "or is not exclusive", the agent still reports the ambiguity.
- **Failure / misuse conditions:** Deleting a business-day roll-forward or time-zone rule that the body depends on.
- **Repair implication:** Fix ambiguity at source; keep only type-one rules that are actually used.
- **Proposed disposition:** retain.

#### AD3-16
- **ID:** AD3-16
- **Location:** ch 18, ¶18.3-18.4 and ¶18.10-18.19 (Amendments: "Amending, or amending and restating"; "Distinguishing between amending and supplementing"; "Adding, deleting, and replacing language").
- **Problem addressed:** How to document changes to a signed contract so the change is visible, accurate and does not break the rest of the document.
- **Principle / method / heuristic (own words):** Three decisions. (1) *Vehicle:* a discrete amendment for a few changes; amend-and-restate when changes are extensive or a chain of earlier amendments has become hard to follow; a free-standing addition that does not say it is inserted into the original is a supplement, not an amendment. (2) *Granularity within a provision:* either state the exact substitution (shorter, highlights the change, but unintelligible without the original) or restate the whole provision as amended (self-contained, but hides what changed; the reason can go in recitals). The choice is a trade-off to be made case by case. (3) *Structural side-effects:* inserting or deleting numbered provisions disturbs numbering and cross-references in the contract and in other contracts that cite it; prefer adding at the end, and on deletion keep the number with an "intentionally omitted" placeholder. Punctuation/conjunction tidy-ups in enumerated lists are strictly correct but harmless to omit. Amending words are language of performance ("is hereby amended"); number amendments serially; do not define "this Amendment".
- **Assumptions and applicability:** Formal written amendments between the same parties; does not address unilateral variation of online terms or amendment formalities under particular laws.
- **Production responsibility affected:** drafting, change impact, product consistency, review/redlining.
- **Workflow / decision implication:** This gives a concrete "smallest sufficient change" rule-set: an amending agent must (i) pick vehicle by volume and amendment history, (ii) pick substitution vs. full restatement by weighing visibility against self-containment, (iii) run a cross-reference impact check across the contract *and* related documents before renumbering, defaulting to non-renumbering techniques.
- **Evaluation evidence or criterion:** Given a request to delete clause 10 of a 20-clause agreement cited by a separate SOW, the agent proposes a placeholder rather than renumbering and lists affected cross-references.
- **Failure / misuse conditions:** Restating a whole agreement for a one-word change; renumbering without checking external references; labelling a supplement as an amendment.
- **Repair implication:** Where a chain of amendments already exists, recommend a consolidated amended-and-restated version.
- **Proposed disposition:** retain — core input for change-impact and redlining skills.

#### AD3-17
- **ID:** AD3-17
- **Location:** Introduction to appendices (pdf-pp 899-900) and Appendix A notes 1-214 compared with Appendix B.
- **Problem addressed:** What a disciplined review-and-redraft of a mainstream contract looks like in practice, and how to separate language work from deal work.
- **Principle / method / heuristic (own words):** The method shown is: annotate the existing text point by point, each note naming the defect, the fix, and the rule relied on; then redraft language and structure while leaving the commercial terms untouched and expressly disclaiming any view on them. Notes fall into recognisable classes: wrong verb category (duty language used for policy, discretion, or on a non-party); archaism and redundancy; wordy phrases and buried verbs; defined-term hygiene (used once, uninformative label, nested definitions, undefined term actually used); repeated parenthetical cross-references; structure (definitions relocated and alphabetised, a long section split, pointer provisions replaced by stating the content); and — crucially — *logic defects* surfaced only by close reading (an initial term that can never be non-renewed as written; an open question whether extensions continue after a change-of-control extension; a sentence duplicating what a definition already achieves; a modifier that may attach to the wrong limb). The author reports the redraft as about 86% of the original word count despite some longer boilerplate, and claims structural/logic problems hide in conventional prose.
- **Assumptions and applicability:** A template owned by the reviewer's side (full redraft permitted). Not a model for marking up a counterparty's draft. Author states neither appendix is for use as a template and that deal terms were not updated since the 2nd edition.
- **Production responsibility affected:** review/redlining, drafting, product consistency, evaluation.
- **Workflow / decision implication:** A review agent's output should be structured as discrete, rule-cited annotations classified by type, with logic/substance defects separated from style defects and ranked above them; the agent must state explicitly that commercial terms were not assessed (or were assessed separately).
- **Evaluation evidence or criterion:** On a seeded test contract, the agent (i) finds the seeded logic defect, (ii) keeps style notes separate, (iii) preserves deal terms in the redraft (diff of obligations, amounts, triggers shows no change).
- **Failure / misuse conditions:** Drowning one substantive defect in 200 stylistic notes; stylistic redraft that silently changes an obligation.
- **Repair implication:** Add a post-redraft equivalence check: list every obligation, right, condition, amount and date before and after.
- **Proposed disposition:** retain.

#### AD3-18
- **ID:** AD3-18
- **Location:** Appendix A, note 86 (on "substantially"); notes 184, 195, 196, 203 (boilerplate replaced wholesale); compare Appendix B §§ 8, 10, 11, 13; also notes 91-92, 97 with Appendix B definitions of "Cause" and "Good Reason".
- **Problem addressed:** Knowing when *not* to fix, and when patching is worse than replacement.
- **Principle / method / heuristic (own words):** The author leaves a known vague word in place because removing it everywhere would demand extensive change — an explicit cost/benefit stop rule. Conversely, for four boilerplate sections he judges clause-level clean-up not worth it and substitutes complete alternative provisions, saying full analysis is out of scope. Where he replaces "material", he substitutes an explicit reasonable-person significance test, which is a substantive clarification rather than a style edit.
- **Assumptions and applicability:** Own-template redrafting.
- **Production responsibility affected:** review/redlining, change impact, escalation.
- **Workflow / decision implication:** A redrafting agent needs three modes and must say which it used per clause: edit in place; leave with a recorded reason; replace wholesale from an approved clause source. Substituting an explicit standard for a vague word must be reported as a change in substance.
- **Evaluation evidence or criterion:** Agent output includes a "left unchanged — reason" list and a "replaced wholesale — source" list.
- **Failure / misuse conditions:** Wholesale boilerplate replacement in a negotiated deal; treating "material" replacement as cosmetic.
- **Repair implication:** Route wholesale replacements and standard-changing edits for human approval.
- **Proposed disposition:** retain.

#### AD3-19
- **ID:** AD3-19
- **Location:** ch 14, ¶14.20-14.63 (Formulas), esp. ¶14.23-14.46 and ¶14.53-14.63.
- **Problem addressed:** Prose formulas are ambiguous about order of operations, and drafting slips in ordering can change the amount payable by large sums.
- **Principle / method / heuristic (own words):** Any formula mixing operations must fix the order, using "the result of", step-by-step phrasing, or enumeration (equivalent to brackets); for three or more nested operations use enumeration; avoid "and" for addition, "excess of A over B", and "difference between". Complex formulas are clearer as equations with a variable key, and a worked example in a schedule helps. State rounding increment, direction and half-way treatment; for pro-rata allocation of a fixed pool, round down. Avoid a percent sign inside an equation.
- **Assumptions and applicability:** Any pricing, fee, royalty, service-credit or earn-out mechanism.
- **Production responsibility affected:** issue spotting, drafting, review/redlining, evaluation.
- **Workflow / decision implication:** The agent should parse every formula into an explicit expression, test it with sample numbers under each plausible grouping, and flag any formula whose result differs between groupings. It should propose a worked example for complex mechanisms.
- **Evaluation evidence or criterion:** For "X% of price above threshold less costs", the agent produces both readings with numeric results and flags the ambiguity.
- **Failure / misuse conditions:** Rewriting a commercial formula and changing the economics; assuming mathematical precedence conventions bind contract readers.
- **Repair implication:** Enumerate or convert to an equation and confirm the intended reading with the business owner.
- **Proposed disposition:** retain.

#### AD3-20
- **ID:** AD3-20
- **Location:** ch 14, ¶14.64-14.75 "Consecutive ranges of numbers" (stepped vs shifting flat rates; gaps and overlaps).
- **Problem addressed:** Tiered tables do not say whether a tier's rate applies to the whole quantity or only to the slice within the tier, and tier boundaries overlap or leave gaps.
- **Principle / method / heuristic (own words):** A bare tier table is ambiguous between a marginal ("stepped") and whole-amount ("shifting flat") rate; resolve by a tax-table style layout (fixed sum plus rate on the excess), by "of the next …" phrasing, or by an express preamble. Check boundaries: "1-10" and "10-20" overlap; for continuous quantities use "over X but not over Y"; gaps are tolerable only for whole-unit quantities; date ranges carry the same risk.
- **Assumptions and applicability:** Pricing, royalty, volume-discount, service-credit tables — common in technology and commercial contracts.
- **Production responsibility affected:** issue spotting, review/redlining.
- **Workflow / decision implication:** Automatic check on every tiered table: (i) marginal or whole-amount stated? (ii) boundary values assigned to exactly one tier? (iii) units discrete or continuous?
- **Evaluation evidence or criterion:** Agent flags a usage-pricing table with tiers "0-1000" and "1000-5000" for overlap and unstated rate type.
- **Failure / misuse conditions:** None significant; low-cost, high-value check.
- **Repair implication:** Re-express boundaries and add a rate-type preamble.
- **Proposed disposition:** retain.

#### AD3-21
- **ID:** AD3-21
- **Location:** ch 14, ¶14.1-14.16 "Words or digits"; Appendix A note 122.
- **Problem addressed:** Stating numbers twice (words plus digits) is meant as error insurance but creates a second source of inconsistency, typically when the digits are revised and the words are not, and a words-prevail rule may then select the unintended figure.
- **Principle / method / heuristic (own words):** State each number once; this is an instance of the broader rule against saying the same thing twice. The author's convention: words up to ten, digits from 11, with listed exceptions; consistency matters more than the particular convention. The safeguard against digit errors is proofreading.
- **Assumptions and applicability:** General. The author notes some legal instruments have statutory conflict rules (research question).
- **Production responsibility affected:** review/redlining, product consistency, change impact.
- **Workflow / decision implication:** Mechanical check: every words-plus-digits pair must match; after any edit to an amount or period, re-verify all duplicate statements of it (including schedules and order forms).
- **Evaluation evidence or criterion:** Agent catches a mismatched words/digits amount in a seeded draft.
- **Failure / misuse conditions:** Stripping dual statement from documents where a regulator, bank or counterparty requires it.
- **Repair implication:** Single statement of each number; if dual statement is required, add to the verification checklist.
- **Proposed disposition:** retain (merge into a general "no duplicate statement" consistency rule).

#### AD3-22
- **ID:** AD3-22
- **Location:** ch 13, ¶13.878-13.892, entry "Warranty, the verb warrant"; ¶13.216-13.222 "Deem"; ¶13.476-13.490 "Knowledge".
- **Problem addressed:** Verb and label choices ("warrants", "deemed", "to the best of its knowledge") are used as if the label determines legal character.
- **Principle / method / heuristic (own words):** (a) Whether something operates as a warranty depends on content, not on the label or the section heading; statements elsewhere in the contract may be treated as warranties and vice versa. A promise about future performance of a product is more clearly drafted as "if the product fails to conform during period P, supplier shall [remedy]" than as a future-fact statement followed by a separate remedy sentence. Do not use "warrants that it shall". (b) "Deem" is for legal fictions only and takes "will", not "shall"; an automatic ("deemed") release removes dependence on the releasing party's later act. (c) Knowledge qualifiers shift the risk of unknown facts; define whose knowledge counts and whether investigation is required; "best of" adds nothing and may mislead; avoid "knowledge and belief" and "is unaware of".
- **Assumptions and applicability:** Sales/technology contracts (warranty), any contract with statements of fact. Author's recommended verb "states" is set out in ch 3 (outside my range).
- **Production responsibility affected:** drafting, review/redlining, issue spotting.
- **Workflow / decision implication:** Review checks: locate every performance-standard statement regardless of heading and confirm the remedy and any exclusive-remedy/disclaimer language reaches it; flag "deemed" used where no fiction is involved; for each knowledge-qualified statement, ask whose knowledge and what inquiry.
- **Evaluation evidence or criterion:** Agent identifies a product-performance statement outside the "Warranties" clause that the warranty disclaimer does not reach.
- **Failure / misuse conditions:** Replacing "warrants" in sale-of-goods documents where statutory warranty regimes attach consequences to wording, without checking.
- **Repair implication:** Conditional-clause-plus-remedy structure; defined "Knowledge".
- **Proposed disposition:** adapt.

#### AD3-23
- **ID:** AD3-23
- **Location:** ch 16, ¶16.23-16.36 "Emphasizing provisions"; ¶16.34-16.35 "Acknowledging that text is conspicuous".
- **Problem addressed:** Whole clauses set in capitals to satisfy "conspicuousness" requirements are harder to read and may not achieve the aim.
- **Principle / method / heuristic (own words):** Do not emphasise provisions unless a rule of law requires it or there is a marked imbalance of sophistication or bargaining power; emphasising one clause implicitly downgrades the rest. Where emphasis is required, bold italics or a border serve better than all capitals unless a statute prescribes capitals. A clause acknowledging that it is itself conspicuous is circular. Do not use typography for rhetorical stress on single words.
- **Assumptions and applicability:** US (UCC) context in the text; the underlying point — check whether the governing law prescribes prominence or form — transfers to consumer and online terms.
- **Production responsibility affected:** drafting, research, product consistency.
- **Workflow / decision implication:** For disclaimers, limitation clauses, jury/class waivers and consumer-facing key terms, the agent raises a research question on prominence/formatting requirements under the governing law instead of defaulting to capitals.
- **Evaluation evidence or criterion:** Agent asks whether a prominence requirement applies before choosing a format for a disclaimer.
- **Failure / misuse conditions:** Removing statutorily prescribed formatting.
- **Repair implication:** Keep required format; otherwise use readable emphasis.
- **Proposed disposition:** qualify — US-specific detail; keep the research trigger.

#### AD3-24
- **ID:** AD3-24
- **Location:** Recurring across ch 13 (e.g., ¶13.163-13.179 consequential damages; ¶13.325-13.327 fraud; ¶13.439-13.441 indemnify; ¶13.461-13.475 joint and several; ¶13.614-13.616 novation; ¶13.736-13.739 sole/exclusive; ¶13.909-13.912 workmanlike).
- **Problem addressed:** Terms of art are used as shorthand although many readers (including clients) do not know their content and courts give them varying meanings.
- **Principle / method / heuristic (own words):** Where a term of art is not needed to invoke a specific legal regime, state the underlying operative content in ordinary words (e.g., say that the claimant may recover the whole from any one obligor and sue them separately, rather than "joint and several"; say the licensor keeps the right to use the subject matter, rather than relying on "sole"). A hybrid — keep the term and add the plain statement ("in that …") — is offered where a party insists on the term. The author accepts that the plain version is longer and novel and treats that as a fair price.
- **Assumptions and applicability:** Author's programme; contestable where a term of art triggers a statutory or doctrinal consequence that paraphrase might miss.
- **Production responsibility affected:** drafting, risk communication, review/redlining, escalation.
- **Workflow / decision implication:** When an agent meets a term of art, it should be able to state the operative content it is assumed to carry; if it cannot do so with authority, that is a research/escalation trigger. In client-facing explanation, always give the plain-language content.
- **Evaluation evidence or criterion:** For each term of art retained in a draft, the agent's notes record the operative meaning relied on and its source or an open research flag.
- **Failure / misuse conditions:** Paraphrasing away a term that the governing law requires or that carries settled meaning in that market.
- **Repair implication:** Use the hybrid form (term plus explicit statement) where uncertain.
- **Proposed disposition:** adapt.

#### AD3-25
- **ID:** AD3-25
- **Location:** Introduction to appendices (pdf-pp 899-900); ch 14, ¶14.19; ch 13, ¶13.345, ¶13.441, ¶13.607, ¶13.612-13.613, ¶13.868; ch 19, ¶19.1-19.11.
- **Problem addressed:** How far to push language reform, and how drafting practice interacts with negotiation and organisational process.
- **Principle / method / heuristic (own words):** Statements the author makes about process in this range: (i) cumulative rigour across all usages yields shorter, clearer contracts, and an organisation applying it to all its contracts should see faster, cheaper contracting and fewer disputes (asserted, not evidenced here); (ii) he deliberately does not ask for every possible change — he declines to push digits-only numbering because reform capital should go to changes with greater consequences; (iii) whether an unnecessary term of art can be replaced is governed by inertia and expediency rather than meaning, and wording can be softened when a counterparty is averse to a label; (iv) late-stage markup of another party's draft justifies techniques he otherwise disfavours; (v) keeping the other side's superseded language for diplomacy is a litigation risk; (vi) a phrase that is legally redundant may still be kept if reminding the parties helps negotiation; (vii) a letter agreement should use the same categories of contract language as a formal contract, in the third person, and a formal contract should not be titled "letter of intent".
- **Assumptions and applicability:** Author's professional opinion; the efficiency claim is not supported by data in the text read.
- **Production responsibility affected:** scoping, review/redlining, evaluation, product consistency.
- **Workflow / decision implication:** Distinguish three operating contexts with different thresholds for intervention: own template (full rigour), live negotiation of own paper (targeted), counterparty paper (substance and ambiguity only; style edits suppressed). The agent should ask which context applies before reviewing.
- **Evaluation evidence or criterion:** Same defective clause presented as own template versus counterparty draft yields different recommended edits with the reason stated.
- **Failure / misuse conditions:** Applying template-grade stylistic rigour to counterparty paper; claiming quantified efficiency gains on the author's authority.
- **Repair implication:** Add a context parameter to review skills; suppress style-only comments below a materiality threshold in negotiation mode.
- **Proposed disposition:** adapt — the context-sensitivity is only lightly stated by the author and needs corroboration from other sources.

### 3. Substantive-law statements noted (research questions only)

None of the following is recorded as a finding about the law. Each is a question for jurisdiction-specific research.

1. Do courts in the relevant jurisdiction read "including" (with or without "but not limited to") restrictively, or apply ejusdem generis to such lists? (¶13.354-13.367)
2. How does the governing law classify direct, indirect/consequential, incidental and lost-profit losses, and are lost profits ever direct loss? (¶13.163-13.185)
3. Is contract damages recovery limited to reasonably foreseeable loss irrespective of any exclusion clause? (¶13.163, 13.168)
4. Does the contractual label "liquidated damages, not a penalty" carry any weight in the penalty analysis? (¶13.68-13.70)
5. Are "indemnify" and "hold harmless" treated as synonymous or distinct; does an indemnity by default cover inter-party claims; does "defend" include advancing defence costs; is an indemnity claim free of remoteness/mitigation rules that apply to damages? (¶13.416, 13.420-13.424, 13.431, 13.440)
6. Are advance releases of liability for gross negligence unenforceable; does the jurisdiction recognise degrees of negligence; what does "gross negligence" mean there? (¶13.560-13.569)
7. Does the governing law imply a duty of good faith, and can "sole discretion" or "for any reason or no reason" displace it? (¶13.297-13.298, 13.685)
8. When "satisfactory to X" is unqualified, do courts default to an objective standard? (¶13.722)
9. What is the legal effect of a "time is of the essence" clause, and does a civil-law system permit termination for trivial delay? (¶13.833-13.839)
10. Do claims and dispute-resolution clauses survive termination without an express survival clause? (¶13.775, 13.779)
11. Does "arising out of" alone exclude tort/statutory claims from a jurisdiction or arbitration clause? (¶13.42, 13.52-13.53)
12. Do statutes convert joint promises into joint and several liability; what are the procedural consequences of joint-only liability? (¶13.469-13.474)
13. Is there a rule that words prevail over figures, and is extrinsic evidence admissible to correct a mismatch? (¶14.2, 14.12)
14. Which terms must be "conspicuous" or in a prescribed format (e.g., warranty disclaimers, indemnities for own negligence, jury waivers), and do capitals satisfy that? (¶16.24-16.30)
15. Will a court disregard a "headings for convenience only" clause where the heading illuminates scope? (¶15.17)
16. Does a "provided that" clause in a licence operate as a condition of the grant or as a covenant? (¶13.665)
17. Can statements outside a "Warranties" section be treated as warranties, and can labelled warranties found a misrepresentation claim? (¶13.891-13.892)
18. Is fraud broader than intentional misrepresentation (e.g., concealment), and would a court treat the two as distinct claim types? (¶13.321-13.324)
19. Is a plaintiff normally unable to recover legal fees absent a contractual provision? (¶13.406 — stated for the US)
20. In licensing, is a "sole" licence distinct from an "exclusive" licence? (¶13.736-13.738)

### 4. Material the author marks as contested, or where the author criticises other approaches

- **"Including but not limited to":** sustained disagreement with Bryan Garner, who recommends defining "including" as non-limiting and challenges anyone to find a case where that failed; the author replies that the real risk is same-class narrowing, not exhaustive reading, so the challenge is too narrow (¶13.378-13.384).
- **"Arising out of or relating to":** rejects conventional practitioner wisdom (quoting a commercial-contracts treatise) and the wording of a major arbitral institution's model clause (¶13.42-13.43); Appendix B substitutes his own arbitration clause (note 184).
- **"Indemnify and hold harmless":** notes a split between dictionaries/courts treating the terms as synonyms and commentators/courts finding a distinction; concludes that the split is the reason to drop the doublet (¶13.420-13.427). Also notes a split of authority on whether indemnities cover inter-party claims (¶13.416).
- **Indemnification as loaded term:** says it is unclear how real the perceived advantage of indemnity claims over damages claims is (¶13.441).
- **"Joint and several":** calls the accepted phrase a "mess" despite its acceptance by a leading legal-usage dictionary (¶13.472).
- **"Force and effect":** disagrees with Garner's view that emphasis can justify the phrase in drafting; contracts do not persuade (¶13.302).
- **"To the extent permitted by law" in waivers:** disagrees with a boilerplate treatise's rationale (¶13.846).
- **Time is of the essence; liquidated damages wording:** criticises conventional formulas as jargon courts may ignore (¶13.71, 13.838).
- **Survival of representations:** acknowledges his approach differs from tradition and cites a court noting that difference (¶13.782).
- **Numbers:** disagrees with the words-and-digits convention; declines to go as far as a plain-language commentator who wants digits only; differs from a general style manual on the words/digits threshold (¶14.13, 14.17-14.19).
- **Internal rules of interpretation:** treats most standard interpretation boilerplate as unnecessary or overreaching; calls "will means shall" clauses a hopeless attempt (¶15.20); judicial canons themselves described as problematic (¶15.4).
- **M&A negotiation practice** of leaving nullified language in place for diplomacy: criticised as litigation-prone (¶13.612-13.613).
- **Termination vs expiration:** rejects the common drafter distinction as unnecessary (¶13.785).
- **Typography:** criticises all-capitals emphasis and "conspicuousness acknowledgments" (¶16.29, 16.35).
- **Mainstream drafting generally:** the appendix introduction describes conventional contract prose as murk in which structural and logical defects hide.

### 5. Content in the assigned range that is out of scope for legal production (and why)

- **Ch 16 Typography** other than emphasis/conspicuousness (fonts, justification, line spacing, characters per line, spaces after punctuation, curly quotes, first-line indents, embellishments): document design with no bearing on legal reasoning, review or risk; at most a house-style matter. Not read.
- **Pure lexical preferences in ch 13** with no effect on meaning or risk: amongst/whilst; shareholder vs stockholder; shareholders agreement apostrophe; guarantee vs guaranty spelling; no later than vs not later than; well and truly; very; allonge; joinder naming. Useful only for a house-style linter, not for legal production skills.
- **Finance/securities-specific entries** (default/event of default labels, warrant certificates, annual meeting, novation in loan amendments): specialised transactional contexts outside the project's technology/commercial/consumer focus, though the "cure vs continuing" logic was retained in AD3-11.
- **Ch 19 Letter Agreements** mechanics (salutation, address block, signature placement): format conventions; only the points that a letter agreement uses ordinary contract language and should not be mislabelled were retained (AD3-25).
- **Ch 17 Drafting as Writing** (skimmed): general prose-style guidance (sentence length, subject-verb proximity, buried verbs, gender-neutral language, wordy phrases). Relevant to a drafting-quality linter but largely covered by general plain-language sources; not extracted in detail because only skimmed.
- **pdf-pp 927-940** (works cited, table of cases, index): reference apparatus.
- **Deal terms of the appendix agreement** (US golden-parachute tax gross-up): the author disclaims them; US employment/tax specific.

### 6. Candidate benchmark cases suggested by the text (own words, synthetic)

1. **Hidden narrowing list.** A SaaS agreement defines "Customer Data" as "all data, including names, email addresses and phone numbers, uploaded by Customer". Task: review. Pass if the agent flags that the list of obvious personal-data items could be argued to narrow "all data" (e.g., excluding uploaded documents or logs) and proposes tightening the general term or using a definition, rather than only adding "without limitation".
2. **Duelling overrides.** A master agreement has a liability cap beginning "Notwithstanding anything else in this Agreement" and a data-protection indemnity beginning with the same words. Pass if the agent identifies the collision, explains each plausible reading, and recommends targeted "subject to clause X" wording.
3. **Proviso classification.** A licence grants use of software "provided that Licensee displays the attribution notice". Pass if the agent raises the condition-vs-obligation question and does not silently pick one in its redraft.
4. **NDA with stock exclusion.** A mutual NDA excludes "indirect, special or consequential loss". Pass if the agent explains that the discloser's realistic loss may fall inside the exclusion, offers alternative mechanisms, and marks loss-classification as a jurisdiction research item.
5. **Cure right mismatch.** A termination clause allows 30 days to cure "any breach", in a contract whose key obligations are confidentiality and exclusivity. Pass if the agent tests cure against those obligations and reports that cure is meaningless for them.
6. **Termination vocabulary gap.** Term clause: "This agreement expires three years after the Effective Date." Exit clause: "On termination, Supplier shall return all Customer Data." Pass if the agent flags that return may not be triggered on expiry and proposes aligned wording.
7. **Ambiguous formula.** "Service credit equals 5% of monthly fees above the Minimum Commitment less any amounts previously credited." Pass if the agent produces both groupings with sample figures and asks which is intended.
8. **Tier table.** Usage pricing tiers "0-10,000 calls: $0.010; 10,000-50,000: $0.008; 50,000+: $0.006" with no preamble. Pass if the agent flags boundary overlap and unstated marginal-vs-whole-volume application.
9. **Minimal amendment.** Instruction: "Remove clause 9 (Exclusivity) from the signed distribution agreement; SOW 2 cites clauses 10-14." Pass if the agent proposes a numbered amendment using a placeholder for clause 9 (no renumbering), lists internal and external cross-references checked, and uses present-performance amending words. Fail if it restates the whole agreement or renumbers without an impact check.
10. **Substitution vs restatement.** Instruction: extend a defined end date by two months. Pass if the agent explains the trade-off (highlighted change vs self-contained text) and chooses with a stated reason.
11. **Interpretation clause does not cure.** Body clause: "Supplier shall deliver reports to the Customer's CFO or Controller"; interpretation clause: "'or' is not exclusive". Pass if the agent still flags who may choose and whether both may be required.
12. **Context-sensitive review.** The same clause containing "hereof", "indemnify, defend and hold harmless", and an unclear notice period is supplied once as the client's own template and once as counterparty paper. Pass if the agent proposes full clean-up for the template but limits counterparty-paper comments to the notice ambiguity and indemnity scope, stating why.
13. **Logic defect under style noise.** A renewal clause provides an initial term ending 31 December of the signing year with non-renewal notice required 12 months before renewal. Pass if the agent reports that non-renewal of the first extension is impossible as drafted, and ranks this above stylistic notes.
14. **Gross negligence carve-out.** A cap excludes "gross negligence or wilful default" under a non-US governing law. Pass if the agent flags governing-law dependency, the act-vs-consequence ambiguity, the risk that deliberate non-performance becomes uncapped, and opens a research task rather than asserting a meaning.
15. **Floating reference.** Consumer terms define "Fees" as "the fees set out in our Pricing Policy as amended". Pass if the agent identifies the reference as floating and unilateral, records it as a change-impact and fairness research issue, and proposes stating which version applies.

---

