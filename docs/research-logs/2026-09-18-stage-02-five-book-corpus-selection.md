# Stage 2 — Five-Book Legal Corpus Selection

**Stage:** 2 of the Legal Skills bootstrap (v1.2)  
**Date:** 18 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — corpus revision 1 accepted (see §7). Source-access needs for S7 and S8 remain open for Stage 3.  
**Governing section:** §8 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Family rule applied:** `production-skills/docs/bootstrap/domain-research-process.md` §1–§2  
**Seed input:** `2026-09-18-stage-01-domain-boundary.md`

---

## 1. Supplied-source inventory

Method: local read of `books/**/*.pdf` with `pypdf` on 18 September 2026. No file was uploaded to an external service. Metadata comes from the documents (title page, copyright page, PDF properties), not from filenames. Bibliographic facts for S4–S8 were cross-checked by `WebSearch` against publisher and bookseller listings (search-result level).

| ID | Work | Edition / year (from document or listing) | Local identifier | Pages in file | What the file is |
| --- | --- | --- | --- | --- | --- |
| S1 | Kenneth A. Adams, *A Manual of Style for Contract Drafting* | 4th ed., ABA, © 2017, ISBN 978-1-63425-964-4 | `books/A_Manual_of_Style_for_Contract_Drafting_-_Kenneth_Adams.pdf` | 983 | Full book text |
| S2 | Emily Finch and Stefan Fafinski, *Legal Skills* | 3rd ed., OUP, © 2011 | `books/Legal_Skills_-_Stefan_Fafinski.pdf` | 508 | Full book text |
| S3 | Frederick Schauer, *Thinking Like a Lawyer: A New Introduction to Legal Reasoning* | Harvard UP, 2009 | `books/Thinking_Like_a_Lawyer_-_Frederick_Schauer.pdf` | 256 | Full book text |
| S4 | Emily Allbon with Ian Hunter (consultant ed. Peter Clinch), *Legal Research: A Practitioner's Handbook* | 3rd ed., Wildy, Simmonds & Hill, 2019 | `books/Research- A Practitioner’s Handbook, 3rd ed. (2019).pdf` | 2 | A two-page summary of the book. Not the book. |
| S5 | A. Masson, H. Bouthinon-Dumas, J.-M. Do Carmo Silva, W. G. Voss (eds), *The Oxford Handbook of Law and Management* | OUP, 2026, ISBN 9780197769034 | `books/The Oxford Handbook of Law and Management  (1).pdf` | 2 | A two-page summary of the book. Not the book. |
| S6 | Tina L. Stark and Monica L. Llorente, *Drafting Contracts: How and Why Lawyers Do What They Do* | 3rd ed., Aspen, 2024 | `books/drafting-contracts-expanded-overview (2).pdf` | 19 | A chapter-by-chapter overview (about 3,100 words). Not the book. |
| S7 | Richard Moorhead, Steven Vaughan, Cristina Godinho, *In-House Lawyers' Ethics: Institutional Logics, Legal Risk and the Tournament of Influence* | Hart, 2018 (paperback 2021) | `books/in-house-lawyers-ethics-expanded-overview (1).pdf` | 15 | A chapter-by-chapter overview (about 2,600 words). Not the book. |
| S8 | Matthew Whalley and Chris Guzelian, *The Legal Risk Management Handbook* | Kogan Page, 2016 | `books/legal-risk-management-handbook-expanded-overview.pdf` | 14 | A chapter-by-chapter overview (about 2,400 words). Not the book. |

Findings:

1. **Eight works are supplied.** The corpus must hold exactly five. Excluding any supplied work from the foundational five needs explicit user approval.
2. **Only S1, S2 and S3 give direct access to the book.** S4–S8 are secondary material. Under the governing rules a summary cannot stand in for direct extraction. The overviews were read in Stage 2 only to understand each book's likely contribution.
3. **Edition currency.** S1 is the 4th edition; a 5th edition was published in 2023 (about 70 pages of new material per the ABA listing). S2 is the 3rd edition (2011); the 10th edition was published in 2025. The supplied editions are retained as supplied. The age of S2's database and EU-law material is a recorded reading limitation.

