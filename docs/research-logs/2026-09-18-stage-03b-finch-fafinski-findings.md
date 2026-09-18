# Stage 3 supporting log b — per-book findings: S2 — Emily Finch and Stefan Fafinski, *Legal Skills*, 3rd ed. (OUP, 2011)

**Stage:** 3 (supporting record for `2026-09-18-stage-03-five-book-extraction.md`)  
**Date:** 18 September 2026  
**Local source identifier:** `books/Legal_Skills_-_Stefan_Fafinski.pdf` (local only; not committed)  
**Access status:** full text available  

## Method and limits

- The book text was extracted locally with `pypdf`. Nothing was uploaded to an external service.
- Reading was split into parts. One reading agent examined each part directly from the extracted text. Agents were forbidden to use the web or model memory as evidence.
- The coverage record in each part states what was read fully, skimmed or not read.
- Locations use chapter, section and print page. Print pages were confirmed against running heads in the text.
- Findings are expressed independently. Short phrases only are quoted.
- Dispositions here are **proposed** by the reader of each part. The accepted dispositions are in the main Stage 3 log.
- Statements of substantive law are recorded as research questions only. They are not authority for any live matter.
- Spot-checks of findings against the book text are recorded in the main Stage 3 log.

---

## Part 1 — Introduction, chapters 1–6 (IDs FF1-)

Assigned range: pdf-pages 23-192 (Introduction; Part I Section A chs 1-3; Section B chs 4-6).
Page mapping confirmed against running heads in the text: print page = pdf-page minus 22 (e.g. pdf 33 carries "10 LEGISLATION"; pdf 99 carries "76 USING LEGISLATION"; pdf 176 carries "153 JUDICIAL PRECEDENT"). All page references below are PRINT pages.

Jurisdiction and date caveat: England and Wales student text, c. 2010. Database names, the EU-law layer (pre-Brexit, European Communities Act 1972 treated as operative), court details and the Human Rights Act case law are perishable. Findings target the METHOD. Every statement of what the law is has been moved to section 3.

### 1. Coverage record

| pdf-page range | chapter / section | status | note |
|---|---|---|---|
| 23-31 | Introduction; Part I and Section A openers | read fully | Mostly orientation; nothing material beyond stated aim (find, understand, use law). |
| 32-41 | ch 1 §1.1 Domestic legislation (statute types, law-making process, commencement, extent, HRA s19, delegated legislation) | read fully | |
| 42-56 | ch 1 §1.2 European legislation, ECHR, summary | read fully | Read quickly; almost entirely substantive/institutional and 2010-era. |
| 58-79 | ch 2 §2.1 Finding domestic legislation (statutes and SIs, library and online) | read fully for method | Reproduced extracts from citators/Halsbury's (each printed twice in the extraction) were skimmed, not studied line by line. Screenshot click-paths skipped as instructed. |
| 80-86 | ch 2 §2.2-2.3 Finding EU legislation and ECHR; summary | read fully | |
| 88-112 | ch 3 Using legislation (anatomy of Act, anatomy of SI, statutory interpretation, ECA 1972, HRA 1998) | read fully | Priority chapter. |
| 114-116 | Section B opener; ch 4 introduction | read fully | |
| 117-120 (first part) | ch 4 §4.1.1 brief legal history | NOT read | Skipped (about 150 text lines); historical narrative. |
| 120-134 | ch 4 §4.1.2-4.4 common law, equity, custom, courts and jurisdictions, tribunals, ECtHR, summary | read fully | More than half of ch 4 read. |
| 136-162 | ch 5 Finding cases (citations, reported/unreported, summaries, citators, Law Reports Index, The Digest, databases, EU and ECtHR cases) | read fully for method | Duplicate extract blocks and database blurbs skimmed. |
| 164-190 | ch 6 Using cases (anatomy of a report, EU reports, precedent, hierarchy, binding/persuasive, ratio/obiter, operation by court, HRA, EU, avoiding precedents, summary) | read fully | Priority chapter. |
| 191-192 | blank; Section C opener | read | No content. |

Coverage gap relative to the assignment focus: the assigned range does NOT contain an explicit ranked "hierarchy of law reports". The only statement found is that the series published by the Incorporated Council of Law Reporting is the most authoritative (ch 5 §5.1.1.2, p. 115), plus an unanswered self-test question asking which report should be cited in court (p. 120). No further ranking was found by reading or by keyword search of the range.

### 2. Material findings

#### FF1-01
- **ID:** FF1-01
- **Location:** ch 1, §1.1.2.1 Statutory instruments, p. 16; §1.1.2.6 Advantages and disadvantages of delegated legislation, p. 18
- **Problem addressed:** Researchers stop at the Act and miss the subordinate layer where most operative detail and most change sits.
- **Principle / method / heuristic (own words):** Treat an Act as a frame and assume the operative detail, the commencement dates, penalty levels and even amendments to the Act itself may sit in instruments made under it. The book reports a ratio of dozens of Acts to thousands of instruments in one year and draws the explicit conclusion that any research must be checked for currency because of that volume.
- **Assumptions and applicability:** UK legislative model (Act plus instruments made by ministers, plus by-laws, court rules, Orders in Council). The general shape (parent/child legislation) transfers to other systems; the specific instrument types do not.
- **Production responsibility affected:** research; authority verification; change impact
- **Workflow / decision implication:** For every Act relied on, run a second pass: what instruments have been made under each relevant enabling section, and what instruments have amended the Act.
- **Evaluation evidence or criterion:** Output that cites an Act lists (or records a nil search for) subordinate legislation made under the sections relied on.
- **Failure / misuse conditions:** Stating a rule from the Act text when the threshold, date or penalty has been reset by instrument.
- **Repair implication:** Add the missing subordinate-legislation search; re-date the conclusion.
- **Proposed disposition:** retain — cheap, high-yield completeness check.

#### FF1-02
- **ID:** FF1-02
- **Location:** ch 1, §1.1.1.6 The domestic law-making process (Royal Assent), p. 15; ch 3, §3.1.4 Date of Royal Assent, pp. 68-69; ch 3, §3.1.7 Commencement, p. 71
- **Problem addressed:** Assuming that an enacted provision is operative law.
- **Principle / method / heuristic (own words):** Enactment and commencement are separate questions. Identify which of the commencement modes applies to each provision: default on assent, a date fixed in the Act, a date relative to assent, or a date appointed later by order. Expect staggered commencement across provisions, commencement limited to certain geographic areas, commencement "for limited purposes only" (e.g. only to allow regulations to be made — visible in the SI example at p. 74), and provisions that are never commenced at all. The year in an Act's short title is not evidence of its in-force date. Presume no retrospective effect unless the Act expressly says so.
- **Assumptions and applicability:** UK Acts; commencement provisions usually sit near the end of the Act. Default rules stated in the book are substantive law (see section 3).
- **Production responsibility affected:** authority verification; reasoning/applicability; change impact
- **Workflow / decision implication:** An agent must record, per provision relied on, (a) commencement mode, (b) date, (c) the commencing instrument, (d) any area or purpose limitation, before applying it to facts with a date.
- **Evaluation evidence or criterion:** Each statutory provision in an output carries an in-force status with source; none is dated from the short-title year.
- **Failure / misuse conditions:** Applying an uncommenced, partially commenced or area-limited provision; applying a provision to facts that pre-date commencement.
- **Repair implication:** Re-run the analysis with the provision treated as not in force for the relevant date/area and flag the change in conclusion.
- **Proposed disposition:** retain — core verification step.

#### FF1-03
- **ID:** FF1-03
- **Location:** ch 1, §1.1.1.6 (Territorial extent), p. 15
- **Problem addressed:** Applying a statute outside the part of the UK to which it extends.
- **Principle / method / heuristic (own words):** Look for the extent provision (normally among the final sections) and for jurisdiction markers in the short title; consider whether the subject is devolved, in which case a different legislature's law may govern.
- **Assumptions and applicability:** UK multi-jurisdiction structure; the presumption and convention stated are substantive (section 3). The habit (check territorial reach before applying) is general.
- **Production responsibility affected:** scoping; reasoning/applicability; escalation
- **Workflow / decision implication:** Matter intake must fix the governing territory; every statute used is checked against it.
- **Evaluation evidence or criterion:** Output states the territorial extent of each statute relied on and matches it to the matter's territory.
- **Failure / misuse conditions:** English-law answer given for a Scottish or Northern Irish matter; devolved-subject legislation overlooked.
- **Repair implication:** Re-scope; escalate to a lawyer qualified in the correct jurisdiction.
- **Proposed disposition:** retain — scoping gate.

#### FF1-04
- **ID:** FF1-04
- **Location:** ch 2, §2.1.1.1 In a library ("Is it in force?"), pp. 46-47
- **Problem addressed:** In-force status is checked at the wrong granularity.
- **Principle / method / heuristic (own words):** Status is recorded per section and sometimes per subsection: within one section, some subsections may be in force and others not, and a provision may be in force yet disapplied for a transitional period. Two complementary checks are shown: a positive table (date and commencing instrument per provision) and a negative table (provisions not yet in force). Both must then be brought up to date with the most recent updating service. For statutes older than the status tool's coverage, a different (historical) table is needed.
- **Assumptions and applicability:** The named print tools are perishable; the granularity and the two-sided check are not.
- **Production responsibility affected:** authority verification
- **Workflow / decision implication:** Verification queries must be keyed to the exact subsection/paragraph relied on, not to the Act or section.
- **Evaluation evidence or criterion:** Status evidence cites the same pinpoint as the proposition it supports.
- **Failure / misuse conditions:** "The Act is in force" used to support reliance on an uncommenced subsection.
- **Repair implication:** Re-verify at pinpoint level; downgrade the confidence of the affected proposition.
- **Proposed disposition:** retain — directly testable.

#### FF1-05
- **ID:** FF1-05
- **Location:** ch 2, §2.1.1.1 (Halsbury's Statutes; Figure 2.1), pp. 42-43, 45, 50; (Chronological Table) p. 38; §2.1.2.1 (Halsbury's Statutory Instruments) p. 55; ch 5, §5.2.1.1 (Current Law Case Citator) p. 119
- **Problem addressed:** Every source is frozen at a publication date; researchers treat it as current.
- **Principle / method / heuristic (own words):** Work in a fixed order from the base text to successive updating layers (main work, then annual cumulative supplement, then the most recent loose-leaf or monthly service) and do not skip a layer. Know each source's lag (one table is said to run two to three years behind). For cases, search citator volumes chronologically from oldest to the latest monthly part so that nothing falls between volumes.
- **Assumptions and applicability:** Print-era procedure; the transferable method is "establish the currency date of each source and close the gap to today with a more recent source".
- **Production responsibility affected:** research; authority verification; change impact
- **Workflow / decision implication:** Agent records a "current to" date for each source consulted and performs an explicit gap check from that date to the date of the work.
- **Evaluation evidence or criterion:** Research log shows source currency dates and a gap-closing step; fails if any authority has no currency date.
- **Failure / misuse conditions:** Relying on a consolidated text or a model's training data without a later-change check.
- **Repair implication:** Run the gap check; mark conclusions provisional until done.
- **Proposed disposition:** adapt — replace print layers with database currency stamps, keep the discipline.

#### FF1-06
- **ID:** FF1-06
- **Location:** ch 2, §2.1.1.1 (Current Law Legislation Citator; Table 2.2 Legislative effects), pp. 39-40; §2.1.2.1 (Statutory Instrument Citator) pp. 55-56
- **Problem addressed:** "Amended or repealed?" is too coarse a question.
- **Principle / method / heuristic (own words):** Later legislation can affect a provision in at least ten distinct ways: added to, amended, applied, consolidated, disapplied, used as an enabling power, merely referred to, repealed, restored after repeal, substituted wholesale, or varied. Two are traps: "varied" means the words stay the same but their application to particular circumstances changes, and "disapplied" means an exception has been carved out. A citator also records judicial consideration of a provision and the instruments made under it. The same apparatus exists for statutory instruments.
- **Assumptions and applicability:** Terminology is that of one UK citator; other tools use different labels but the categories recur.
- **Production responsibility affected:** authority verification; change impact; reasoning/applicability
- **Workflow / decision implication:** Status check returns a typed effect list, not a boolean. "Varied"/"disapplied"/"applied" entries trigger reading the affecting provision even though the text of the target is unchanged.
- **Evaluation evidence or criterion:** Given a provision whose text is unchanged but has been varied for a class of case, the agent detects the variation.
- **Failure / misuse conditions:** Concluding "unamended, therefore applies as written"; missing a restoration after repeal.
- **Repair implication:** Re-run status check with typed effects; re-read affecting provisions.
- **Proposed disposition:** retain — strong candidate for a verification schema.

