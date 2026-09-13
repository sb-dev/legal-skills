# Stage 02: Complementary five-book corpus selection

**Status:** Complete for Stage 2; supplied sources recorded, Stage 3 access gaps remain  
**Version:** 1.1  
**Date:** 13 September 2026  
**Bootstrap:** [Legal Skills bootstrap v1.2, Stage 2](2026-09-08-legal-skills-new-project-bootstrap-process.md#8-stage-2--select-the-complementary-five-book-legal-corpus)  
**Input:** [Stage 01: Project charter and legal-production boundary](2026-09-12-stage-01-domain-boundary.md)  
**Execution branch:** `feat/bootstrap-2`

## 1. Decision and evidence boundary

Select these five distinct foundational works:

1. **Legal Skills** — Emily Finch and Stefan Fafinski, 10th edition, 2025.
2. **Thinking Like a Lawyer: A New Introduction to Legal Reasoning** — Frederick Schauer, 2009.
3. **Drafting Contracts: How and Why Lawyers Do What They Do** — Tina L. Stark and Monica L. Llorente, 3rd edition, 2024.
4. **The Legal Risk Management Handbook: An International Guide to Protect Your Business from Legal Loss** — Matthew Whalley and Chris Guzelian, 1st edition, 2016.
5. **In-House Lawyers' Ethics: Institutional Logics, Legal Risk and the Tournament of Influence** — Richard Moorhead, Steven Vaughan and Cristina Godinho, first edition, originally 2018; 2021 paperback identified below.

The set combines practical legal methods, a deeper account of reasoning, transactional production, organisational risk practice and an empirical critical perspective. The original selection followed comparison with three additional books. It does not allocate one skill to each book or settle the eventual capability architecture.

**Supplied-source update:** The user subsequently supplied eight files representing these five works and three complementary works. All are retained. The [source-intake addendum](2026-09-13-stage-02-supplied-source-intake.md) records the files, editions, contributions and summary limitations. The foundational five remain selected; Adams, the practitioner research handbook and the Oxford law-and-management handbook are supplied complements. Sections 6 and 8 below reflect current access and provenance.

The execution baseline is the Stage 1 commit, [`3c514e2`](https://github.com/sb-dev/legal-skills/commit/3c514e27428b962ef312c90fed99eff219d5ce33). The governing [Production Skills domain research process](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/bootstrap/domain-research-process.md) was re-examined at revision `20979e0c68ac4b37433374df7fe10ceb2e7ee69a`; its separation of selection, direct examination and wider challenge remains applicable. No corpus is imported from another branch.

The original selection examined bibliographic records, publisher descriptions, contents pages, limited book front matter or chapter openings, and one author-written companion article. Subsequent intake checked the supplied files and relevant publisher records as detailed in the addendum. These support a **selection and intake judgement**, not extracted production rules. Descriptions of intended usefulness, comparative advantages and gaps below are project assessments from that bounded evidence. They remain subject to direct examination in Stage 3. No selected book has yet been meaningfully examined across its intended contribution.

No books were supplied at the original selection. All five foundational choices were selected additions. The later request expressly adds complementary sources, so retaining the three additional works in that role requires no exclusion or substitution decision. No supplied work is removed or demoted.

## 2. Coverage map derived from Stage 1

The unit of work remains a bounded legal matter for software, digital products or creative production. England and Wales is the initial positive proving jurisdiction; UK-wide rules apply only where their actual scope supports that treatment. The books supply reusable methods. Current law, territorial applicability and the consumer's facts require separate evidence.

| Required knowledge | Depth needed from the research foundation | Production use and limit |
|---|---|---|
| Matter scoping and issue spotting | A repeatable way to distinguish the requested decision, material facts, missing facts and legal questions | Support an inspectable matter brief and recognise when the question exceeds competence or scope. |
| Research and source hierarchy | Practical source discovery plus reasons for treating sources as authoritative, persuasive or merely explanatory | Support reproducible authority research. Database operation, current status and temporal validity need later primary-source verification. |
| Reasoning and applicability | Depth on rules, precedent, interpretation, analogy, factual distinctions and uncertainty | Connect an authority to the particular question; expose the reasoning for review. |
| Drafting and legal-product consistency | Methods for translating intent and obligations into clear, internally coherent text | Connect documents to actual conduct. A contract drafting method alone cannot validate a product's disclosures or implementation. |
| Review, redlining and repair | Practical diagnosis, explanation and bounded amendment | Preserve approved work while locating defects and explaining the effect of changes. |
| Risk and uncertainty communication | Distinguish legal constraints, interpretive uncertainty, exposure, missing evidence and business choices | Produce actionable options without a single score or an unsupported compliance conclusion. |
| Organisational judgement and escalation | How legal work reaches accountable decision makers, and how organisational incentives can distort it | Prepare review and specialist handoffs. Legal Skills does not acquire professional status or decision authority. |
| Requirement traceability and change impact | Link facts, legal propositions, requirements, documents and implementation evidence; identify dependencies affected by change | Assess legal consequences. Implementation and lifecycle orchestration remain with the consuming project. |
| Quality and evidence discipline | Ways to test reasoning, document choices, recognise defects and challenge a proposed answer | Inform later evaluation design; textbook exercises or professional reputation do not demonstrate agent reliability. |

These dimensions overlap. None requires a dedicated book slot. The map deliberately includes traceability and change impact even though the selected corpus offers only partial coverage: a convenient selection must not erase an owned responsibility.

## 3. Candidate comparison

The original comparison is qualitative. No numerical scores or coverage percentages are inferred from contents pages. Publication details and access observations were checked on 13 September 2026. The evidence links in sections 4 and 7 identify what was inspected for selection. The later supplied-source comparison is in the addendum; the three additions remain retained complements.

| Candidate | Contribution assessed against the boundary | Main limitation or overlap | Selection decision |
|---|---|---|---|
| B1 — Finch and Fafinski, *Legal Skills*, 10th ed. (2025) | Broad practical anchor for finding and using legal materials, problem analysis and written work | Introductory and student-oriented; substantial study and assessment material is outside our intended reading scope | **Select.** Supplies the practical context needed to connect the other, narrower works. |
| B2 — Schauer, *Thinking Like a Lawyer* (2009) | Concentrated conceptual treatment of legal reasoning | Overlaps B1's introductory reasoning; does not provide an operational research service or current English law | **Select.** Retain depth on justification alongside practical procedure. |
| B3 — Stark and Llorente, *Drafting Contracts*, 3rd ed. (2024) | Connects transaction design, language, drafting process, review and amendments | Transactional and substantially US-oriented; cannot stand for all legal writing or consumer-facing documents | **Select.** Broadest production contribution among the contract-writing candidates examined. |
| B4 — Whalley and Guzelian, *The Legal Risk Management Handbook*, 1st ed. (2016) | Connects legal issues with organisational assessment, mitigation and reporting | Corporate orientation; methods for measuring risk require challenge; substantive examples age | **Select.** Adds decision and organisational context to analysis and drafting. |
| B5 — Moorhead, Vaughan and Godinho, *In-House Lawyers' Ethics* (2018; paperback 2021) | Empirical challenge to assumptions about independence, commercial alignment and legal risk | Study of human in-house practice; neither a workflow manual nor evidence about agent behaviour | **Select.** Provides a distinct critical perspective on how advice can be distorted. |
| A1 — Kenneth A. Adams, *A Manual of Style for Contract Drafting*, 5th ed. (2023) | Detailed language choices and critique of inherited drafting habits | Strong complement to B3, but a narrower addition than organisational judgement within five slots | **Not foundational.** The subsequently supplied fourth edition (2017) is retained as complement S1; see the addendum. |
| A2 — David W. Tollen, *The Tech Contracts Handbook*, 3rd ed. (2021) | Practical treatment of technology agreements close to likely consumer projects | Concentrates on an agreement category; would duplicate part of B3 while narrowing the foundation | **Do not select as foundational.** Reconsider for evidenced technology-contract needs. |
| A3 — Michelle Finneran Dennedy, Jonathan Fox and Thomas R. Finneran, *The Privacy Engineer's Manifesto*, 1st ed. (2014) | Policy-to-engineering translation, lifecycle work and verification | Strong relevance to one gap, but privacy-specific and partly in engineering's ownership | **Do not select as foundational.** Retain as a candidate for the traceability gap investigation. |

The comparison concerns the contribution of each work to this five-book foundation. It does not declare the rejected alternatives inferior books or approve them as future packs.

## 4. Selected corpus and intended examination

### B1 — Legal Skills

**Identity:** Emily Finch and Stefan Fafinski; 10th edition, 2025; Oxford University Press. Print ISBN **9780198924722**. Origin: **selected addition**. OUP's [edition-specific resource page](https://learninglink.oup.com/access/finch10e) confirms the work and authors. The [Wildy bibliographic record and contents listing](https://www.wildy.com/isbn/9780198924722/legal-skills-10th-ed-paperback-oxford-university-press) identify the print edition and year.

**Intended contribution:** Examine how to find, read and use legal sources, organise a problem and produce supported written work. This is the practical research-and-analysis anchor against which specialist contributions can be connected. The visible contents include legislation, cases, other legal materials, reasoning, writing and drafting. The retailer's listing is incomplete, so it is not a reliable basis for exhaustive chapter numbering.

**Credibility and limits:** An established university-press teaching text offers an organised introduction, not proof of sufficient professional or autonomous competence. Student assessment, revision, mooting and employability material does not define our production boundary. Its recent edition is useful for orientation, but no cited law or research interface becomes current merely because the book is recent.

**Stage 3 reading target:** Source discovery and use, reasoning, problem analysis, referencing and practical drafting. Confirm locations against the actual tenth edition. Record when a student exercise fails to address a production decision, source-status check or review requirement.

### B2 — Thinking Like a Lawyer: A New Introduction to Legal Reasoning

**Identity:** Frederick Schauer; original work, 2009; Harvard University Press. Selected source identifier: ebook ISBN **9780674054561**, [publisher record on JSTOR](https://www.jstor.org/stable/j.ctvjk2x3k). Origin: **selected addition**. A later paperback format does not count as a separate work.

**Intended contribution:** The contents and short openings identify rules, precedent, authority, analogy, statutory interpretation and questions about legal reasoning's explanatory force. Examine how those methods justify a conclusion and where they fail. This is the depth complement to B1's practical introduction.

**Credibility and limits:** A scholarly conceptual treatment can challenge mechanical rule application. It is not a research operations manual, current authority or a sufficient account of the initial jurisdiction. Distinguish transferable reasoning from jurisdiction-dependent examples. Its age is less concerning for conceptual questions than for substantive legal propositions.

**Stage 3 reading target:** The identified reasoning topics and their counterarguments. Ask what evidence would reveal an invalid analogy or an unjustified authority choice in our work; do not infer an evaluation rule from the contents alone.

### B3 — Drafting Contracts: How and Why Lawyers Do What They Do

**Identity:** Tina L. Stark **and Monica L. Llorente**; 3rd edition, 2024; Aspen Publishing. Print-plus-ebook ISBN **9781543803907**; ebook ISBN **9781543845976**. Origin: **selected addition**. The [publisher record](https://aspenpublishing.com/products/stark-draftingcontracts3) names both authors and dates this edition to 27 February 2024.

**Intended contribution:** Examine the translation from a business arrangement to contract structure and language, then the workflow for drafting, reviewing and changing it. The [third-edition contents](https://assets.ctfassets.net/exvcr1lfm0et/5aHeDlmwrlPS3ZwBrcfhgh/8a5dc0d0b99cfb9bdcd6a06f4c072097/Drafting_Contracts_3e_TOC.pdf) provide identifiable reading targets: contract concepts and drafting, clarity, the drafting process, review and comments, amendments, and professional responsibility. The [preface](https://assets.ctfassets.net/exvcr1lfm0et/5EkCE2fAXm7ARZwrGTxqhm/9620abf842b3dc00ca5b86e3e1dce341/Drafting_Contracts_3e_Preface.pdf) describes the edition's structure; it is not a substitute for those chapters.

**Credibility and limits:** The teaching design joins explanation and exercises, making it a promising source of work that can be inspected. Direct examination must test that promise. US transactional concepts, remedies and professional-responsibility examples require qualification before use in England and Wales. Negotiated commercial drafting cannot establish the fairness, legality or clarity of consumer terms, a privacy notice or a product interface.

**Stage 3 reading target:** Relevant parts of A–D for the conceptual and language foundation, followed by chapters 32–35 for process, review, changes and responsibility. Inspect surrounding examples before deriving a method. The public preface includes earlier-edition material; use the third-edition contents and actual book to resolve locations rather than carrying forward old chapter references.

### B4 — The Legal Risk Management Handbook: An International Guide to Protect Your Business from Legal Loss

**Identity:** Matthew Whalley and Chris Guzelian; 1st edition, 2016; Kogan Page. Print ISBN **9780749477974**. Origin: **selected addition**. The [publisher record](https://www.koganpage.com/risk-compliance/the-legal-risk-management-handbook-9780749477974) identifies the edition and publication date of 3 December 2016.

**Intended contribution:** Examine how legal questions enter organisational risk assessment, mitigation and reporting. The [detailed contents](https://cdn.koganpage.com/media/public/document/the-legal-risk-management-handbook-01-whalley-9780749477974-toc-1.pdf) distinguish general management and reporting from regulatory, conduct, contract and other applications. The foundation needs the general decision methods; application chapters may expose their assumptions.

**Credibility and limits:** The publisher presents practitioner and academic experience behind the work. That is relevant background, not independent validation of its framework. Corporate structures and measurement methods may not transfer to a founder or small production team. The Stage 1 requirement to separate legal constraints, uncertainty and exposure remains in force: a book cannot authorise collapsing them into one score. Substantive examples and professional-role descriptions require later verification where used.

**Stage 3 reading target:** Chapters 1–3, then selected regulatory, conduct and contract sections needed to test the general approach. Look specifically for what can and cannot be measured, who owns a decision, and what happens when evidence is missing. Dispute material may inform referral boundaries without adding litigation to core ownership.

### B5 — In-House Lawyers' Ethics: Institutional Logics, Legal Risk and the Tournament of Influence

**Identity:** Richard Moorhead, Steven Vaughan and Cristina Godinho; first edition, originally 2018; Hart Publishing. The identified [publisher paperback record](https://www.bloomsbury.com/uk/inhouse-lawyers-ethics-9781509944323/) is the **2021 paperback**, ISBN **9781509944323**. Origin: **selected addition**. The paperback date is a format date, not evidence of a revised study.

**Intended contribution:** Test assumptions that commercial integration and helpfulness necessarily improve legal judgement. An [author-written companion article](https://clp.law.harvard.edu/knowledge-hub/magazine/issues/in-house-ethics/the-tournament-of-influence/) describes research involving 67 interviews and a survey of 400 in-house lawyers in England and Wales. It links the study to questions about professional independence and organisational influence. This is a useful reason to select the book, not a substitute for examining its argument and evidence.

**Credibility and limits:** The empirical basis supplies a different kind of evidence from the teaching and management books. The companion account concerns attitudes, reported practice and ethical indicators; it does not establish observed misconduct rates or a causal model for agents. Generalisation from in-house organisations to small teams, external counsel and automated work needs testing. Current professional obligations require current professional sources.

**Stage 3 reading target:** Obtain the book's methods and limitations, findings about organisational position and legal-risk handling, and discussion of ethical judgement. Use the actual contents to establish chapter locations. Test what evidence would distinguish constructive challenge from compromised advice; do not convert the companion article into a settled escalation rule.

## 5. Combined coverage and selection trade-offs

This matrix expresses **expected contribution for examination**, not coverage verified by reading. **Lead** means a main reason for selection; **support** means an anticipated secondary contribution; **limited** means a boundary or gap to investigate. A dash means no material contribution is relied on at this stage.

| Stage 1 responsibility | B1 Skills | B2 Reasoning | B3 Contracts | B4 Risk | B5 Ethics |
|---|---|---|---|---|---|
| Scope and identify issues | Lead | Support | Support | Support | Limited |
| Research authorities | Lead | Support | — | — | — |
| Analyse applicability and options | Support | Lead | Support | Support | Limited |
| Draft legal documents | Support | — | Lead | Limited | — |
| Review, redline and repair | Support | Support | Lead | Support | Limited |
| Compare legal statements with product behaviour | Limited | Limited | Support | Support | Limited |
| Assess change impact and preserve traceability | Limited | Limited | Support | Support | — |
| Communicate risk and uncertainty | Support | Support | Support | Lead | Lead |
| Package human review and specialist escalation | Limited | Limited | Support | Support | Lead |

The last row concerns reasons to investigate escalation and independence, not a claim that B5 supplies a ready-made handoff procedure. Similarly, contract amendments and risk monitoring are only partial starting points for legal-product change impact.

**B1 with B2:** Some overlap is deliberate. A general procedural anchor and concentrated scrutiny of reasoning answer different research needs. Stage 3 must establish whether B2 contributes enough beyond B1; that has not been assumed from reputation alone.

**B3 over A1 or A2:** The boundary owns drafting, review and repair across varied matters. A language manual or technology-contract specialisation would help, but B3's visible process and amendment coverage gives the five-book set more immediate breadth. A1 remains useful if direct examination reveals insufficient precision; A2 remains useful if actual proving work needs deeper technology agreements.

**B4 with B5:** This retains both the appeal of making legal work useful to organisational decisions and a critical investigation of pressures on that work. They are complementary questions, not a finding that one refutes the other. Stage 3 should examine whether their methods disagree, operate at different levels or leave unresolved tensions.

**Keeping A3 outside the five:** Open access and an implementation-facing focus make it a serious alternative. Replacing B5 with A3 would strengthen the privacy-engineering connection but remove the clearest empirical challenge to organisational judgement. Replacing B4 would trade general risk practice for a domain-specific lifecycle treatment. On the Stage 1 boundary, retain the broader set and explicitly carry the traceability gap into subsequent research. Accessibility influenced the comparison but did not silently replace relevance or critical breadth as the selection criterion.

Questions to carry into direct examination include whether risk quantification obscures legal constraints; whether a commercially attractive option changes the treatment of facts or uncertainty; whether a drafting recommendation assumes negotiated bargaining power; and whether a repair preserves the evidence behind an earlier decision. These are project questions, not extracted findings or reconciled conflicts.

## 6. Source-access register and Stage 3 entry work

Access status records the material now available after the user's uploads, not whether a book exists for sale. U identifiers below resolve to the filenames and inspection record in the [source-intake addendum](2026-09-13-stage-02-supplied-source-intake.md). **Full text available** records access, not completed examination. **Relevant excerpts available** is qualified by its actual extent. **Secondary material only** includes supplied summaries and descriptive or contents-only evidence without substantive book passages.

| Book | Access status | Material actually examined | Limitation and next access action |
|---|---|---|---|
| B1 | **full text available** for supplied 3rd ed. (2011); **secondary material only** for selected 10th ed. (2025) | Original publisher/listing evidence; U08 title, copyright, contents and separated body/end samples | U08 supports direct examination of its methods, with findings cited to 2011. It does not establish access to or equivalence with the selected tenth edition. Resolve the edition basis before claiming the intended B1 contribution complete. |
| B2 | **full text available** | Original JSTOR evidence; U07 title, copyright, contents and separated body/end samples | The supplied 2009 copy resolves direct-text access. Meaningful examination of the intended reasoning topics, examples and qualifications remains to be performed. |
| B3 | **relevant excerpts available**, limited to public front matter; U01 is **secondary material only** | Aspen metadata, public contents and selected preface passages; supplied 19-page overview | No substantive book chapter supplied. U01's chapter numbers conflict with the third-edition contents. Obtain the actual chapters and use the verified publisher locations, not the summary's numbering. |
| B4 | **secondary material only** | Kogan Page metadata and detailed contents; supplied 14-page overview U03 | U03 supplies questions for examination, not direct book text. Obtain chapters 1–3 and enough application material to test their assumptions and attributed methods. |
| B5 | **secondary material only** | Publisher record, author-written companion article and supplied 15-page overview U02 | Neither article nor summary is the book. Obtain the relevant methods, findings and limitations directly; detailed summary claims remain unverified. |

Full text is now available for B2 and the supplied earlier edition of B1. The supplied fourth edition of Adams is also available as a complementary direct source. The research and management handbook additions are two-page summaries. No purchasing, account registration or acquisition of a licence was performed. Public source locations are recorded here and in the addendum; no book files, extensive quotations or private access details are committed.

Stage 3 can begin with the available direct material while resolving the remaining access needs. A user-provided copy, existing authorised library access, or sufficiently substantial authorised excerpts can resolve an access need. Excerpts must support the intended contribution and its limitations; there is no arbitrary page quota. Record the actual edition and stable locations. A different format of the same edition is not a sixth book; a different edition needs an explicit comparability check. The addendum identifies the differences already observed in U08.

**Stage 3 cannot be marked complete until all five have been meaningfully examined.** Intake and copy availability do not complete extraction. If remaining access cannot be obtained or direct examination exposes a weak contribution, record the problem and revisit the selection explicitly. Do not substitute a different book silently or treat a supplied summary or model memory as direct book evidence.

## 7. Alternative-source evidence and remaining gaps

The original non-foundational candidates were assessed from the following bounded evidence. A1's supplied fourth edition is now retained as S1; S2 and S3 are documented in the addendum.

| Candidate | Evidence inspected and access observation | Currency and applicability qualification |
|---|---|---|
| A1 — Adams | The [author's book page](https://www.adamsdrafting.com/writing/mscd/) confirms the fifth edition and February 2023 publication; a public [introduction PDF](https://www.adamsdrafting.com/wp-content/uploads/2023/02/MSCD5-Introduction.pdf) was inspected for scope. This is partial direct material, not examination of the manual's individual prescriptions. | Language discipline may endure, but conventions, legal consequences and the needs of a particular document still require scrutiny. |
| A2 — Tollen | The [author's book page](https://www.techcontracts.com/tech-contracts-handbook/) identifies the 2021 third edition, subject coverage and purchase routes, and links later corrections. No book-body text was examined. | Technology terminology and agreement practice can date quickly. The commercial IT-contract focus does not establish consumer or product-regulatory coverage. |
| A3 — Dennedy, Fox and Finneran | The [Apress/Springer book record and contents](https://link.springer.com/book/10.1007/978-1-4302-6356-2) identify the 2014 first edition and offer open-access book/chapter downloads. The contents show requirements, lifecycle and quality-assurance material. The full book was not examined. | The publication predates GDPR. Its engineering methods may remain useful, but its legal statements need current authority and its allocation of responsibilities must fit our boundary. |

The corpus does not claim to cover all substantive law relevant to the Stage 1 matter classes. Its most consequential gaps are:

| Gap or uncertainty | Why it matters | Follow-up owner in the bootstrap |
|---|---|---|
| Legal requirement-to-product traceability, change dependency analysis and repair | This is owned core work, yet the selected books appear to cover it only indirectly | Stage 3 must report the actual shortfall. The supplied Oxford handbook summary and verified contents add targeted legal-design, contract-management and systems-thinking research leads (S3). Stage 4 should examine professional and implementation practice, with A3 also a candidate supporting source. Later workflow and evaluation work must demonstrate the result. |
| Current authority, territorial scope and temporal validity | Durable research concepts cannot establish whether a proposition is currently applicable | Stage 4 primary-source and professional-practice challenge; later matter work must verify applicable authority and status. |
| Privacy, consumer commerce, IP, open-source licensing and creative-production depth | Stage 1 includes bounded work in these fields without promising specialist competence in each | Stage 4 should identify needed authoritative and specialist sources. Later specialisation decisions need their own evidence; this selection approves no pack catalogue. |
| Confidentiality, privilege and safe use of tools or external databases | Professional and technical handling requirements are not established by book selection | Stage 4 must examine current applicable obligations and actual tool behaviours. Later workflow design must make boundaries inspectable. |
| AI-specific failure, source verification and legal evaluation | None of these works supplies evidence that an agent can perform the proposed responsibilities reliably | Later tool comparison and evaluation stages must establish failure cases, review requirements and regression evidence. Advertised AI supplements do not close this gap. |
| Proportionate operations for small teams and non-specialist users | Corporate legal management and in-house research may assume resources the intended users lack | Stage 3 should identify assumptions; Stage 4 should challenge them against professional practice. Later progressive examples test whether the adapted work remains usable. |
| Reliable escalation and accountable adoption | Ethics and risk discussions may explain the problem without specifying a sufficient review packet or decision boundary | Stage 3 and Stage 4 should inform the method; later workflows and benchmarks must test its adequacy while retaining Stage 1's human authority boundaries. |

Kakeibo and Worldstack remain possible later proving contexts, not evidence that these books cover their legal needs. No facts about either consumer are inferred here.

## 8. Origin, approval and completion record

| Decision class | Record |
|---|---|
| Supplied books | None at original selection. Subsequently, eight files represent the five foundational works and three expressly complementary works; see the intake register. |
| Retained supplied books | All represented works retained. Three full-length copies and five summaries are distinguished; *Legal Skills* and Adams have earlier supplied editions than those originally compared. |
| Added foundational books | B1–B5: exactly five distinct works. |
| Substituted, removed or demoted supplied books | None. |
| Alternatives not selected | A1–A3 were not selected as foundational. The supplied Adams fourth edition is now retained as S1; the two new handbook additions are S2–S3. A2–A3 remain possible later sources. |
| Approval decisions | No supplied-book exclusion or substitution requires approval; no pending approval decision prevents completion of Stage 2. |
| Source-access needs | B2 direct text available; B1 third edition available with a selected-edition gap; B3–B5 remain without substantive book text. S1 is directly available; S2–S3 are summaries. Section 6 and the addendum record the actions. |
| Remaining knowledge gaps | Explicitly assigned to subsequent research and validation in section 7. |

The Stage 2 exit is met: the boundary-derived coverage map exists, a broader candidate pool has been compared, exactly five works are selected, their origins and access limitations are recorded, and substitution decisions and remaining gaps are explicit.

The next stage is **Stage 3: Extract and Reconcile the Five-Book Corpus**, using available direct sources and resolving the remaining access needs. It must produce located, independently expressed findings with applicability, failure conditions, production implications and dispositions. This record and its addendum supply selection, intake and the reading agenda only; extraction, reconciliation, broader challenge, implementation and evaluation remain uncompleted.

**Revision 1.1:** Records the user's eight uploads, retains three complementary works, updates access and provenance, and links edition and summary checks. The five foundational works remain selected.