---

## 2. Legal-production knowledge-coverage map

Dimensions come from the Stage 1 boundary (owned outcomes, quality definition), not from the supplied books.

| # | Responsibility | Depth needed | Provisional coverage from supplied works | Gap after supplied works |
| --- | --- | --- | --- | --- |
| D1 | Matter scoping and issue spotting | High | S2 ch 14 (problem-solving: issues, rules, application, conclusion); S4 Part A (summary only) | Practitioner intake practice → Stage 4 |
| D2 | Legal research method and source hierarchy | High | S2 Part I (legislation, cases, secondary sources; finding and using); S4 (summary only); S3 ch 4 (authority) | S2 tools are 2011-era; current official sources and citators → Stages 4, 5, 11 |
| D3 | Legal reasoning and applicability | High | S3 whole book (rules, precedent, authority, analogy, statutory interpretation, rules vs standards, law and fact); S2 ch 3, 6 | US-leaning; UK/EU interpretive method cross-check → Stage 4 |
| D4 | Drafting | High | S1 whole book (categories of contract language, ambiguity, defined terms, structure); S6 (overview only: deal-to-concept translation, contract parts) | Consumer-facing and notice-style documents (privacy notices, terms) are not contract drafting between businesses → Stage 4 |
| D5 | Review and redlining | Medium–High | S6 ch 28 (overview only); S1 usage rules as review criteria | Review workflow evidence is thin without S6 full text |
| D6 | Legal risk, uncertainty and communication | High | S8 (overview only: definition of legal risk, taxonomy, register, appetite, reporting, probability language); S7 (overview only: how "legal risk" framing is used in practice) | Calibrated language evidence → Stages 4, 9 |
| D7 | Professional judgement, independence, escalation, human review | High | S7 (overview only: empirical study of in-house decisions, pressure, ethical infrastructure, escalation routes) | AI-specific supervision duties → Stage 1 seed + Stage 4 |
| D8 | Legal operations / product-counsel practice | Medium | S5 (summary only: legal astuteness, proactive law); S7, S8 partially | Product-counsel workflow is mainly article-level evidence → Stage 4 |
| D9 | Requirement traceability and change impact | High | None | **No supplied book covers this.** Reconnaissance found mainly research papers (legal requirements engineering; regulatory traceability), not foundational books → Stage 4, Stage 8 |
| D10 | Confidentiality and privilege in tool use | Medium | None directly | → Stage 10 |

---

## 3. Candidate comparison

### 3.1 Supplied works

| ID | Relevance | Adds to corpus | Practical contribution | Credibility / caution | Perspective | Currency / durability | Access |
| --- | --- | --- | --- | --- | --- | --- | --- |
| S1 Adams | D4, D5 | Sentence-level drafting discipline no other work gives | Categories of contract language; ambiguity sources; usage rules usable as review checks | Widely used practitioner reference; US-centred; prescriptive and sometimes contested style positions | Strongly prescriptive | Durable method; 4th ed. superseded by 5th (2023) | Full text |
| S2 Finch & Fafinski | D1, D2, D3 | UK source system and research procedure; structured problem-solving | Finding/using legislation and cases; precedent; problem-question method | OUP student text; academic skills chapters (essays, exams, mooting) are out of scope | Pedagogic, UK | Method durable; databases, EU material and court structure notes dated (2011) | Full text |
| S3 Schauer | D3, D2 | Theory of how rules, precedent and authority actually constrain | Binding vs persuasive authority; holding vs dicta; rules vs standards; law vs fact; realist challenge | Leading scholar; Harvard UP; US common-law focus | Critical and sceptical contrast to S2's procedural view | Durable | Full text |
| S4 Allbon | D1, D2 | Practitioner research workflow; source-by-source use guidance; court directions on research | Problem analysis; source selection; presenting results | Established UK practitioner handbook | Practitioner, UK + EU + international | 2019; source details change | **Secondary only** |
| S5 Oxford Handbook L&M | D8 | Law as a managed organisational capability | Legal astuteness; proactive law; legal knowledge management | New OUP handbook; academic; large edited volume, uneven relevance | Strategic / instrumental view of law | 2026, current | **Secondary only** |
| S6 Stark & Llorente | D4, D5 | Translating a deal into contract concepts; review and comment process; AI-use ethics (per overview) | Building-block taxonomy; drafting process; review method | Standard US teaching text | Process view; complements S1's language view | 2024, current | **Secondary only** |
| S7 Moorhead et al. | D6, D7 | Only empirical work in the pool; shows how pressure distorts legal-risk advice | Evidence for escalation routes, independence safeguards, ethical infrastructure | Peer-reviewed empirical study; UK; self-report limits noted by the authors (per overview) | Critical of the profession's self-image | 2018; durable findings | **Secondary only** |
| S8 Whalley & Guzelian | D6 | Operational legal-risk framework | Definition, taxonomy, register, appetite, controls, reporting; argues for probability language | Practitioner + academic authors; financial-services flavour | **Contrasts** with the bootstrap's "no single score" default — useful tension | 2016; durable framework | **Secondary only** |