#### FF1-07
- **ID:** FF1-07
- **Location:** ch 2, §2.1.1.1 (Public General Acts extract; Halsbury's main-volume extract and notes), pp. 36, 49-50; §2.1.1.2 Online (legislation.gov.uk, BAILII), pp. 50-51
- **Problem addressed:** Confusing the amending text with the law as amended, and "as enacted" text with current text.
- **Principle / method / heuristic (own words):** Many sections are only editing instructions directed at an earlier Act; they tell you nothing usable until applied to the target text. Read the target provision in a consolidated version in which inserted or substituted words are visibly marked (square brackets) and each mark is traced in notes to the amending provision. Know whether a given source holds legislation as originally enacted or in revised form; the book notes one free source holds "as enacted" text while the official site holds mostly revised text.
- **Assumptions and applicability:** UK textual-amendment drafting style. Which sites hold which version is perishable.
- **Production responsibility affected:** research; authority verification; drafting; review/redlining
- **Workflow / decision implication:** Agent labels every quoted statutory text with version type (as enacted / revised to date X) and keeps the amendment provenance.
- **Evaluation evidence or criterion:** Quoted provision matches the revised text for the relevant date; provenance of each amendment can be stated.
- **Failure / misuse conditions:** Quoting the as-enacted text of a heavily amended section; citing the amending Act as if it were the operative rule.
- **Repair implication:** Replace with revised text; re-check reasoning that depended on superseded wording.
- **Proposed disposition:** retain.

#### FF1-08
- **ID:** FF1-08
- **Location:** ch 2, §2.1.1.2 Online (Westlaw point-in-time facility), p. 52; ch 2 end-of-chapter self-test question 5, p. 61; ch 2 (Chronological Table for legislative history), p. 38
- **Problem addressed:** The law that governs a past event is the law at that date, not today's.
- **Principle / method / heuristic (own words):** The book treats "what was the wording of this section on a given past date" as a standard research task and points to point-in-time search and historical tables for tracing earlier states of legislation.
- **Assumptions and applicability:** Availability of historical versions depends on the tool and date range (perishable).
- **Production responsibility affected:** scoping; research; reasoning/applicability
- **Workflow / decision implication:** Intake fixes the legally relevant date(s); research is run "as at" each date; differences between then and now are reported.
- **Evaluation evidence or criterion:** For a fact pattern dated before an amendment, the agent applies the pre-amendment text and says so.
- **Failure / misuse conditions:** Applying current text to historic facts, or historic text to a forward-looking advice.
- **Repair implication:** Re-run with correct date; show both versions where transitional issues arise.
- **Proposed disposition:** retain.

#### FF1-09
- **ID:** FF1-09
- **Location:** ch 2, §2.1.1.2 Online, p. 50 (paraphrased statute text on non-official sites); ch 2, §2.1.1.1 (Current Law Statutes Annotated), p. 41; ch 3, §3.1.10 Explanatory Notes, p. 73 and §3.2.8, p. 75; ch 5, §5.1.3 Case summaries, p. 118; ch 5 (Current Law Yearbook digest is not a law report), p. 121; ch 6, §6.1.9 Headnote, p. 145
- **Problem addressed:** Derivative texts are mistaken for the authority.
- **Principle / method / heuristic (own words):** Paraphrases of statutes on firm or council sites, editorial annotations, government explanatory notes, case digests and reporters' headnotes are finding aids and context, not law. The headnote is written by the reporter, not the judge, and the book demonstrates a headnote that dropped a limiting word ("subsequent") found in the judgment. Rule: use the official wording of legislation; if relying on a summary of a case, go to the full judgment and read it all.
- **Assumptions and applicability:** General. Explanatory notes and annotations retain value for purpose and legislative history (see FF1-17).
- **Production responsibility affected:** research; authority verification; evaluation
- **Workflow / decision implication:** Agent tags each source by type (primary text / editorial / official explanatory / digest) and may not support a proposition of law solely from a non-primary tag.
- **Evaluation evidence or criterion:** Every legal proposition traces to a primary text pinpoint; a planted headnote/judgment discrepancy is caught.
- **Failure / misuse conditions:** Quoting a headnote or digest as the holding; relying on a plain-English paraphrase of a statute.
- **Repair implication:** Pull primary text; correct the proposition; record the discrepancy.
- **Proposed disposition:** retain — central to authority verification; also applies to AI-generated summaries.

#### FF1-10
- **ID:** FF1-10
- **Location:** ch 3, §3.1 Anatomy of an Act of Parliament, §§3.1.1-3.1.9, pp. 65-73
- **Problem addressed:** Reading a section in isolation from the machinery of the Act.
- **Principle / method / heuristic (own words):** An Act has standard parts with standard jobs: short title (the name to use), year-and-chapter citation (unique identifier; older Acts use regnal-year citation), long title (purpose and scope), assent date, enacting words, body (sections, subsections, paragraphs, subparagraphs), interpretation provisions, commencement and similar machinery near the end, and schedules. Schedules hold definitions, detail referred to from the body, consequential amendments to other Acts, and repeals; their divisions are paragraphs, not sections. Pinpoint to the smallest unit that contains the words relied on. Older Acts may have a preamble setting out purposes.
- **Assumptions and applicability:** UK Acts; structure differs for other jurisdictions and for EU instruments.
- **Production responsibility affected:** research; reasoning/applicability; drafting; review/redlining
- **Workflow / decision implication:** Fixed reading order for any Act: long title, interpretation section(s), target provision, cross-referred provisions and schedules, then commencement/extent/transitional machinery, then repeals and consequential amendments schedule (for change impact).
- **Evaluation evidence or criterion:** Pinpoints resolve to the correct unit type; defined terms used in the target provision have been looked up; schedules checked.
- **Failure / misuse conditions:** Missing a statutory definition; citing a schedule paragraph as a "section"; ignoring the repeals schedule when assessing impact on other legislation.
- **Repair implication:** Re-read using the full order; correct pinpoints.
- **Proposed disposition:** retain.

#### FF1-11
- **ID:** FF1-11
- **Location:** ch 3, §3.1.6.1 Headings, p. 70; §3.1.9 Preambles, pp. 72-73; §3.3.1.8 Intrinsic aids to interpretation, p. 83
- **Problem addressed:** Not all text printed with an Act has the same status.
- **Principle / method / heuristic (own words):** Start from the principle that the whole Act is read before looking outside it. Then weight each internal component: definitions and examples within the Act are part of it and carry great weight; long title and preamble help only where the body is ambiguous; short title is descriptive; headings are part of the Act while marginal notes are not, and both are mainly navigation; punctuation can help in ambiguity.
- **Assumptions and applicability:** Weights stated are the book's 2010 account of English practice (section 3 for verification).
- **Production responsibility affected:** reasoning/applicability; risk communication
- **Workflow / decision implication:** When an interpretive argument rests on a component, the agent states the component's status and whether an ambiguity threshold has been met.
- **Evaluation evidence or criterion:** No argument presents a heading, side-note or explanatory note as if it were operative text.
- **Failure / misuse conditions:** Over-reading a heading to cut down clear operative words.
- **Repair implication:** Re-ground the argument in operative text; demote the aid to supporting role.
- **Proposed disposition:** qualify — method sound, weights need current verification.

#### FF1-12
- **ID:** FF1-12
- **Location:** ch 3, §3.2 Anatomy of a statutory instrument, §§3.2.1-3.2.8, pp. 73-75; ch 1, §1.1.2.5 Validity of delegated legislation, pp. 17-18
- **Problem addressed:** Reading and validating subordinate legislation.
- **Principle / method / heuristic (own words):** An instrument declares its year-and-number citation, subject heading (including territorial application), title (which names the parent Act and function, e.g. a numbered commencement order), the date made (or laid), any separate coming-into-force date, the enabling power recited, the body (articles for orders, regulations, or rules), the signatory, and an explanatory note that is not part of the instrument. Because subordinate legislation, unlike an Act, can be attacked for exceeding its enabling power, the recited power is the starting point for a validity check.
- **Assumptions and applicability:** UK SIs. Note an apparent error in the book: it says the bracketed "C" number is the parent Act's chapter number, but the reproduced instrument's own footnote gives a different chapter number for the parent Act (p. 74). Treat that statement as unreliable.
- **Production responsibility affected:** research; authority verification; reasoning/applicability; escalation
- **Workflow / decision implication:** For each SI relied on: capture made / laid / in-force dates separately; read the enabling section in the parent Act and check the SI's subject falls within it; check whether the parent power itself is in force and unamended.
- **Evaluation evidence or criterion:** SI record contains enabling provision, three dates, territorial heading; the enabling provision has itself been status-checked.
- **Failure / misuse conditions:** Using the "made" date as the in-force date; relying on an SI whose enabling power has been repealed without checking savings.
- **Repair implication:** Complete the record; escalate possible vires doubts rather than resolving them.
- **Proposed disposition:** retain, with the C-number point marked research further.

#### FF1-13
- **ID:** FF1-13
- **Location:** ch 3, §3.3 Statutory interpretation and §3.3.1 How to interpret a statutory provision, pp. 75-76; §§3.3.1.1-3.3.1.4, pp. 76-79
- **Problem addressed:** Treating the traditional "rules" of interpretation as an algorithm.
- **Principle / method / heuristic (own words):** The literal, golden and mischief approaches and the purposive approach are descriptions of judicial technique, not binding rules; a judge need not follow or even name one. The practical use is adversarial: for any ambiguous provision, generate the reading each approach yields, identify which readings help and which hurt, and anticipate the opponent's. The mischief approach supplies a usable question set (prior law; the defect; the remedy chosen; the reason for it). The book reports purposive reading as now predominant, with the degree of latitude varying by subject matter. Interpretation is only engaged where wording is unclear; ordinary meaning is a question of fact, legal meaning a question of law.
- **Assumptions and applicability:** English courts c. 2010. Relative dominance of approaches is a substantive claim needing verification.
- **Production responsibility affected:** issue spotting; reasoning/applicability; risk communication
- **Workflow / decision implication:** Agent produces a structured "competing readings" table (literal / absurdity-avoiding / purpose-based), not a single confident reading, and reports interpretive risk where readings diverge.
- **Evaluation evidence or criterion:** For an ambiguous provision the output shows at least two candidate readings with the supporting approach and an assessment of which a court is more likely to adopt.
- **Failure / misuse conditions:** Announcing "under the literal rule the answer is X" as if determinative; inventing ambiguity where the text is clear.
- **Repair implication:** Add the omitted readings; convert certainty language to risk language.
- **Proposed disposition:** adapt — keep the multi-reading discipline, drop the rule labels as decisive.

#### FF1-14
- **ID:** FF1-14
- **Location:** ch 3, §3.3.1.5 The teleological approach, pp. 79-80; §3.3.2 Interpretation and the European Communities Act 1972, p. 85; §3.3.3 Interpretation and the Human Rights Act 1998, pp. 85-87
- **Problem addressed:** Domestic text that implements or is constrained by a higher-order instrument cannot be read by domestic technique alone.
- **Principle / method / heuristic (own words):** Before interpreting, ask where the provision comes from. If it implements a supranational instrument, courts read it to achieve that instrument's aim, even to the point of reading words in. If rights-compatibility is in play, a separate statutory interpretive duty applies that does not depend on finding ambiguity and is bounded only by what is "possible". The book ranks the two duties by strength and shows judges disagreeing about where interpretation ends and legislating begins.
- **Assumptions and applicability:** HEAVILY perishable: written with EU law supreme in the UK. The transferable method is "identify the provenance and any overriding interpretive obligation of each provision".
- **Production responsibility affected:** issue spotting; reasoning/applicability; escalation
- **Workflow / decision implication:** Provenance check (purely domestic / implements international or EU-origin instrument / rights-sensitive) is a mandatory field; non-domestic provenance routes to specialist review.
- **Evaluation evidence or criterion:** Output identifies the source instrument for implementing legislation and states the current interpretive regime with a verified authority.
- **Failure / misuse conditions:** Applying the book's ECA 1972 analysis as current law; reading implementing regulations literally against the purpose of the parent instrument.
- **Repair implication:** Re-research the current status of retained/assimilated EU-origin law and rights-based interpretation; escalate.
- **Proposed disposition:** research further — method retained, substance must be rebuilt from current sources.

#### FF1-15
- **ID:** FF1-15
- **Location:** ch 3, §3.3.1.6 Rules of language, pp. 80-81; §3.3.1.7 Presumptions, p. 82
- **Problem addressed:** Lists, general words and silence in statutes (and by extension in drafted documents) create predictable interpretive disputes.
- **Principle / method / heuristic (own words):** Three linguistic canons: general words after a specific list are confined to the list's type; a word takes colour from its neighbours; naming some items implies exclusion of others. A set of presumptions is read into legislation unless clearly displaced: no implied change to common law, no retrospectivity, no deprivation of liberty or property without clear words, Crown not bound, courts' jurisdiction not ousted, criminal liability requires a mental element.
- **Assumptions and applicability:** English statutory interpretation; the book does not apply these to contracts, so extension to drafting review is this extractor's inference, not the authors'.
- **Production responsibility affected:** issue spotting; reasoning/applicability; drafting; review/redlining
- **Workflow / decision implication:** Use as a checklist when reading any list-plus-general-words provision and when a reading would produce one of the presumed-against results (flag that clear words are needed).
- **Evaluation evidence or criterion:** Given a provision with a specific list plus "or other", the agent raises the class-limitation issue and identifies the common characteristic of the list.
- **Failure / misuse conditions:** Treating canons as conclusive; applying them where the statute defines the term.
- **Repair implication:** Re-state as rebuttable aids; check statutory definitions first.
- **Proposed disposition:** retain as issue-spotting checklist; qualify as non-conclusive.

#### FF1-16
- **ID:** FF1-16
- **Location:** ch 3, §3.3.1.9 Extrinsic aids to interpretation, pp. 83-85; ch 2 (annotated statutes giving Hansard references), p. 41; ch 3 §3.1.10, p. 73
- **Problem addressed:** Over-use of legislative history and other outside material.
- **Principle / method / heuristic (own words):** Outside aids have an order and gates: a general interpretation statute supplies default definitions; dictionaries serve where a word has no legal meaning; the same words in earlier or related Acts may be considered; official reports that preceded the Act may show the defect addressed. Parliamentary debate is admissible only when three conditions are all met (unclear or absurd text; a statement by the minister or promoter; the statement itself clear). The authors flag as a common error the claim that debates can always be consulted, and note courts are in practice reluctant.
- **Assumptions and applicability:** English law; conditions are substantive (section 3).
- **Production responsibility affected:** research; reasoning/applicability; risk communication
- **Workflow / decision implication:** Agent must state the gate before citing legislative history and label it as supporting material only.
- **Evaluation evidence or criterion:** Any use of debates is accompanied by an explicit statement that each gating condition is met; otherwise it is presented as background.
- **Failure / misuse conditions:** Using a backbencher's remark or an explanatory note to contradict clear text.
- **Repair implication:** Remove or demote the material; re-base the argument on text and purpose.
- **Proposed disposition:** retain, qualify pending current law on the gates.

#### FF1-17
- **ID:** FF1-17
- **Location:** ch 5, §5.1.1 Making sense of case citations, §5.1.1.1 Neutral citation, §5.1.1.2 Law report citations, pp. 114-116; §5.1.2 Reported and unreported cases, p. 116; §5.2.1.1, p. 119
- **Problem addressed:** Citations are copied rather than read; they carry verification data.
- **Principle / method / heuristic (own words):** A neutral citation encodes year of judgment, court (and therefore level of authority) and judgment number, is medium-independent, and comes first; a report citation encodes year of the report, volume, series and first page. The report year can differ from the judgment year. Bracket shape around the year is meaningful (it signals whether the year is needed to find the volume) and must be reproduced exactly. Where there is no neutral citation, add a court abbreviation. Most judgments are never reported; unreported transcripts exist. The series from the semi-official reporting body is described as the most authoritative. If a citation fails to resolve, suspect a misprint or a misread abbreviation and look for a parallel citation.
- **Assumptions and applicability:** England and Wales conventions; no full ranking of report series is given in this range.
- **Production responsibility affected:** authority verification; drafting; evaluation
- **Workflow / decision implication:** Parse every case citation into fields; derive the court from it; cross-check court and year against the judgment itself; prefer the most authoritative report available and keep the neutral citation.
- **Evaluation evidence or criterion:** Citation parses; court derived from citation matches the judgment; a fabricated or mis-yeared citation fails resolution and is flagged rather than silently "fixed".
- **Failure / misuse conditions:** Hallucinated or transposed citations; treating report year as decision year when sequencing authorities.
- **Repair implication:** Resolve via parallel citations in a citator; if unresolvable, remove the authority.
- **Proposed disposition:** retain; research further on ranking of report series (not covered here).

#### FF1-18
- **ID:** FF1-18
- **Location:** ch 5, §5.2.1.1 (Current Law Case Citator; Law Reports Index "cases judicially considered"; The Digest annotations and Table of annotations), pp. 119-126; ch 6, §6.1.9 Table 6.2 Headnote terminology, pp. 145-146
- **Problem addressed:** A case is cited without knowing what happened to it afterwards.
- **Principle / method / heuristic (own words):** For every case, establish (a) its own appellate history and (b) its treatment in later, different cases. The vocabulary is graded: within the same litigation a decision is affirmed or reversed; across cases it may be applied, followed, approved, considered, explained, extended, distinguished, doubted, disapproved, not followed or overruled. The worked example shows one precedent applied by an intermediate court and then departed from by the top court in the same later litigation, so a single "applied" entry is not the end of the inquiry. Dicta of a particular judge can be separately tracked.
- **Assumptions and applicability:** Print citators named are perishable; the treatment vocabulary and two-axis check are durable in common-law systems.
- **Production responsibility affected:** authority verification; reasoning/applicability; risk communication; change impact
- **Workflow / decision implication:** Noting-up is mandatory before reliance; results are stored as typed treatment events with court and date; negative treatment by an equal or higher court blocks or qualifies reliance.
- **Evaluation evidence or criterion:** Given an overruled or reversed case, the agent refuses to rely on it for the overruled point and says why; given a distinguished case, it reports the limit.
- **Failure / misuse conditions:** Citing a first-instance or intermediate decision that was reversed on appeal; reading "considered" as endorsement.
- **Repair implication:** Replace with the surviving authority; re-assess the proposition's strength.
- **Proposed disposition:** retain — core of the authority-verification skill.

#### FF1-19
- **ID:** FF1-19
- **Location:** ch 5, §5.2.2.1 Which database? and §5.2.2.2-5.2.2.3, pp. 127-128; ch 6, §6.1.15 Electronic reports, pp. 147-148
- **Problem addressed:** Assuming one database is complete and that every version of a judgment is equivalent.
- **Principle / method / heuristic (own words):** No single service carries every report series; pair broad services. Versions differ: one electronic version of the example case lacked the headnote, the lists of cases and the procedural history, and showed different catchwords and different parallel citations; paragraph numbers may be missing; page breaks of the print report appear as inline markers that must be read backwards to find the page for a pinpoint. Search strategy: start simple with a distinctive party name; add subject keywords only when the name is common.
- **Assumptions and applicability:** Specific coverage tables are perishable.
- **Production responsibility affected:** research; authority verification
- **Workflow / decision implication:** A nil result in one source is not evidence of absence; record which sources were searched; record which version a pinpoint comes from.
- **Evaluation evidence or criterion:** Research log names sources searched; pinpoints state paragraph or page scheme and version.
- **Failure / misuse conditions:** "No authority exists" after a single-source search; pinpoints that do not match the cited report.
- **Repair implication:** Widen sources; re-derive pinpoints.
- **Proposed disposition:** adapt.

#### FF1-20
- **ID:** FF1-20
- **Location:** ch 6, §6.1 Reading UK cases, §§6.1.2-6.1.14, pp. 143-147
- **Problem addressed:** Extracting the wrong things from a law report.
- **Principle / method / heuristic (own words):** Read a report by parts, each with a use: case-name form signals type of proceeding (Crown prosecutions, judicial review naming conventions that changed over time, anonymised family matters, "in the matter of", ship names); court fixes precedential weight; hearing and judgment dates (reserved judgments are dated later); the bench — seniority and standing affect persuasive weight where the decision is not binding; catchwords and headnote are editorial; the list separating cases the judges actually referred to from cases merely cited by counsel (the former matter more); procedural history; then the judgments, typically material facts, applicable law, reasoning, disposal. In multi-judge courts each judge may give reasons, concur shortly or dissent. Pinpoint by paragraph number or marginal letter.
- **Assumptions and applicability:** English reports; EU court reports differ (single collegiate judgment, no dissents, separate non-binding Advocate General opinion, less speculation beyond the facts) — ch 6 §6.2, pp. 148-150.
- **Production responsibility affected:** research; reasoning/applicability; authority verification
- **Workflow / decision implication:** Case-brief template should capture: court, bench, dates, procedural posture, material facts, issue, rule, reasoning, disposal, per-judge alignment (majority/concurring/dissenting), cases relied on by the court.
- **Evaluation evidence or criterion:** Brief distinguishes majority reasoning from dissent and editorial matter from judicial text.
- **Failure / misuse conditions:** Quoting a dissent or counsel's argument as the court's holding.
- **Repair implication:** Re-brief with per-judge attribution.
- **Proposed disposition:** retain.

#### FF1-21
- **ID:** FF1-21
- **Location:** ch 6, §6.3.1 Precedent and the hierarchy of the courts, pp. 151-153; §6.3.2 Binding and persuasive precedents and Table 6.3, pp. 153-154
- **Problem addressed:** Deciding how much an earlier case constrains the present question.
- **Principle / method / heuristic (own words):** A precedent binds only when three conditions hold together: the material facts are sufficiently analogous; the earlier court is above or (normally) level with the deciding court; and the proposition relied on was part of the earlier court's necessary reasoning. Failing any one makes it at most persuasive. Persuasive categories listed: similar but not analogous facts; reasoning of a lower court; passing remarks of a higher or equal court; dissents; decisions from outside the jurisdiction, including the Privy Council. A Court of Appeal case is assessed in three directions — up, down and sideways. Being the ratio does not by itself make something binding, and being obiter does not make it worthless: it depends on the relationship between the two courts.
- **Assumptions and applicability:** English doctrine of precedent; hierarchy details are substantive and dated (section 3).
- **Production responsibility affected:** reasoning/applicability; authority verification; risk communication
- **Workflow / decision implication:** Each case authority gets a weight label computed from the three-part test relative to the forum that would decide the matter (so the forum must be identified first).
- **Evaluation evidence or criterion:** Output labels each authority binding/persuasive with the reason (which limb fails); labels change correctly when the hypothetical forum changes.
- **Failure / misuse conditions:** Calling a foreign, dissenting or obiter statement "binding"; ignoring forum.
- **Repair implication:** Recompute labels; soften conclusions resting on persuasive authority.
- **Proposed disposition:** retain.

#### FF1-22
- **ID:** FF1-22
- **Location:** ch 6, §6.3.3 Finding the ratio decidendi and obiter dicta, pp. 154-156
- **Problem addressed:** Identifying what a case actually decides.
- **Principle / method / heuristic (own words):** Judges do not label their ratio and there is no mechanical rule. Method: (1) isolate material facts using a "so what?" test — would changing this fact have changed the reasoning and result? (2) state the rule of law treated, expressly or impliedly, as a necessary step to the conclusion; (3) mark as obiter anything wider than needed, hypotheticals on different facts, what the judge would have decided but for binding authority, and everything in a dissent. (4) Recognise that a ratio can be framed at several levels of generality — the worked example gives four, from fact-bound to very broad — and that the level which prevails is settled by later courts, not by the original judgment. A statement may begin as obiter and acquire binding force through later adoption.
- **Assumptions and applicability:** Common-law reasoning generally.
- **Production responsibility affected:** reasoning/applicability; issue spotting; risk communication
- **Workflow / decision implication:** Agent drafts narrow, middle and broad formulations of the ratio, then checks later cases to see which formulation courts have actually applied, and reports the residual uncertainty.
- **Evaluation evidence or criterion:** Ratio statement is supported by later-case usage, not only by the original judgment; immaterial facts are not embedded in the rule.
- **Failure / misuse conditions:** Over-broad ratio used to cover the client's facts; over-narrow ratio used to dismiss an adverse case without checking later treatment.
- **Repair implication:** Re-frame using later authority; present alternative formulations as risk.
- **Proposed disposition:** retain — directly supports applicability analysis.

#### FF1-23
- **ID:** FF1-23
- **Location:** ch 6, §6.6 Avoiding difficult precedents, pp. 165-166; §6.3.4.2 The Supreme Court, pp. 157-159; §6.3.4.3 The Court of Appeal, pp. 159-160; §6.4 Precedent and the Human Rights Act 1998, pp. 162-164
- **Problem addressed:** What to do with an adverse authority.
- **Principle / method / heuristic (own words):** First decide the aim: side-step the case while leaving it standing, or remove its authority. Available techniques, in roughly ascending ambition: (a) distinguish on material facts or on the point of law; (b) argue for a narrow (or, where helpful, wide) reading of its ratio; (c) argue it has no discernible single ratio (split reasoning, heavy obiter, dissent); (d) show it conflicts with another decision of the same court, forcing a choice; (e) show it cannot stand with a later decision of a higher court even though not expressly overruled; (f) show it was decided in ignorance of a binding statute or authority that would inevitably have changed the result — a demanding standard; (g) invoke greater flexibility where liberty is at stake in criminal appeals; (h) argue incompatibility with rights jurisprudence; (i) at the top court, ask for departure, which requires express notice and more than showing the earlier case was wrong, with heightened caution for settled commercial, property, fiscal and criminal expectations; (j) overruling by a higher court, which is distinguished from reversing on appeal in the same case.
- **Assumptions and applicability:** England and Wales; several limbs are substantive and need current verification. Technique (a)-(c) are general common-law method.
- **Production responsibility affected:** reasoning/applicability; risk communication; escalation
- **Workflow / decision implication:** Adverse authority must be disclosed and addressed, not omitted; agent maps which techniques are open in the likely forum and rates each as strong/weak; options needing a higher court are flagged as cost/escalation issues.
- **Evaluation evidence or criterion:** Given a binding adverse case, the output names it, selects only techniques available to the relevant court, and does not claim per incuriam merely because the case seems wrong.
- **Failure / misuse conditions:** Ignoring adverse authority; "distinguishing" on immaterial facts; treating disapproval by a non-binding court as removal of authority.
- **Repair implication:** Insert adverse-authority section; re-rate prospects.
- **Proposed disposition:** retain as an options checklist; qualify each limb pending verification.

#### FF1-24
- **ID:** FF1-24
- **Location:** ch 6, §6.3.4 The operation of judicial precedent in the courts, pp. 156-162 and Figure 6.8, p. 161; ch 4, §4.3 The courts, their personnel, and their jurisdictions, pp. 100-108
- **Problem addressed:** Authority weight depends on a court map that changes over time.
- **Principle / method / heuristic (own words):** The book models "who binds whom" as a lookup: for each court, whether it binds itself, which courts it binds, and named exceptions; first-instance courts at the bottom bind nobody and are rarely reported; decisions of a single judge at High Court level bind below but only persuade sideways; tribunals sit in a two-tier structure with onward appeal on law. It also models successor courts by assumption (the new top court treated as inheriting its predecessor's practice "for practical purposes").
- **Assumptions and applicability:** Snapshot as at 2010, including a newly created Supreme Court and tribunal system; details are substantive (section 3).
- **Production responsibility affected:** authority verification; reasoning/applicability
- **Workflow / decision implication:** Maintain the court-hierarchy table as dated reference data with a verification date, not as model knowledge; when a court is renamed or replaced, record the basis for treating old decisions as carrying over.
- **Evaluation evidence or criterion:** Weight labels cite the hierarchy table version used.
- **Failure / misuse conditions:** Using the 2010 map (e.g. EU court at the apex) today.
- **Repair implication:** Refresh table from current primary sources.
- **Proposed disposition:** adapt — keep the lookup design, rebuild the content.

#### FF1-25
- **ID:** FF1-25
- **Location:** ch 1, §1.2.1.2 The institutions of the European Community, pp. 21-24; ch 2, §2.2.2.1 The Treaty of Amsterdam: renumbering treaty provisions, p. 59; ch 2, §2.2.1 The Official Journal, pp. 57-58; ch 5, §5.3.1.1-5.3.1.3, pp. 133-134; ch 5, §5.4, pp. 135-137
- **Problem addressed:** Identity errors in supranational sources.
- **Principle / method / heuristic (own words):** The authors repeatedly warn about look-alike bodies (two different European courts in different cities under different treaties; three similarly named "Councils"; Commission "Decisions" versus court decisions) and about treaty articles that were renumbered, so an article number is meaningless without knowing which numbering scheme the citing document uses. Only one publication is the official text of EU legislation; official court reports lag (translation), so faster commercial reports are unofficial. The EU court itself is said not always to use "directly applicable" and "direct effect" consistently.
- **Assumptions and applicability:** Pre-Brexit; institutional details perishable. The identity-disambiguation habit is durable (and the treaties have been renumbered again since).
- **Production responsibility affected:** authority verification; research; escalation
- **Workflow / decision implication:** When a source cites a treaty article or a "European" body, resolve identity and numbering era before use; record official versus unofficial text.
- **Evaluation evidence or criterion:** Agent correctly refuses to equate the two European courts and maps an old article number to its current number with source.
- **Failure / misuse conditions:** Attributing a human-rights judgment to the EU court; citing a superseded article number.
- **Repair implication:** Correct identity; re-verify the proposition.
- **Proposed disposition:** adapt; research further for current position.

### 3. Substantive-law statements noted (research questions only)

None of the following is recorded as a finding about the law. Each needs checking against current primary sources.

1. Is it still the default that a UK Act comes into force at the start of the day of Royal Assent absent contrary provision (book cites Interpretation Act 1978 s 4 and an 1879 case)? (pp. 15, 68-69)
2. Is there still a presumption that post-1707 UK Acts extend to the whole UK, and what is the present status of the Sewel Convention and devolved competence? (p. 15)
3. What are the current parliamentary procedures for statutory instruments (negative / affirmative / none) and the proportions the book gives? (pp. 16-17)
4. On what grounds can delegated legislation now be held ultra vires; does conflict with earlier primary legislation or EU-origin law still invalidate it? (pp. 17-18)
5. What is the current effect of HRA 1998 ss 2, 3, 4, 6, 10 and 19; is Ghaidan v Godin-Mendoza still the leading account of s 3; is R v A still good law? Has the HRA been amended or replaced? (pp. 16, 85-87, 162-164)
6. Post-Brexit: what replaced ECA 1972 ss 2(1), 2(4), 3(1); what is the status of retained/assimilated EU law, of CJEU decisions in UK courts, of the Article 234 (now 267 TFEU) reference procedure and the CILFIT criteria; do Pickstone/Litster-style readings survive? (pp. 24-30, 79-80, 85, 156, 164-165)
7. Direct applicability / direct effect, the Van Gend criteria, horizontal effect of directives, Francovich liability — current EU-law position (relevant for EU-member-state matters only). (pp. 25-28)
8. Is the purposive approach still described by the UK Supreme Court as predominant; how do courts now treat tax and social-welfare statutes differently? (p. 79)
9. Are the Pepper v Hart conditions unchanged; how has later case law narrowed or applied them; does the principle extend to Law Commission and committee reports as the book says? (pp. 84-85)
10. Current status of intrinsic aids: are headings and side-notes treated as the book states (R v Montilla)? Are Explanatory Notes admissible as aids? (pp. 70, 83)
11. Are the listed presumptions (against retrospectivity, against ousting jurisdiction, mens rea, Crown immunity, etc.) stated accurately for today? (p. 82)
12. Does the 1966 Practice Statement apply to the UK Supreme Court, and on what authority (the book only assumes so)? What criteria now govern departure? (pp. 157-158)
13. Are the Young v Bristol Aeroplane exceptions still the complete list for the Court of Appeal (Civil Division); what is the present position on Privy Council decisions and the Court of Appeal (book cites Re Spectrum Plus and a suggestion by Baroness Hale)? (pp. 159-160)
14. Is the per incuriam test still that the court "must inevitably" have decided differently, and "manifestly wrong"? (p. 160)
15. Does the Court of Appeal (Criminal Division) still have the wider R v Gould latitude; can a five-judge court depart from a three-judge decision; are the two Divisions bound by each other? (p. 160)
16. Do High Court judges bind each other; status of Divisional Court decisions; does the Crown Court bind anyone; precedent in the Upper Tribunal and First-tier Tribunal (not addressed by the book)? (p. 162)
17. Must a lower court follow Strasbourg over a binding domestic higher-court decision, as the book suggests from Re Medicaments? (The book flags only "see also" Price v Leeds.) (pp. 163-164)
18. Current court structure: single County Court and Family Court, track financial limits (book: small claims 5,000; fast track 25,000), allocation of High Court business, tribunal chambers, abolition of bodies named. (pp. 101-108)
19. Neutral citation: current list of courts and abbreviations, including tribunals and new lists/courts. (pp. 114-115)
20. Which report series must be cited in court when a case is reported in several (hierarchy of reports / practice directions)? The book asks but does not answer this in the assigned range. (p. 120)
21. The seven tests for local custom and the 1189 date. (pp. 99-100)
22. Equitable maxims and the discretionary nature of equitable remedies as summarised in Table 4.1. (pp. 97-99)
23. Judicial review grounds (illegality, irrationality, procedural impropriety), standing test and the four-question Convention-rights analysis. (p. 104)
24. Is the meaning of "(C. n)" in an SI citation the parent Act's chapter number (as the book says) or a commencement-order series number? The instrument reproduced in the book is inconsistent with the book's explanation. (p. 74)

### 4. Material the author marks as contested, or where the author criticises other approaches

- Literal approach: criticised by the authors for producing "unthinking" outcomes, assuming perfect drafting and ignoring limits of language; an example is said to defeat Parliament's evident aim (ch 3 §3.3.1.1, p. 77).
- "Rules" of interpretation: authors say they are not rules; judges need not follow or disclose any (p. 76). Whether the court finds Parliament's intention or guesses what it would have intended is presented as an open characterisation (p. 76).
- HRA s 3: the book presents R v A as arguably "quasi-legislation", sets out Lord Hope's dissenting concern about judges legislating, and then Ghaidan as clarifying; marked as a live tension between interpretation and amendment (pp. 86-87).
- Hansard: authors note judicial reluctance in practice and point to academic debate (further reading: a reply to Lord Steyn on retreat from Pepper v Hart) (pp. 85, 89).
- Ratio of Donoghue v Stevenson: authors report disagreement over whether the broad neighbour-type principle was ratio or obiter later adopted; they conclude ratio is "ultimately determined" by later courts (p. 156). They also say academic discussion of how to find a ratio is extensive (p. 155, quoting the court).
- 1966 Practice Statement: some thought such a change should have come by legislation; authors stress reluctance to use it (pp. 157-158). Tension noted between the Statement's wording and the dictum that a wrong decision is not enough (p. 157).
- Court of Appeal and Privy Council disapproval: recorded as not an exception, but with a judicial suggestion that it might become one (p. 159).
- Criminal/Civil Division relationship: "no ruling" on whether they bind each other (p. 160).
- EU terminology: the EU court is said not to distinguish consistently between direct applicability and direct effect (p. 26); exceptions to the no-horizontal-effect rule for directives are footnoted (p. 27 n 19). European Parliament's censure power described via a quoted critic as largely illusory (p. 22).
- Delegated legislation: authors weigh speed/expertise against reduced scrutiny and publicity (p. 18).
- Source-tool criticisms: Law Reports—Statutes "hardly worth waiting for"; Chronological Table 2-3 years stale; Halsbury's Statutes comprehensive but cumbersome and splits one Act across subject volumes; Official Journal Index unhelpful; CELEX hard to use (pp. 37-38, 44, 60, 62).
- Internal inconsistencies observed in the book itself (relevant to how far to trust it as a secondary source): Hunting Act dated 2004 at p. 11 and 2005 at p. 15; Abortion Act dated 1967 at p. 11 and 1963 at p. 78; the EU Court of Justice described as having "originated as a discussion chamber" (apparently copied from the Parliament entry) at p. 22; SI example titled 2003 in text and 2006 in the instrument (p. 73-74); figure caption "Misrepresentation Act 2006" for the 1967 Act (p. 70); the "(C. 4)" explanation (p. 74); the EHRR citation example for Handyside shows a Series A citation instead (p. 137); first-instance civil defendant called "respondent" (p. 143). These are observations from the text only; none has been checked externally.

### 5. Content in the assigned range that is out of scope for legal production (and why)

- Introduction (pp. 1-3): book rationale and structure for students; study-skills framing.
- ch 1 §1.1.1.1-1.1.1.4 and §1.1.1.6 parliamentary stages, Bill types, Parliament Acts history (pp. 10-15): civics background; does not change how an enacted provision is found, verified or applied (except commencement/extent, captured above).
- ch 1 §1.2.1.1-1.2.1.2 EU history, membership table, composition and voting of institutions (pp. 19-24): dated institutional description.
- ch 4 §4.1.1 legal history (not read) and §4.1.3 equity maxims, §4.2 custom (pp. 94-100): doctrinal background, substantive.
- ch 4 §4.3 personnel, judicial titles, numbers of courts, addresses (pp. 100-108): descriptive and dated; only the hierarchy-for-authority aspect is retained (FF1-24).
- ch 2 and ch 5 print-library procedures, volume date ranges, colour of bindings, URLs, database blurbs, screenshots, practical exercises and self-test questions: perishable tool detail; method abstracted in FF1-04 to FF1-08, FF1-18, FF1-19.
- Written-style points (do not start a sentence with "s"; abbreviations "sch", "para", "reg", "r") (pp. 70, 72, 75): minor citation style; belongs to a house-style layer, not to a skill.
- Counsel names being useful for choosing a barrister (p. 146): practice-management aside.

### 6. Candidate benchmark cases suggested by the text (own words, synthetic)

1. **Uncommenced subsection.** A fictional "Data Brokers Act 2021" has s 12(1)-(4) commenced by order on a stated date and s 12(5) never commenced; a second order commences s 14 only in three named regions. The user asks whether s 12(5) and s 14 bind a company in a fourth region. Pass: agent reports provision-level and area-level status with the commencing instrument, refuses to apply s 12(5), and does not infer the in-force date from "2021".
2. **Varied, not amended.** A section's text is unchanged since enactment, but a later instrument varies its application to small enterprises and another disapplies it for a transitional period. Pass: agent's status check returns typed effects and the answer differs for a small enterprise during the transitional window.
3. **Amending section trap.** The user supplies only the text of an amending section ("in subsection (2), for 'X' substitute 'Y'") and asks what the law requires. Pass: agent says the amending text is not the operative rule, retrieves or requests the revised target provision, and states the version date.
4. **As-at date.** Facts occurred before a substitution of a key subsection. Pass: agent applies the earlier wording, flags the change, and states the source for historical text.
5. **Headnote discrepancy.** Provide a synthetic report whose headnote omits a temporal limit that appears in the judgment. Pass: agent states the holding from the judgment and flags the headnote as inaccurate.
6. **Reversed on appeal.** Provide an intermediate appellate decision with a citator entry showing reversal by the top court, plus an unrelated later case that "applied" the intermediate decision before reversal. Pass: agent declines to rely on the reversed point and explains the chronology.
7. **Binding or persuasive by forum.** The same four authorities (top-court obiter, co-ordinate court ratio, first-instance ratio, foreign apex-court ratio) are to be weighed first for a first-instance judge and then for the intermediate appellate court. Pass: labels change correctly with the forum and each label names the limb of the three-part test that decides it.
8. **Ratio at multiple levels.** A synthetic judgment about a contaminated sealed product. Pass: agent proposes narrow, middle and broad formulations, applies the "would changing this fact change the result?" test to discard immaterial facts, and says which formulation later (supplied) cases have adopted.
9. **Adverse precedent options.** A binding co-ordinate-court decision is against the client; supplied materials include an earlier conflicting decision of the same court and a later, inconsistent decision of the higher court that does not mention it. Pass: agent discloses the adverse case, identifies conflict and implied-overruling routes as open, rejects per incuriam absent an overlooked binding authority, and frames prospects as risk.
10. **Gated legislative history.** Clear statutory text; the user offers a backbench speech supporting a different reading. Pass: agent declines to use it to override clear text, explains the gating conditions, and treats it as background only.
11. **List plus general words.** Provision: "any kiosk, booth, stall or other place". Question: does an online marketplace fall within "other place"? Pass: agent raises the class-limitation canon, identifies the common characteristic, notes the canon is rebuttable, checks for a statutory definition first, and presents competing readings.
12. **SI validity and dates.** An instrument recites an enabling power limited to "fees"; its body creates a criminal offence; it shows made, laid and coming-into-force dates that differ. Pass: agent uses the correct in-force date, flags a possible excess-of-power issue, and escalates rather than deciding validity.
13. **Identity and numbering.** A memo cites "Article 119" of the founding EU treaty and attributes a human-rights ruling to "the European Court" in Luxembourg. Pass: agent resolves the numbering era, separates the two courts, and corrects the attribution.
14. **Citation integrity.** A list of six case citations in which one has round instead of square brackets for a year-identified series, one has a court code inconsistent with the named court, and one does not resolve anywhere. Pass: agent flags all three, corrects only what it can verify, and removes the unresolvable authority.
15. **Trusting the textbook.** Provide a secondary-source paragraph containing two internally inconsistent dates for the same Act. Pass: agent notices the inconsistency and verifies against the primary source instead of choosing one.

---

## Part 2 — chapters 7–18 (IDs FF2-)

Examiner note: this is a UK undergraduate academic-skills text. Its tools (Westlaw/Lawtel/LexisLibrary coverage tables, print Halsbury's, URLs, OSCOLA 4th edn mechanics) are dated as of 2011 and were not treated as evidence of current tooling. Only method was extracted. Much of the range (study skills, grammar, exams, presentations, referencing style minutiae) is out of scope for legal production and is recorded as such in section 5. Page mapping confirmed from running heads: print page = pdf-page minus 23 throughout this range (e.g. pdf 367 = print 344; pdf 195 = print 172; pdf 441 = print 418; pdf 475 = print 452). All locations below cite print pages.

### 1. Coverage record

| pdf-page range | chapter / section | status | note |
|---|---|---|---|
| 193-205 | Ch 7 Books, journals and official publications (print 171-182) | read fully | Status and use of secondary sources; soft law |
| 206-228 | Ch 8 Finding books, journals, official publications; Halsbury's Laws; Bills; Hansard (print 183-205) | read fully, for method only | Database coverage tables, URLs, Command Paper series, citation formats are dated tool detail; not extracted |
| 229-259 | Part II opener; Ch 9 Study skills (print 207-236) | headings only | Out of scope (lectures, seminars, note-taking, time management, PDP) |
| 260-267 | Ch 10 Writing skills §10.1-10.2 (print 237-244) | read fully | Precision of language; legal vs everyday meanings; abbreviations |
| 267-279 | Ch 10 §10.3 Grammar and punctuation (print 244-256) | not read (first lines only) | General grammar; out of scope |
| 279-285 | Ch 10 §10.4-10.6 paragraphs, quotations, word limits (print 256-262) | read fully | Quotation discipline; concision tests |
| 285-289 | Ch 10 §10.7 Presentation | not read | Formatting of coursework |
| 290-300 | Ch 11 §11.1-11.2 plagiarism, when to reference, styles (print 267-276) | read fully | Why/when to reference |
| 300-323 | Ch 11 §11.3-11.4 OSCOLA and Harvard mechanics (print 277-300) | skimmed headings; read §11.3.3.2 (pinpoints, print 280-281) and §11.3.7 (internet sources, print 287) | Style minutiae not extracted |
| 324-327 | Ch 12 §12.1-12.2 (print 301-304) | headings only | Essay-question analysis |
| 328-338 | Ch 12 §12.3 Research and planning (print 305-315) | read fully | Research trail; notes by issue; supporting material hierarchy |
| 338-342 | Ch 12 §12.4-12.5 | not read | Essay writing craft |
| 343-365 | Ch 13 Dissertations (print 320-342) | headings; read §13.5 (print 338-339) | Source-range advice only |
| 366-389 | Ch 14 Answering problem questions (print 343-366) | read fully | Core chapter |
| 390-439 | Ch 15 Revision/exams; Ch 16 Presentation skills (print 367-416) | headings only | Out of scope |
| 440-445 | Ch 17 §17.1 The moot problem (print 417-422) | read fully | Court level, fixed facts, case history |
| 445-450 | Ch 17 §17.2 Participants (print 422-427) | not read | Moot roles/etiquette |
| 450-465 | Ch 17 §17.3 Researching the moot; §17.4 Preparing to moot incl. submissions, skeletons, bundles (print 427-442) | read fully | Argument from authority; counter-argument |
| 465-468 | Ch 17 §17.5.1 (print 442-444) | not read | Speech openings/closings |
| 467-470 | Ch 17 §17.5.2-17.5.3 judicial interventions, using cases (print 444-447) | read (de-duplicated text) | Oral citation convention not extracted |
| 470-473 | Ch 17 remainder/summary | not read | |
| 474-488 | Ch 18 §18.1-18.3 (print 451-465) | read fully | Preparation of negotiating positions |
| 488-495 | Ch 18 §18.4-18.5 conducting/reflection (print 465-472) | headings; read §18.4.1 opening lines and §18.4.5 ethics (print 470) | Conduct-of-negotiation technique mostly not read |

The extracted text duplicates many boxed passages (box text appears twice); duplication was read through, not double-counted.

### 2. Material findings

#### FF2-01
- **ID:** FF2-01
- **Location:** ch 14, §14.2 Problem-solving technique (incl. Figure 14.1), pp. 345-347 (print)
- **Problem addressed:** Analysts who know the law still fail to answer the client's actual question because they lack a repeatable reasoning procedure.
- **Principle / method / heuristic (own words):** Every named mnemonic (IRAC, IPAC, CLEO, PLAN) reduces to the same four moves: frame the precise question; state the rule that answers it; work out how the rule operates on these facts; state a conclusion that answers the question framed. The procedure is domain-independent (the authors demonstrate it on a coursework late-penalty rule) and transfers across areas of law.
- **Assumptions and applicability:** Presented for UK law-school fact-pattern questions, but framed by the authors as the skill a client expects (advice on the client's situation, not a survey of decided cases). Assumes the facts are given; does not address fact-gathering.
- **Production responsibility affected:** reasoning/applicability, issue spotting, evaluation
- **Workflow / decision implication:** An applicability-analysis skill should emit, per issue, four explicitly separable elements (question, rule with authority, application to named facts, conclusion) rather than narrative discussion.
- **Evaluation evidence or criterion:** For each issue in an output, can a reviewer point to the four elements, and does the conclusion answer the question as framed (not a neighbouring question)?
- **Failure / misuse conditions:** Treating the mnemonic as a document layout (see FF2-02); using it where the task is evaluative commentary rather than determination of a position.
- **Repair implication:** If any element is missing for an issue, regenerate that issue block rather than patching the prose.
- **Proposed disposition:** retain — baseline reasoning skeleton; merge with equivalent IRAC-type findings from other books.

#### FF2-02
- **ID:** FF2-02
- **Location:** ch 14, §14.2.1 Warning, p. 348; §14.4.3.1 Law in large chunks, p. 356 (print)
- **Problem addressed:** The commonest structural failure: applying the four-step method once to the whole problem (all issues listed, then all law, then a thin application, then a summary).
- **Principle / method / heuristic (own words):** The four-step cycle must run once per sub-issue. A pooled "law" section detaches rules from facts and guarantees weak application. Finish rule-application-conclusion for one sub-issue before stating the rule for the next.
- **Assumptions and applicability:** General; especially relevant to long memos and multi-party matters.
- **Production responsibility affected:** reasoning/applicability, drafting, review/redlining
- **Workflow / decision implication:** Agent output structure should be issue-nested (issue > sub-issue > rule/application/conclusion), not section-by-function. A reviewer skill should flag any standalone block of legal exposition that is not immediately followed by application.
- **Evaluation evidence or criterion:** No paragraph run of pure law longer than one sub-issue's worth; each sub-issue has its own mini-conclusion.
- **Failure / misuse conditions:** Over-fragmentation of trivially satisfied elements (the authors accept brief treatment of unproblematic elements — see FF2-08).
- **Repair implication:** Re-cut the document by sub-issue and relocate each rule statement next to the facts it governs.
- **Proposed disposition:** retain — concrete, checkable structural rule.

#### FF2-03
- **ID:** FF2-03
- **Location:** ch 14, §14.3.1 Analyzing the question (parties, events; Table 14.1, Figure 14.3), pp. 349-350 (print)
- **Problem addressed:** Issues are missed because facts are read impressionistically.
- **Principle / method / heuristic (own words):** Build a "who did what to whom" grid first: list every person, classify each as potential claimant, potential defendant or other; list each event/harm and link it to a claimant-defendant pair. People who fit neither role are probably there for a reason and must be accounted for. Work sentence by sentence, logging potentially relevant facts even when their relevance is not yet understood; the list later forces precise factual reference during application.
- **Assumptions and applicability:** Designed for constructed scenarios where every fact is deliberate; in real matters irrelevant facts are common, so "every fact matters" becomes "every fact is triaged and the triage is recorded".
- **Production responsibility affected:** scoping, issue spotting
- **Workflow / decision implication:** Issue-spotting skill should produce a party/event/relationship matrix and an "unexplained facts" list before any legal research starts.
- **Evaluation evidence or criterion:** Every person and every harm/event in the input appears in the matrix; every fact is either used in an issue or listed as unassigned with a reason.
- **Failure / misuse conditions:** Jumping to the most familiar issue; ignoring third parties (e.g. a contractor or a supervising adult) who change the analysis.
- **Repair implication:** When a missed issue is found late, return to the matrix and re-run linkage rather than bolt on a paragraph.
- **Proposed disposition:** retain/adapt — adapt the "every fact is deliberate" assumption for real instructions.

#### FF2-04
- **ID:** FF2-04
- **Location:** ch 14, §14.3.2 Finding the subissues (Figure 14.4 and worked outline), pp. 351-352 (print)
- **Problem addressed:** "Big" liability questions are too coarse to be reasoned about or checked.
- **Principle / method / heuristic (own words):** Decompose each head of liability into the legal elements that must each be established (status of defendant, status of claimant, nature of duty, exclusion, defences, etc.). Each element becomes a mini-question with its own rule, application and conclusion; the big issue is concluded only by drawing the element conclusions together.
- **Assumptions and applicability:** Requires knowing the element structure of the cause of action, which itself comes from research (so the decomposition is revised after initial reading — §14.4.1, p. 354).
- **Production responsibility affected:** issue spotting, reasoning/applicability, research
- **Workflow / decision implication:** Agent should derive an element checklist from authority for each candidate cause of action and treat the checklist as provisional until research confirms it.
- **Evaluation evidence or criterion:** Each element in the governing test appears as a sub-issue; none is silently assumed; defences/exclusions are included, not only positive elements.
- **Failure / misuse conditions:** Element list taken from memory or a secondary summary and never verified; omission of defences.
- **Repair implication:** Re-derive the checklist from the primary source and diff it against the sub-issues analysed.
- **Proposed disposition:** retain.

#### FF2-05
- **ID:** FF2-05
- **Location:** ch 14, §14.3.2.1 Identifying the correct area of law, pp. 352-353; §14.3.2.2 Multiple areas of law, p. 353 (print)
- **Problem addressed:** When instructions do not name the legal basis, a wrong characterisation derails everything downstream.
- **Principle / method / heuristic (own words):** Enumerate candidate legal areas, reduce each to a short statement of its essential nature, and eliminate those that cannot fit the facts; keep all survivors. Where the same facts plausibly support more than one basis, analyse each and then evaluate which is the more suitable. If still unsure, ask for guidance, framing the query as a specific proposed scope.
- **Assumptions and applicability:** The book's first step (eliminate what the syllabus has not covered) is a student shortcut with no professional analogue; the rest generalises. The "ask, stating your proposed scope" move maps to scoping confirmation with the instructing person.
- **Production responsibility affected:** scoping, issue spotting, escalation
- **Workflow / decision implication:** A characterisation step should output a candidate list with one-line essence and an include/exclude reason for each, and should trigger a scoping question when more than one basis survives and the instruction is ambiguous.
- **Evaluation evidence or criterion:** Output shows rejected as well as accepted legal bases with reasons; overlapping bases are compared rather than one silently chosen.
- **Failure / misuse conditions:** Candidate universe limited to what the analyst happens to know (the professional version of the syllabus shortcut).
- **Repair implication:** Widen the candidate list using a comprehensive index/encyclopaedic source before eliminating.
- **Proposed disposition:** adapt — drop syllabus logic; keep enumerate-summarise-eliminate-compare.

#### FF2-06
- **ID:** FF2-06
- **Location:** ch 14, §14.7.1 Follow the instructions, pp. 363-364 (print)
- **Problem addressed:** Scope creep: analysing issues the instruction excluded, or reorganising a structured question.
- **Principle / method / heuristic (own words):** The instruction defines the party advised, the area of law and the structure. Issues raised by the facts but excluded by the instruction earn nothing and consume capacity owed to in-scope issues. If the question is set out in lettered parts, answer in those parts, in that order, with those labels.
- **Assumptions and applicability:** Assessment framing. In practice an excluded-but-serious issue would normally be flagged rather than ignored; the book does not address that and should not be read as forbidding a flag.
- **Production responsibility affected:** scoping, drafting, escalation
- **Workflow / decision implication:** Agent should parse the instruction for (a) who is advised, (b) limits on subject matter, (c) required structure, and mirror (c) exactly; out-of-scope observations go in a short separate flag, not in the analysis.
- **Evaluation evidence or criterion:** Output headings map one-to-one to the instruction's parts; no in-body analysis of expressly excluded heads.
- **Failure / misuse conditions:** Reading the rule as licence to stay silent about a material out-of-scope risk in a real matter.
- **Repair implication:** Move out-of-scope analysis to a flagged note; restore instruction's structure.
- **Proposed disposition:** qualify — retain scope discipline, add professional duty to flag.

#### FF2-07
- **ID:** FF2-07
- **Location:** ch 14, §14.4.1 Researching the law, p. 354 (print)
- **Problem addressed:** Unfocused research and research that stops at a secondary summary.
- **Principle / method / heuristic (own words):** Read a secondary overview first; then revisit and correct the issue/sub-issue framing; then research sub-issue by sub-issue with notes kept per sub-issue; record statutory wording and full citations exactly at the time of reading; follow footnoted authorities the overview does not explain; concentrate on the current law and its interpretation, not history; do not expect an on-point answer — look for general principles and analogous cases because the facts are designed to be novel; jot provisional views on application as you go.
- **Assumptions and applicability:** Student workflow, but every step maps to a research loop. "Current law only" applies to advice-type outputs, not to law-reform or policy pieces.
- **Production responsibility affected:** research, authority verification, issue spotting
- **Workflow / decision implication:** Research skill should have an explicit "re-frame issues after orientation reading" checkpoint and should store notes keyed by sub-issue with exact text and full citation captured at source.
- **Evaluation evidence or criterion:** Research log shows issue list before and after orientation; each sub-issue has at least one primary authority with exact citation; no sub-issue rests only on the overview text.
- **Failure / misuse conditions:** Treating the absence of an on-point case as absence of law; importing historical or comparative material into an advice output.
- **Repair implication:** Where no on-point authority exists, state that and reason from the nearest principle/analogue explicitly.
- **Proposed disposition:** retain.

#### FF2-08
- **ID:** FF2-08
- **Location:** ch 14, §14.4.2 Stating the law, pp. 355-356; §14.4.3.2 No abstract statement of the law and Table 14.2, pp. 356-357; §14.4.3.3 Too much detail, p. 357 (print)
- **Problem addressed:** Rule statements that are either contaminated with the facts, unsupported, or bloated.
- **Principle / method / heuristic (own words):** State the rule first in abstract, general terms with its source (statute or case), adding further authority only where it sharpens the test for the point in dispute. Saying "the element is satisfied by [this fact]" is application, not a statement of law; merging the two hides whether the analyst knows the rule. Calibrate depth: the more uncertain the law or complicated the issue, the more principle is needed; a simple foundational element gets a short but still explicit treatment. Apply a "so what?" test to each sentence and delete anything that contributes nothing to resolving the sub-issue, especially narrated case facts and law on issues the facts do not raise.
- **Assumptions and applicability:** General. The "so what?" test is phrased for word-limited coursework but serves client-facing concision equally.
- **Production responsibility affected:** reasoning/applicability, drafting, authority verification, review/redlining
- **Workflow / decision implication:** Rule blocks must be fact-free and each carry an authority; a reviewer pass should test each rule sentence for (a) abstraction, (b) authority, (c) necessity to the sub-issue.
- **Evaluation evidence or criterion:** Rule sentence contains no party names or matter facts; has a cited source; removing it would leave the sub-issue unresolvable (otherwise delete).
- **Failure / misuse conditions:** Collapsing rule and application to save space; over-citing on uncontested elements; under-citing on the contested one.
- **Repair implication:** Split fused sentences into rule then application; reallocate depth toward the contested element.
- **Proposed disposition:** retain.

#### FF2-09
- **ID:** FF2-09
- **Location:** ch 14, §14.5 Application and evaluation, p. 358; §14.5.1.1 Lazy application and Figure 14.6, pp. 359-360 (print)
- **Problem addressed:** Application that asserts rather than demonstrates, or that hands the decision to someone else.
- **Principle / method / heuristic (own words):** Application means selecting the specific facts that satisfy (or fail) each requirement of the rule and saying so. Two named defects: (1) generic assertion that a requirement is met "on the facts" without naming the facts; (2) abdication — observing that the point is one for the court or jury and stopping. Even where a tribunal of fact will decide, the adviser must marshal the available facts into a predicted, even tentative, answer, because the client is asking what will happen to them.
- **Assumptions and applicability:** General to any advice product. Prediction must still be calibrated (see FF2-10, FF2-13).
- **Production responsibility affected:** reasoning/applicability, risk communication, review/redlining
- **Workflow / decision implication:** Ban (and lint for) phrases of the "clearly satisfied on the facts" and "this will be a matter for the court" type unless followed by named facts and a predicted direction.
- **Evaluation evidence or criterion:** Every application paragraph names at least one matter-specific fact tied to a rule element; any "question of fact" statement is followed by a reasoned likelihood.
- **Failure / misuse conditions:** Over-correcting into unjustified certainty; predicting where the necessary facts are absent without saying so.
- **Repair implication:** Replace assertion with fact-to-element mapping; add a tentative prediction with its basis.
- **Proposed disposition:** retain — directly usable as an evaluation rubric item.

#### FF2-10
- **ID:** FF2-10
- **Location:** ch 14, §14.5.2.1 Speculative application and Figure 14.7, p. 361; chapter summary, p. 366 (print)
- **Problem addressed:** The facts supplied are insufficient to determine an element.
- **Principle / method / heuristic (own words):** Where a needed fact is missing, reason conditionally ("if X then Y") across the realistic alternatives. Binary gaps (e.g. whether a permission was granted) need only a sentence; gaps that turn on an open-textured term deserve illustrated alternatives showing where the boundary lies. First apply the general rule, then consider whether an exception might apply. The conclusion after conditional reasoning must be marked as the best available on known facts and liable to change if further facts emerge or a different interpretation is preferred. Do not stray far from the given facts.
- **Assumptions and applicability:** In coursework the missing fact cannot be obtained; in practice it often can. The professional adaptation is: reason conditionally AND raise the fact as a question to the client.
- **Production responsibility affected:** reasoning/applicability, risk communication, scoping, escalation
- **Workflow / decision implication:** Agent should maintain a "missing facts" register; each entry records the element affected, the branches, the outcome on each branch, and a question for the instructing person. Conclusions depending on a branch must carry the contingency flag.
- **Evaluation evidence or criterion:** No invented facts; each identified gap has explicit branches and a contingent conclusion; hypotheticals stay within the plausible range of the given scenario.
- **Failure / misuse conditions:** Silent assumption of the missing fact; speculative branches proliferating beyond what the facts could support; using speculation to avoid asking an answerable question.
- **Repair implication:** Convert hidden assumptions into stated branches; add client questions.
- **Proposed disposition:** adapt — add "ask the client" limb absent from the text.

#### FF2-11
- **ID:** FF2-11
- **Location:** ch 14, §14.5.2.2 Taking a balanced approach, pp. 361-362; summary, p. 366 (print)
- **Problem addressed:** One-sided analysis and premature reliance on the first authority found.
- **Principle / method / heuristic (own words):** Because adjudication tests competing claims, each contested sub-issue should be examined for a viable counter-argument; not every element has one, and uncontested elements should not be padded with invented opposition. Where the point turns on the meaning of a word or phrase, do not stop at the first case: search for conflicting authority that would support a different outcome. Where the facts are silent on the point that would found the counter-argument, use conditional reasoning (FF2-10) to explore it.
- **Assumptions and applicability:** General. The authors' incentive framing (extra marks) is academic; the underlying method is professional.
- **Production responsibility affected:** reasoning/applicability, research, authority verification, risk communication
- **Workflow / decision implication:** For each contested sub-issue, run a deliberate contrary-authority search and record its result (including "none found, searched X"). Output should state the strongest counter-position and why it is or is not likely to prevail.
- **Evaluation evidence or criterion:** Contested elements show both positions with authority; interpretive points show evidence of a search for conflicting decisions.
- **Failure / misuse conditions:** False balance on clear points; omitting adverse authority because it is inconvenient.
- **Repair implication:** Add contrary-authority search and adverse-case treatment to the sub-issue.
- **Proposed disposition:** retain.

#### FF2-12
- **ID:** FF2-12
- **Location:** ch 14, §14.5.2.3 Supporting authority, p. 362; summary, p. 366 (print)
- **Problem addressed:** "Citation by bracket": a case name appended to a sentence without showing what it establishes — or worse, implying it decided something it did not.
- **Principle / method / heuristic (own words):** An authority supports a proposition only when the text states the principle drawn from it and links that principle to the present facts, including how it may affect the outcome. A bare parenthetical adds nothing; a loose "this issue was discussed in [case]" can actively mislead by suggesting the case concerned the present fact pattern.
- **Assumptions and applicability:** General; high relevance to machine-generated citations, where the citation-proposition link is the main hallucination risk.
- **Production responsibility affected:** authority verification, reasoning/applicability, drafting, review/redlining
- **Workflow / decision implication:** For each cited case the agent must be able to state (a) the principle relied on, (b) where in the judgment it is found, (c) how it maps to a fact in the matter. Citations that cannot pass (a)-(c) are removed or flagged for verification.
- **Evaluation evidence or criterion:** Each citation is accompanied by a one-sentence principle and a fact linkage; a verifier can confirm the principle against the source.
- **Failure / misuse conditions:** Principle paraphrased from a textbook's account without reading the case (see FF2-15, FF2-16); overstating how close the cited facts are.
- **Repair implication:** Read the source; rewrite the sentence as principle + linkage; downgrade wording where the case is only analogous.
- **Proposed disposition:** retain — core citation-discipline criterion.

#### FF2-13
- **ID:** FF2-13
- **Location:** ch 14, §14.6 Conclusion and outcome, pp. 362-363; summary, p. 366 (print)
- **Problem addressed:** Conclusions that are absent, falsely definite, or inconsistent with the body.
- **Principle / method / heuristic (own words):** Conclude at three levels — each sub-issue, each issue (cumulatively from its sub-issues), and the whole question — and check the levels for consistency after drafting. Law usually yields stronger and weaker arguments rather than right answers, so the target is the conclusion most likely to be reached. An "it depends" conclusion is legitimate provided the specific contingency is named. Always supply the overall conclusion; never leave the reader to assemble it from scattered mini-conclusions.
- **Assumptions and applicability:** General.
- **Production responsibility affected:** risk communication, reasoning/applicability, product consistency, review/redlining
- **Workflow / decision implication:** Generate a conclusions roll-up table (sub-issue > issue > overall) and run an automated consistency check between body findings and the executive conclusion; require every hedged conclusion to name its contingent fact or interpretive choice.
- **Evaluation evidence or criterion:** (a) An overall conclusion exists and answers the instruction's question; (b) no sub-issue finding contradicts it; (c) each "depends" names what it depends on.
- **Failure / misuse conditions:** Unanchored hedging ("it depends" without the dependency); confident overall conclusion resting on a contingent sub-issue.
- **Repair implication:** Propagate contingencies upward into the overall conclusion; reconcile contradictions by re-examining the sub-issue.
- **Proposed disposition:** retain.

#### FF2-14
- **ID:** FF2-14
- **Location:** ch 14, §14.5.1.2 Essays in disguise, p. 360; §14.7.2 Get to the point, p. 364; §14.7.3 Methodical approach, pp. 364-365; §14.7.4 Check and polish, p. 365 (print)
- **Problem addressed:** Advice drifting into general exposition; fact recitals; cherry-picking the familiar issue; unreviewed first drafts.
- **Principle / method / heuristic (own words):** (i) Replace the test "is this relevant to the topic?" with "is this necessary to establish this part of the law?". (ii) Anchor every paragraph to a named party and a specific fact to prevent drift into abstraction. (iii) Do not open by restating the scenario; restated facts without law applied to them carry no value. (iv) Work issues in order methodically rather than starting with the one that resembles a known case, because that is how less obvious issues get dropped. (v) Never issue a first draft; re-read after a break, checking content accuracy, references, and language.
- **Assumptions and applicability:** Advice/problem-type outputs. (iii) should be qualified: professional advice often needs a short statement of facts relied on and assumptions — that is a record of the factual basis, not padding.
- **Production responsibility affected:** drafting, review/redlining, issue spotting
- **Workflow / decision implication:** Reviewer checks: paragraph-level party/fact anchor; necessity test on each legal statement; issue list worked exhaustively; mandatory second pass.
- **Evaluation evidence or criterion:** Proportion of analysis paragraphs containing a party name and a matter fact; absence of historical/comparative/reform digressions in advice outputs.
- **Failure / misuse conditions:** Deleting the facts-relied-on statement in a professional memo on the strength of (iii).
- **Repair implication:** Cut or relocate non-necessary exposition; add anchors.
- **Proposed disposition:** adapt — qualify (iii) for professional documents.

#### FF2-15
- **ID:** FF2-15
- **Location:** ch 7, §7.1.1 Student textbooks, p. 172; §7.1.2 Cases and materials books, pp. 172-173; §7.1.4 Practitioners' books, p. 173; §7.1.5-7.1.6.2 encyclopedias, digests, judicial dictionaries, pp. 173-175; ch 10 §10.5 Using quotations, pp. 257-258; ch 12 §12.3.5.1 Textbooks, pp. 312-313 and guidelines p. 315 (print)
- **Problem addressed:** Treating secondary sources as if they were the law; relying on extracts; using stale editions.
- **Principle / method / heuristic (own words):** A graded view of secondary material: student textbooks carry little authority (a few established works are occasionally cited in court); extract collections are a starting point only and never substitute for the full primary text, since extracts reflect an editor's selection; practitioner works are multi-volume reference tools updated by supplements or looseleaf and therefore must be read with their updates; encyclopaedic works and digests are finding tools; judicial dictionaries collect judicial and statutory interpretations of words and phrases. Textbooks are for orientation and for harvesting references; they should never be the cited source for a statement of law that lives in a case or statute. Always use the current edition — an out-of-date edition risks inaccurate research.
- **Assumptions and applicability:** England and Wales; the named titles and their status are as of 2011. The hierarchy of persuasive weight of commentary varies by jurisdiction and court.
- **Production responsibility affected:** research, authority verification
- **Workflow / decision implication:** Tag each source by type (primary / practitioner commentary / academic commentary / student text / extract / finding aid) and enforce: statements of law cite primary sources; secondary sources cited only for commentary, interpretation or as locators; edition and currency date recorded for every secondary source.
- **Evaluation evidence or criterion:** No proposition of law supported only by a textbook, extract collection or encyclopaedia entry; every secondary source carries edition/date; extracts are traced to the full source before reliance.
- **Failure / misuse conditions:** Agent cites commentary because it is what retrieval returned; relies on a headnote-like extract; uses superseded edition.
- **Repair implication:** Trace each secondary-only proposition to its primary source, read it, and re-cite.
- **Proposed disposition:** retain — qualify titles/status as dated.

#### FF2-16
- **ID:** FF2-16
- **Location:** ch 7, §7.2 Journals, pp. 175-176; §7.2.5 Some guidance on using journals, pp. 176-177 (print)
- **Problem addressed:** Misuse of commentary: citing the article instead of the primary source it discusses; misreading the author's point; leaning on partisan or lightweight pieces.
- **Principle / method / heuristic (own words):** Books are always to some degree out of date (publication lag; new editions roughly biennially at best), so periodicals are the currency supplement. Articles are opinion about the law, not the law. When the point concerns a primary source, cite the primary source, not the article through which it was found. Academic journals generally carry more weight than practitioner journals, but practitioner journals appear faster and may be the only commentary on a new development — use them with balance and look for a weightier treatment of the same point. Make sure the author's actual argument is understood before using it; explain why the view matters to the argument and take a position on it; be wary of extreme or sensational pieces and present both sides.
- **Assumptions and applicability:** Academic-authority ranking is a UK law-school convention; in practice the weight given to a practitioner note versus an academic article depends on forum and purpose (the moot chapter, §17.3.9.1 pp. 435-436, itself calls the academic/practitioner preference a sweeping generalisation and advises choosing the piece that best supports the argument, knowing who the author is and being able to justify the choice, e.g. recency or depth).
- **Production responsibility affected:** research, authority verification, risk communication
- **Workflow / decision implication:** Commentary may be used for (a) currency alerts, (b) interpretation where primary law is silent, (c) identifying the counter-view; each use must be labelled as commentary with author standing and date, and any primary source it mentions must be read and cited directly.
- **Evaluation evidence or criterion:** No primary-law proposition cited to an article; each commentary citation has author/date/type and a sentence stating what it is used for; opposing commentary acknowledged where it exists.
- **Failure / misuse conditions:** Quoting commentary because it "sounds" authoritative; one-sided sourcing; treating speed-of-publication notes as settled analysis.
- **Repair implication:** Replace article-as-proxy citations with the primary source; add author-standing and date metadata.
- **Proposed disposition:** retain with qualification on the academic-over-practitioner ranking.

#### FF2-17
- **ID:** FF2-17
- **Location:** ch 7, §7.4.1 The Internet, p. 179; ch 12 §12.3.5.5 Internet sources, p. 314; ch 11 §11.3.7 Referencing Internet sources, p. 287 (print)
- **Problem addressed:** Reliability and reproducibility of web-sourced material.
- **Principle / method / heuristic (own words):** Screen web material by: named author and their standing; reputable publication; presence of references; official versus personal site; independent pre-publication review. Official sites are acceptable for official publications; potted legal summaries and tertiary/encyclopaedic sources are for background, terminology and search terms only, never as cited authority (the book notes that a well-known community encyclopaedia says this of itself). Because web content changes, record the access date and keep a permanent copy of web-only material so the research can be substantiated if challenged.
- **Assumptions and applicability:** 2011 web; the criteria remain sound. Directly relevant to agents with web tools.
- **Production responsibility affected:** research, authority verification, evaluation
- **Workflow / decision implication:** Web sources pass a five-point provenance screen before use; tertiary sources are usable only as leads; every web citation stores URL, access date and an archived snapshot/hash.
- **Evaluation evidence or criterion:** Each web citation has provenance fields completed and a retained copy; none supports a proposition of law unless it is an official publisher of primary material.
- **Failure / misuse conditions:** Citing summaries/blogs as law; link rot leaving conclusions unsupported.
- **Repair implication:** Replace with primary/official source; if web-only, archive and mark reliability tier.
- **Proposed disposition:** retain.

#### FF2-18
- **ID:** FF2-18
- **Location:** ch 7, §7.4.4 'Soft law' and Table 7.1, pp. 180-181 (print)
- **Problem addressed:** Codes, circulars, guidance, practice directions, regulator statements and voluntary codes are easily mistaken for binding law or, conversely, ignored.
- **Principle / method / heuristic (own words):** The authors group such instruments (prescriptive rules, procedural rules, instructions, interpretive guides, recommendations, rules of practice, voluntary codes) as quasi-legislation whose legal effect is uncertain until tested in court — sometimes given effect, sometimes not, and not always consistently.
- **Assumptions and applicability:** UK public-law framing; examples are dated (several bodies named no longer exist). The category and the caution generalise.
- **Production responsibility affected:** authority verification, reasoning/applicability, risk communication
- **Workflow / decision implication:** Classify each instrument's status explicitly (binding / statutory guidance to which regard must be had / non-binding / voluntary) and verify whether courts or the parent statute have given it effect before relying on it; communicate status uncertainty to the reader.
- **Evaluation evidence or criterion:** Every non-legislative instrument cited carries a status label with its basis.
- **Failure / misuse conditions:** Presenting guidance as a legal requirement; dismissing guidance that a statute makes relevant.
- **Repair implication:** Research the instrument's statutory footing and judicial treatment; relabel.
- **Proposed disposition:** research further — the specific legal effect of each instrument type is a substantive-law question (see section 3).

#### FF2-19
- **ID:** FF2-19
- **Location:** ch 8, §8.4.1 Using Halsbury's Laws in a library (Figure 8.2), pp. 195-199; §8.2.3 Online, p. 187; §8.1.2.3 References in textbooks, p. 185; §8.3 Finding official publications, pp. 192-193 (print)
- **Problem addressed:** Research that is incomplete (single database) or stale (main text without updates), or that stops at the commentary.
- **Principle / method / heuristic (own words):** Four method points survive the dated tooling: (1) Encyclopaedic route: index term > paragraph > footnotes > the underlying statutory provision or case; the narrative paragraph is a pointer, the footnoted primary source is the target. (2) Layered currency: a main text is current only to its publication date; always go on to the annual supplement and then the latest noter-up, in that order, on every search. (3) Coverage awareness: each database indexes only certain publishers' titles, so a single-database search is not exhaustive (the authors report one 2006 search returning 28, 2 and 8 hits on three services); over-narrow filters (one specialist journal) exclude relevant general-journal material. (4) Harvest references from footnotes and bibliographies of good secondary works; use official/pre-legislative publications and debates to understand why a provision is framed as it is.
- **Assumptions and applicability:** Tools and coverage figures are obsolete; the principles (follow to primary, layer updates, know your corpus gaps) are tool-independent. The worked Olympic-symbol example also models going from a lay client question to index vocabulary.
- **Production responsibility affected:** research, authority verification, change impact
- **Workflow / decision implication:** Research skill records for each source its "current to" date and the update layers checked; records which corpora were searched and known gaps; never ends a trail at an encyclopaedia paragraph.
- **Evaluation evidence or criterion:** Research log shows (a) primary source reached from each secondary pointer, (b) currency check beyond the base text, (c) more than one corpus or a stated coverage limitation.
- **Failure / misuse conditions:** Concluding from the base text alone (the book's own worked example reaches firm advice before reminding the reader to check updates — a sequencing weakness not to be copied); assuming null results mean no material exists.
- **Repair implication:** Re-run with update layers and additional corpora; record limits where a corpus is unavailable.
- **Proposed disposition:** adapt — retain principles, discard tools.

#### FF2-20
- **ID:** FF2-20
- **Location:** ch 11, §11.1.1.1 When to reference, pp. 268-271; §11.1.1.2 Common knowledge, pp. 271-272; §11.2.4 Never mix styles, p. 275; §11.3.3.2 Pinpoint referencing of cases, pp. 280-281; ch 12 §12.3.3.2 research trail, p. 308 and §12.3.3.4 Organizing your research, pp. 309-310 (print)
- **Problem addressed:** Unsupported or mis-sourced statements; citing a source one has not read; unverifiable quotations; losing track of provenance.
- **Principle / method / heuristic (own words):** (a) Four things always need a source: statements of law (to the case or provision), direct quotations, factual/statistical material, and definitions. Referencing is what evidences a statement's authoritative status. Summaries and paraphrases need a source just as quotations do. (b) If a primary source is known only through a secondary account of it, cite it as found "in" the secondary source; citing the primary alone falsely represents that it was read. (c) An idea specific to one judge or author needs attribution; a point appearing unattributed across several standard works may be treated as common knowledge; if in doubt, cite. (d) Use a pinpoint (page or paragraph, and the judge) whenever relying on a particular passage or quoting; a general citation suffices only when the case stands for a point as a whole. (e) One citation style, applied completely and consistently. (f) Keep a research trail: list of sources sought/found/useful, notes keyed by issue with page references, quotation marks around verbatim text in notes, and retain the notes as evidence of the work done.
- **Assumptions and applicability:** Framed around plagiarism in assessment; the plagiarism sanction regime is out of scope, but (a)-(f) are provenance and verification rules directly applicable to machine-assisted work. Style system (OSCOLA 4th, 2010) is jurisdiction- and date-specific.
- **Production responsibility affected:** authority verification, drafting, product consistency, evaluation
- **Workflow / decision implication:** Agent must never cite a primary source it has not itself retrieved without marking it "as cited in"; all quotations and passage-specific reliance carry pinpoints; a provenance log (source, where found, whether read in full, verbatim flags) accompanies the work product.
- **Evaluation evidence or criterion:** Random sample of citations: source retrievable; pinpoint leads to the quoted/paraphrased passage; "as cited in" used where applicable; single style throughout.
- **Failure / misuse conditions:** Citation laundering (lifting a textbook's footnotes as if read); fabricated pinpoints; mixing styles after copy-paste from sources.
- **Repair implication:** Retrieve and read, or downgrade to "as cited in"; add/verify pinpoints; normalise style.
- **Proposed disposition:** retain — adapt plagiarism framing to provenance/verification.

#### FF2-21
- **ID:** FF2-21
- **Location:** ch 10, §10.1 Why are writing skills important?, pp. 238-239; §10.2.1, p. 240; §10.2.2.3-10.2.2.5 Latin, legal words, abbreviations, pp. 242-244; §10.5.2 Effective use of quotations, pp. 259-260; §10.6.1, pp. 260-261 (print)
- **Problem addressed:** Imprecise or ambiguous language changing legal meaning or confusing the reader.
- **Principle / method / heuristic (own words):** (i) Punctuation and word choice can alter legal effect (the authors use a reported contract dispute over a comma governing a termination clause; and a judge's public criticism of an error-strewn indictment) — write for the reader's understanding, not the writer's. (ii) Prefer plain English over archaic formalism; unfamiliar grand words invite misuse. (iii) Do not use a word in its everyday sense inside a field where it is a term of art (e.g. assault, consideration, intention, property); choose a synonym for the lay sense. (iv) Use only standard abbreviations, define on first use, and never let one abbreviation stand for several things. (v) Quotations support, not replace, the writer's own explanation: introduce them, choose the reporting verb deliberately because it signals stance ("alleges" vs "notes"), discuss them, keep them short, mark omissions with ellipses and insertions with square brackets, and never edit so as to reverse or distort meaning (Figure 10.8 shows an ellipsis that inverts the sense). (vi) Concision checks: remove irrelevant points, case-fact narration and surplus words.
- **Assumptions and applicability:** Academic register (the ban on first person, §10.2.2.1, is an academic convention and not extracted as a finding). Points (i)-(vi) apply to advice and drafting.
- **Production responsibility affected:** drafting, review/redlining, product consistency
- **Workflow / decision implication:** Drafting/review skills should include a term-of-art collision check, an abbreviation register, a quotation-integrity check (elisions do not change meaning; source and pinpoint present), and a reporting-verb neutrality check.
- **Evaluation evidence or criterion:** No term of art used in lay sense within its field; every abbreviation defined once and used with one meaning; every altered quotation preserves the original's sense when compared to source.
- **Failure / misuse conditions:** Over-simplification that loses a term of art's precision; selective elision.
- **Repair implication:** Substitute lay synonyms; restore elided qualifiers; re-verify quotations against source.
- **Proposed disposition:** retain (drafting hygiene) — merge with stronger drafting sources.

#### FF2-22
- **ID:** FF2-22
- **Location:** ch 17, §17.3.1-17.3.6, pp. 427-429 (Figures 17.5, 17.6 at pp. 429-430); §17.1.3 The facts, pp. 420-421; §17.1.4 Case history, p. 421 (print)
- **Problem addressed:** Preparing an argument without mastering the facts or the other side's case.
- **Principle / method / heuristic (own words):** Facts before law: know the problem before researching the answer. Reduce the point to be argued to its simplest accurate form and keep it visible throughout research. Build a chronology of significant events — sequencing often exposes the key issue. Treat every fact as potentially relevant; where a fact's significance is unclear, note it and test it by asking how the problem would change if that fact were altered or absent; never ignore an ununderstood fact, because it may be the opponent's best point. Tabulate facts for and against your position in two columns, and convert the analysis into a list of research questions before researching. On appeal-type tasks the found facts are fixed: do not supplement or reinterpret them, and keep fact questions distinct from law questions. Use the reasoning of the decision below as a predictor of the opponent's argument (appellant) or as a starting platform (respondent), but do not confine the argument to it. Tie the legal argument to the particular facts rather than arguing doctrine in the abstract.
- **Assumptions and applicability:** Moot (appellate, fixed record). Chronology, counterfactual fact test, for/against table and question list transfer to any contentious or advisory analysis; "facts are fixed" applies to appellate/review contexts and to not inventing facts generally.
- **Production responsibility affected:** issue spotting, scoping, research, reasoning/applicability
- **Workflow / decision implication:** Add to the issue-spotting workflow: timeline artefact; counterfactual test on unexplained facts; two-column fact table; research-question list derived from the table.
- **Evaluation evidence or criterion:** Timeline present for date-sensitive matters; every unexplained fact has a recorded counterfactual test result; facts adverse to the client's position are listed, not omitted.
- **Failure / misuse conditions:** Importing extraneous "facts" (e.g. trade statistics) to fill gaps on a fixed record; blind spots toward adverse facts.
- **Repair implication:** Strip non-record facts; re-run for/against table.
- **Proposed disposition:** retain — the counterfactual fact test is a useful, checkable heuristic.

#### FF2-23
- **ID:** FF2-23
- **Location:** ch 17, §17.3.7 Research the law and Figure 17.8, pp. 429-431 and p. 434; §17.3.8 Using cases (17.3.8.1-17.3.8.7), pp. 431-433; §17.1.1 Level of the court, p. 418 (print)
- **Problem addressed:** Building an argument on authorities without testing their weight, status and fit.
- **Principle / method / heuristic (own words):** Research funnel: encyclopaedic statement of current law and leading sources > analytical textbooks (if the text makes the point look easy, find a deeper one; revision guides are not citable) > cases (the bulk of the work) > articles for depth on the narrow point or to extend principle where case law is silent. For every case — yours and the opponent's — run a checklist: which court decided it and how that binds the present forum; what legal issue it actually decided; what is ratio and what is merely obiter; which jurisdiction (domestic binding vs foreign/Privy Council persuasive — and if relying on persuasive authority, say so openly and explain why it helps); how it has been treated since (applied, distinguished, overruled — relying on an overruled case is described as fatal); how close its facts are (argue parallels for helpful cases, material differences to distinguish harmful ones); and cite the most authoritative report series. Record, case by case, points for and against you; adverse passages must not be ignored because the tribunal will raise them even if the opponent does not.
- **Assumptions and applicability:** English doctrine of precedent and English report hierarchy as of 2011; the specific rules of bindingness are substantive/jurisdictional (section 3). The checklist shape is portable.
- **Production responsibility affected:** research, authority verification, reasoning/applicability
- **Workflow / decision implication:** Authority-verification skill should populate, per case: court/level, binding-or-persuasive for this forum, issue decided, ratio vs obiter classification of the passage relied on, subsequent treatment check with date, factual proximity note, best citation, for/against extracts.
- **Evaluation evidence or criterion:** Every relied-on case has a completed record including a dated subsequent-treatment check; persuasive authorities are labelled as such in the output; obiter is not presented as holding.
- **Failure / misuse conditions:** Treatment check skipped; obiter or foreign authority presented as binding; opponent's authorities not checked.
- **Repair implication:** Run treatment check; relabel weight; replace overruled authority or concede the point.
- **Proposed disposition:** retain — merge with authority-verification findings from other texts.

#### FF2-24
- **ID:** FF2-24
- **Location:** ch 17, §17.4.1 Constructing submissions (single, alternative, cumulative, combined), pp. 436-437 (print)
- **Problem addressed:** How to structure an argument so that it survives rejection of one limb and is pitched at a defensible strength.
- **Principle / method / heuristic (own words):** A submission is one self-contained strand, each supported by its own authority. Options: a single submission (simple but brittle); alternative submissions (a second independent route if the first fails, e.g. a policy/common-sense argument where authority is weak or absurd in result, which may draw on foreign authority or academic writing); cumulative submissions (the point broken into smaller sub-questions each separately supported); or a combination with a fallback limb. Pitch matters: claiming that binding authority compels the result leaves no room if the tribunal disagrees; claiming that the weight of authority favours the result is more defensible.
- **Assumptions and applicability:** Advocacy setting; transfers to structuring advice on contested points, position papers and negotiation arguments. Policy arguments are, by the authors' own description, not authority-based and should be labelled accordingly.
- **Production responsibility affected:** reasoning/applicability, drafting, risk communication
- **Workflow / decision implication:** When constructing an argument, generate primary and fallback limbs, mark each limb's basis (binding authority / weight of authority / analogy / policy), and calibrate the verbal strength of each claim to that basis.
- **Evaluation evidence or criterion:** Each limb independently supported; strength words ("binding", "preponderance", "arguable") match the authority record from FF2-23; policy limbs flagged as such.
- **Failure / misuse conditions:** Overclaiming bindingness; fallback limbs that contradict the primary limb's factual premises without saying "alternatively".
- **Repair implication:** Re-pitch claim strength; add explicit alternative framing.
- **Proposed disposition:** retain.

#### FF2-25
- **ID:** FF2-25
- **Location:** ch 17, §17.3.5 Two sides to the argument, p. 428; §17.4.3 Skeleton arguments (17.4.3.1-17.4.3.3) and Extract 17.1, pp. 439-441; §17.4.4.2 Preparing the bundle, pp. 441-442; §17.5.2 Dealing with judicial interventions, pp. 444-445; §17.5.3.3-17.5.3.4, p. 447 (print)
- **Problem addressed:** Anticipating and meeting the counter-argument; candour in argument documents; handling questions one cannot answer.
- **Principle / method / heuristic (own words):** Know the opposing case as well as your own. On receiving the other side's outline: obtain and read their authorities in full; note what helps them and, more importantly, what in their cases helps you; check whether their cases are still good law; check whether they can be distinguished on the facts. A skeleton is a clear list of propositions each paired with its authorities; opaque or misleading skeletons, and listing a long case one does not intend to use in order to distract, are unethical. Include whole authorities, not fragments, in the supporting bundle; when quoting, take the reader to the exact page and passage, then explain how it applies; never quote the headnote or counsel's argument. Know for each case whether its facts matter (analogy/distinction) or whether it is cited only for a general principle. When questioned: listen, think, seek clarification or restate the question, answer when asked rather than deferring, be concise, and if unable to answer say so rather than bluffing on.
- **Assumptions and applicability:** Moot conventions; the ethics and verification points generalise to any adversarial or reviewed work product. The "say you cannot assist" rule maps to agent abstention/escalation. Note the authors elsewhere remark that good mooters can "bluff" past gaps (p. 427) — that remark should not be adopted.
- **Production responsibility affected:** authority verification, review/redlining, escalation, reasoning/applicability
- **Workflow / decision implication:** A review/adversarial skill should run the four-question audit on any counterpart's authorities; outline documents should be proposition+authority pairs with no decoy citations; agents should quote only from the judgment body with pinpoints; unanswerable queries are surfaced, not papered over.
- **Evaluation evidence or criterion:** For a counterpart document: each cited authority has a status check, a helps-them/helps-us note and a distinguishability note. For own outline: every listed authority is actually used.
- **Failure / misuse conditions:** Quoting headnotes or summaries as the court's words; padding authority lists; confident answers to questions outside the researched area.
- **Repair implication:** Remove unused authorities; replace headnote quotations with judgment passages; convert bluffed answers into flagged open questions.
- **Proposed disposition:** retain/qualify — reject the "bluff" aside.

#### FF2-26
- **ID:** FF2-26
- **Location:** ch 18, §18.1.1 Types of negotiation, pp. 452-455; §18.3.1 Analysis of the scenario, pp. 457-459 (print)
- **Problem addressed:** Negotiating to the client's stated demand without understanding why they want it, and without mapping limits on authority.
- **Principle / method / heuristic (own words):** Distinguish positional (zero-sum, suited to narrow, purely monetary disputes with no relationship to preserve) from interest-based bargaining (asks why each side wants what it wants, enabling non-obvious trades). Even a "just money" instruction should be probed for its purpose. Preparation checklist: legal area; client's express and implied wants (speed, amicability, reluctance to litigate); client's interests, found by asking "why" of each want — while guarding against false assumptions; express limits on authority and outcomes ruled out; clues to the other side's priorities; own strengths and weaknesses and how each will be handled. Two readers comparing inferences helps expose ambiguity in instructions.
- **Assumptions and applicability:** Student competition format with written instructions only; in practice the adviser asks the client. Interest-based framing draws on mainstream negotiation literature (not cited in the passages read).
- **Production responsibility affected:** scoping, risk communication, escalation, drafting (position papers)
- **Workflow / decision implication:** A negotiation-preparation skill should output a wants/interests/limits table with each interest marked "stated" or "inferred — confirm with client", plus an other-side interests hypothesis and a strengths/weaknesses list.
- **Evaluation evidence or criterion:** Every want has a recorded "why"; inferred interests are flagged for confirmation; authority limits are stated explicitly.
- **Failure / misuse conditions:** Imposing the adviser's idea of a good outcome; treating inferences as instructions.
- **Repair implication:** Return to client for confirmation of inferred interests and limits.
- **Proposed disposition:** retain/adapt.

#### FF2-27
- **ID:** FF2-27
- **Location:** ch 18, §18.3.2.1 Researching the law, pp. 459-460; §18.3.2.2 Researching the facts, pp. 460-461; §18.3.3.1-18.3.3.5 Strategy (Figure 18.7), pp. 461-465; §18.4.5 Ethical considerations, p. 470 (print)
- **Problem addressed:** Setting and defending negotiating positions on a principled basis.
- **Principle / method / heuristic (own words):** Anchor positions in the litigated alternative: ask (1) would the client win in court — anything short of a clear yes is a reason to settle, and even a clear yes leaves cost, delay and flexibility reasons; (2) what would success yield, net of cost and time — this informs the bottom line, since settling for worse than the court outcome rarely makes sense; use damages guides and analogous decided cases to support figures; (3) what happens if the agreement is breached — a negotiated deal must be genuinely acceptable to both sides and, for contract-type negotiations, should build in responses to foreseeable failures. Verify objectively any fact that can be verified rather than relying on the client's account (e.g. a client's own valuation). Fix four reference points: best negotiated outcome, best alternative to agreement (BATNA), worst acceptable outcome, worst alternative (WATNA). Break the desired outcome into discrete issues; for each set top and bottom lines; rank issues by importance to the client (which may differ from the order of discussion); plan trades of low-priority concessions for high-priority gains without breaching express instructions; generate creative options from reasonable inferences but never invented facts; put it on a one-page plan used as an aide-memoire, not a script. Ethical limit: never misstate instructions, limits or willingness to litigate, deliberately or through careless wording; persuade by reference to merits instead.
- **Assumptions and applicability:** England and Wales civil/family context, competition setting. The statement that a negotiated agreement "is not binding" (p. 460) is a substantive-law claim that is at best incomplete (see section 3) and must not be adopted. The bottom-line-equals-court-outcome heuristic ignores risk-weighting beyond the authors' brief mention of cost and time.
- **Production responsibility affected:** risk communication, scoping, research, drafting, escalation
- **Workflow / decision implication:** Negotiation-prep output should contain: litigated-alternative assessment with probability and net value; four reference points; per-issue range and priority table; concession/trade map; list of client-asserted facts with verification status; explicit authority limits; and an honesty constraint on any generated negotiating language.
- **Evaluation evidence or criterion:** All four reference points present and justified by research; each issue has range+rank; no proposed statement misrepresents instructions or alternatives; client-asserted key facts marked verified/unverified.
- **Failure / misuse conditions:** Bottom line set by client wish rather than alternative analysis; bluffing about limits; invented facts to create options.
- **Repair implication:** Recompute reference points from the litigated-alternative analysis; strip misleading language.
- **Proposed disposition:** adapt — retain structure; qualify enforceability statement and add risk-weighting.

### 3. Substantive-law statements noted (research questions only)

None of the following is adopted as a statement of current law.

1. Ch 14 worked example (pp. 355-362): who counts as an "occupier" for occupiers' liability in England and Wales, the visitor/trespasser distinction, effect of warnings, children and allurements, and exceeding permission. RQ: what are the current governing provisions and leading authorities, and are the cases the book relies on still good law?
2. Ch 14 Figure 14.6 (p. 360): the test for dishonesty in theft is presented as a two-stage objective/subjective test. RQ: what is the current test for dishonesty in English criminal law, and has the 2011 position changed? (Must be verified from current primary sources; not assessed here.)
3. Ch 14 practical exercise (p. 357): definitions of "wound" and "grievous bodily harm" and psychiatric injury under the Offences against the Person Act 1861. RQ: current position.
4. Ch 7 §7.4.4 (pp. 180-181): legal effect of codes of practice, circulars, practice directions, extra-statutory tax concessions and voluntary codes is said to be uncertain until tested. RQ: for each instrument type relevant to a matter, what is its current statutory footing and judicial treatment? Several named bodies (e.g. Press Complaints Commission, Inland Revenue, Judicial Studies Board) have since been replaced.
5. Ch 7 §7.3.5 (p. 179): Law Commission Act 2009 reporting duty; proportion of recommendations implemented. RQ: current position.
6. Ch 8 §8.4.1 (pp. 197-199): scope of the Olympics association right under the Olympic Symbol etc (Protection) Act 1995 and remedies. RQ: current law on protected Olympic marks/words in the UK.
7. Ch 10 §10.2.2.2 (p. 241): masculine includes feminine under Interpretation Act 1978 s 6. RQ: current drafting convention and statutory interpretation rule.
8. Ch 17 §17.1.1 and §17.3.8 (pp. 418, 431-432): bindingness of House of Lords/Supreme Court decisions on the Court of Appeal; Court of Appeal's self-binding rule and exceptions; status of Privy Council decisions as persuasive; binding effect of ECJ decisions. RQ: current rules of precedent in England and Wales, including post-2011 developments on Privy Council authority and on EU case law after UK withdrawal.
9. Ch 17 sample moot (pp. 419, 429-433): advertisement as offer vs invitation to treat; whether the postal rule or the instantaneous-communication rule governs acceptance by email; revocation before acceptance. RQ: current English contract law on formation by electronic communication.
10. Ch 17 Figure 17.7 (p. 433): hierarchy of law report series for citation. RQ: current practice direction on citation of authorities.
11. Ch 18 §18.3.2.1 (p. 460): statement that a negotiated settlement "is not binding". RQ: when is a negotiated settlement a binding contract or embodied in a consent order, and what are the enforcement routes?
12. Ch 18 introduction (p. 451): roughly 90 per cent of civil and family disputes settle without trial. RQ: current, sourced figure if needed.
13. Ch 18 scenario (pp. 458-459): law on child contact arrangements and the legal position of transgender parents. RQ: current family-law framework and terminology ("access" is outdated).
14. Ch 11 intro (p. 267): plagiarism findings reportable to professional bodies as character issues. RQ: current regulator (SRA/BSB) character and suitability rules.

### 4. Material the author marks as contested, or where the author criticises other approaches

- Criticism of using IRAC-type mnemonics as a four-part document layout rather than a per-sub-issue cycle (ch 14 §14.2.1, p. 348).
- Criticism of "lazy application" and of abdicating the conclusion to court or jury (ch 14 §14.5.1.1, p. 359); of bracket-citation without stated principle (§14.5.2.3, p. 362); of fusing rule and application to save words (§14.4.3.2, p. 357).
- The authors insist there is usually no single right answer in law, only stronger and weaker arguments (ch 14 §14.6, p. 363).
- Criticism of reliance on cases-and-materials extracts as producing "blinkered" research (ch 7 §7.1.2, pp. 172-173), of revision guides and A-level-type web summaries as sources (ch 7 §7.1.7 p. 175; ch 12 §12.3.5.5 p. 314), and of quotation-heavy writing sourced from textbooks (ch 10 §10.5, pp. 257-258).
- Relative weight of academic vs practitioner journals: ch 7 §7.2.5 (pp. 176-177) ranks academic higher; ch 17 §17.3.9.1 (p. 435) concedes the preference is a generalisation depending on the judge. Internally in tension; treat as contested.
- "Common knowledge" exception to citation: the authors state that experts disagree on its scope and offer only rough quantity/ubiquity tests (ch 11 §11.1.1.2, pp. 271-272).
- Positional bargaining is reported as criticised for failing on non-monetary and multi-issue disputes; the authors favour interest-based bargaining even in apparently financial disputes (ch 18 §18.1.1, pp. 453-455).
- Gender-neutral drafting vs masculine-includes-feminine convention described as a matter on which academics differ (ch 10 §10.2.2.2, pp. 241-242).
- Order of preparation (facts first vs law first) acknowledged as a matter on which mooters differ; authors prefer facts first (ch 17 §17.3.1, p. 427).
- Unethical skeleton practices (opaque submissions, decoy authorities) condemned (ch 17 §17.4.3.3, p. 441); misrepresentation of limits in negotiation condemned (ch 18 §18.4.5, p. 470).
- Examiner's own caution: the Halsbury's worked example (ch 8, pp. 197-199) reaches firm advice to the hypothetical client before the update check is mentioned; and ch 17 p. 427 casually approves of "bluffing" past knowledge gaps. Neither should be modelled.

### 5. Content in the assigned range that is out of scope for legal production (and why)

- Ch 9 Study skills (print 207-236): lectures, seminars, note-taking, working with lecturers/students, time management, personal development planning — student learning logistics.
- Ch 10 §10.2.2.1 first-person prohibition, §10.3 grammar and punctuation, §10.4 paragraph formula (topic/expansion/illustration/link — marginally useful, general writing), §10.6.2-10.6.3 word-limit penalties, §10.7 presentation — academic conventions and general English.
- Ch 11 plagiarism definitions, motives, detection and sanctions (§11.1.2); OSCOLA and Harvard formatting mechanics (§11.3-11.4) — institution-specific and style-edition-specific (OSCOLA 4th edn 2010). Only the when/why-to-cite and pinpoint logic was extracted.
- Ch 12 essay-question analysis, brainstorming, essay structure and writing (§12.1-12.2, 12.4-12.5); Bloom's taxonomy discussion — academic essay craft. Only research-trail and supporting-material guidance extracted.
- Ch 13 Dissertations: topic choice, proposals, milestones, supervision, writing process — academic project management. §13.5's list of wider source types (case commentaries, monographs, newspapers for unreported first-instance decisions, interest-group literature with a bias warning) adds little beyond ch 7.
- Ch 15 Revision and examination skills; Ch 16 Presentation skills (topic choice, visual aids, delivery, nerves) — headings only; student assessment technique.
- Ch 17 moot roles, order of speeches, courtroom etiquette, modes of address, oral citation convention, speech "housekeeping", not reading from a script, bundle tabbing — advocacy performance and competition rules.
- Ch 18 parent/child bargaining illustrations, competition format, introductions, agenda-setting, deadlock-breaking, teamwork, post-negotiation reflection — live-negotiation conduct (largely not read) rather than preparation of positions.
- Ch 8 tool detail: library catalogues (Copac), Current Law Monthly Digest, journal abbreviation tables, database coverage table, Command Paper series/abbreviations, Bill citation format, Hansard column referencing, 2010-era URLs — dated tooling; only method retained (FF2-19).

### 6. Candidate benchmark cases suggested by the text (own words, synthetic)

1. **Multi-claimant premises scenario with a bystander and a contractor.** A small visitor attraction; three injured people (an adult who could not read a warning, a child who entered a cordoned area against a relative's instruction, an employee hurt by faulty work done by an independent tradesperson). Instruction limits advice to one statutory head and excludes general negligence. Tests: party/event matrix including non-party actors; element-by-element sub-issues including warnings and defences; scope discipline with a separate flag for the excluded head; three-level consistent conclusions (FF2-02, -03, -04, -06, -13).
2. **Missing-fact penalty rule.** A simple tiered late-filing penalty rule with "good cause" and "prior permission" exceptions; facts give the filing time but say nothing on either exception. Pass requires: general rule applied first; binary gap handled briefly; open-textured "good cause" explored with two contrasting hypotheticals; contingent conclusion naming what would change it; question to client; no invented fact (FF2-10, -13).
3. **Lazy-application detector.** Provide a draft analysis containing "clearly satisfied on the facts", "a matter for the tribunal", and a case name in brackets with no principle. Pass requires the reviewer to flag all three, rewrite each with fact-to-element mapping, a tentative prediction, and a principle-plus-linkage sentence (FF2-09, -12).
4. **Rule/application separation.** Give five sentences mixing abstract rules and fact-laden "rules" (e.g. "the relevant standard is that of an experienced surgeon"). Pass requires correct classification and rewriting of the fact-laden ones as abstract rule followed by application (FF2-08).
5. **Secondary-source laundering.** Research pack contains a textbook paragraph summarising a case and an article summarising another article; the underlying primary sources are available but unread. Pass requires: no primary proposition cited to the textbook; article cited "as discussed in" unless the original is retrieved; pinpoints for any quotation; source-type tags and edition dates (FF2-15, -16, -20).
6. **Currency layering.** A base commentary paragraph (dated) states a rule; a later supplement entry narrows it; a most-recent update notes a reversing decision. Pass requires consulting all layers in order, reporting the current position with "current to" dates, and not advising from the base text alone (FF2-19).
7. **Authority audit of an opponent's outline.** Opponent's skeleton lists four authorities: one overruled, one foreign decision presented as binding, one where the relied-on passage is obiter, one sound but factually distant. Pass requires status check, correct weight labels, distinguishing note, and identification of any passage that helps our side (FF2-23, -25).
8. **Argument structuring under weak authority.** Point where domestic authority leans against the client but a foreign appellate decision and academic commentary support them. Pass requires cumulative limbs where possible, an explicit alternative policy limb labelled as such, persuasive authority disclosed as persuasive, and claim strength pitched at "weight of authority"/"arguable", not "binding" (FF2-24).
9. **Counterfactual fact test.** Scenario includes an apparently idle detail (e.g. a stated finite stock quantity in an advertisement). Pass requires the agent to flag the unexplained fact, test how the analysis changes if the fact is removed, and identify which side it favours (FF2-22).
10. **Soft-law status labelling.** Advice draws on a statute, a statutory code of practice, a regulator's guidance note and an industry voluntary code. Pass requires a status label and basis for each instrument and wording that does not present guidance as binding law (FF2-18).
11. **Negotiation preparation pack.** One-sided written instructions with a money demand, an unstated underlying need discoverable by asking "why", an express floor, a client-asserted valuation that is objectively checkable, and multiple issues of differing priority. Pass requires wants/interests/limits table with inferred items flagged for confirmation; litigated-alternative assessment; four reference points; per-issue ranges and ranking; trade map; verification flag on the valuation; and no proposed language that misstates the floor or willingness to litigate (FF2-26, -27).
12. **Web-source screen.** Three web results: an official publisher of legislation, an anonymous legal-summary site, and a community encyclopaedia entry. Pass requires only the official source to support a legal proposition, the others used (if at all) as leads, with access dates and retained copies (FF2-17).

---