### 3.2 Wider candidate pool (not supplied)

Researched by `WebSearch`, 18 September 2026, at listing level. None has been examined.

| Candidate | Would serve | Why not proposed for the five |
| --- | --- | --- |
| J. Holland and J. Webb, *Learning Legal Rules* (OUP, 11th ed.) | D2, D3 | Overlaps S2 + S3, which are supplied and accessible |
| W. Twining and D. Miers, *How to Do Things with Rules* (CUP) | D3 | Overlaps S3 |
| P. Rylance, *Writing and Drafting in Legal Practice* (OUP) | D4 (advice letters, memoranda, reports) | Useful for advice-writing; supplement in Stage 4 |
| B. W. Heineman Jr., *The Inside Counsel Revolution* (ABA, 2016) | D7, D8 | Overlaps S7; normative rather than empirical |
| P. Butt, *Modern Legal Drafting* (CUP) | D4 | Overlaps S1 |
| Research literature on legal requirements engineering and regulatory traceability (for example Breaux; Springer chapters) | D9 | Papers and theses, not books. Must not be counted as books. Use in Stage 4 / Stage 8. |

With eight works already supplied, adding any non-supplied book would force the exclusion of a fourth supplied work. No non-supplied book is proposed. The pool stays available to Stage 4.

---

## 4. Proposal A (recommended) — APPROVED

Foundational five:

| Slot | Work | Intended contribution | Access now |
| --- | --- | --- | --- |
| 1 | S1 Adams, *MSCD* 4th ed. | Drafting and review language discipline (D4, D5) | Full text |
| 2 | S2 Finch & Fafinski, *Legal Skills* 3rd ed. | UK source system, research procedure, structured problem-solving (D1, D2) | Full text |
| 3 | S3 Schauer, *Thinking Like a Lawyer* | Reasoning, authority, applicability, law vs fact (D3) | Full text |
| 4 | S8 Whalley & Guzelian, *Legal Risk Management Handbook* | Risk definition, taxonomy, reporting, uncertainty language (D6) | Secondary only — **full text needed** |
| 5 | S7 Moorhead, Vaughan & Godinho, *In-House Lawyers' Ethics* | Professional judgement, independence, escalation, human review (D6, D7) | Secondary only — **full text needed** |

Excluded from the foundational five and kept as **supplementary** (needs approval):

| Work | Reason | Loss | Mitigation |
| --- | --- | --- | --- |
| S4 Allbon | D1/D2 are already served by S2, which is accessible in full | Practitioner-level research workflow; more current sources | Stage 4 research; may be used as supplementary if full text appears |
| S6 Stark & Llorente | D4 is served by S1; a second drafting book would leave D6 or D7 without a book | Deal-to-concept translation; review/comment process (D5) | Stage 4 must cover review workflow; supplementary use if full text appears |
| S5 Oxford Handbook | Least connected to owned production responsibilities; strategy-level | Legal-operations framing (D8) | Stage 4 professional-practice research |

Why this combination: it is the only five that puts one book on each high-depth dimension D1–D7 except D5, and it includes one critical voice (S3) and one empirical study (S7).

## 5. Proposal B (alternative) — not chosen

Same as A, but **S6 Stark & Llorente replaces S7 Moorhead et al.**

- Gain: two complementary drafting books (language + process); D5 review workflow gets book-level evidence.
- Loss: no book-level evidence on independence, pressure and escalation (D7). That would rest on Stage 4 research alone.
- Access: S6 is also secondary only. Proposal B needs the same number of full texts as A.

## 6. Source-access register (current)

| Work | Access status | Material actually examined in Stage 2 | Reading limitation |
| --- | --- | --- | --- |
| S1 | full text available | Copyright page; table of contents (front matter pages) | Not yet read for extraction |
| S2 | full text available | Copyright page; preface; "new to this edition"; outline and detailed contents | Not yet read for extraction; 2011 edition |
| S3 | full text available | Title and copyright pages; contents | Not yet read for extraction |
| S4 | secondary material only | Supplied 2-page summary | Summary of unknown authorship; cannot support extraction |
| S5 | secondary material only | Supplied 2-page summary | Same |
| S6 | secondary material only | Supplied overview: headings and closing section | Same |
| S7 | secondary material only | Supplied overview: headings, opening pages and closing section | Same |
| S8 | secondary material only | Supplied overview: headings, opening pages and closing section | Same |

Consequence for Stage 3: extraction cannot be completed for any selected work whose status is "secondary material only". Selection may close with this need recorded. Stage 3 will stop at that work with an exact missing-source blocker unless the full text is present under `books/`.

## 7. Approval decisions

| # | Decision required | Status | Date | Reference |
| --- | --- | --- | --- | --- |
| A1 | Approve the foundational five (Proposal A or B) and the demotion of the other three supplied works to supplementary | **Approved: Proposal A.** S4 Allbon, S5 Oxford Handbook and S6 Stark & Llorente become supplementary sources. | 18 Sep 2026 | User answer to the `/bootstrap` approval question, session of 18 Sep 2026 |
| A2 | Source-access route for selected works that are summary-only | **Decided: the user will add full-text PDFs** of S7 and S8 under `books/`. No replacement is authorised. | 18 Sep 2026 | Same |

Only the approved change was applied. No supplied work was removed or replaced. No non-supplied book was added.

### Corpus revision 1 (accepted 18 September 2026)

| Slot | Work | Origin | Status |
| --- | --- | --- | --- |
| 1 | S1 Adams, *A Manual of Style for Contract Drafting*, 4th ed. (2017) | Supplied | Retained — full text available |
| 2 | S2 Finch & Fafinski, *Legal Skills*, 3rd ed. (2011) | Supplied | Retained — full text available |
| 3 | S3 Schauer, *Thinking Like a Lawyer* (2009) | Supplied | Retained — full text available |
| 4 | S8 Whalley & Guzelian, *The Legal Risk Management Handbook* (2016) | Supplied | Retained — **secondary material only; full text to be supplied by the user** |
| 5 | S7 Moorhead, Vaughan & Godinho, *In-House Lawyers' Ethics* (2018) | Supplied | Retained — **secondary material only; full text to be supplied by the user** |
| — | S4 Allbon; S5 Oxford Handbook; S6 Stark & Llorente | Supplied | Demoted to supplementary with approval A1 |

Later changes to this corpus must follow the same permission rules and must identify affected extraction and design work.

## 8. Remaining knowledge gaps (independent of the decision)

- D9 traceability and change impact: no book in the pool. Stage 4 and Stage 8 must carry this.
- D10 confidentiality and privilege in tool use: Stage 10.
- Consumer-facing document drafting (notices, terms): Stage 4.
- Non-UK professional-boundary rules: Stage 1 Q2.
- S2 currency: all tool and source details must be re-verified in Stages 5 and 11.

## 9. Exit check

| Exit requirement | State |
| --- | --- |
| Coverage map | Done (§2) |
| Candidate comparison | Done (§3) |
| Exactly five books selected | Done (§7, corpus revision 1) |
| Substitution / exclusion decisions resolved | Done (A1 approved; A2 decided) |
| Source-access needs explicit | Done (§6, §7): full text of S7 and S8 is required before Stage 3 can complete |
| Remaining gaps explicit | Done (§8) |
