# Stage 4 supporting log c — privacy / data protection; AI / automated-system regulation; law-to-requirements traceability

**Stage:** 4 (supporting record for `2026-09-19-stage-04-professional-practice-challenge.md`)  
**Retrieved:** 18–19 September 2026 (each register row carries its own date)  
**Evidence ID prefix:** `C-`

## Reading notes

- This record was produced by one research agent working under a written brief. Sources were discovered with web search and inspected with a fetch tool, or by local text extraction of downloaded public PDFs.
- The fetch tool returns a model-written extract. Agents caught it misquoting, reversing a holding, and inventing content. Treat every quotation not marked as text-verified as "as reported". Re-check at the source before durable use.
- Legal propositions here are valid only as of the retrieval date, for the named jurisdiction. They are design evidence. They are not advice and not authority for a live matter.
- Dispositions here are the researcher's proposals. Accepted dispositions are in the main Stage 4 log.
- Benchmark ideas are synthetic.

---

Research dates: 2026-09-18 and 2026-09-19 (the session was interrupted; each source carries its own retrieved-at date).
Every legal proposition below is **valid only as of its retrieved-at date and only for the named jurisdiction**. None is a timeless statement of law.
Method note: web pages were inspected through a fetch tool that returns a model-written summary of the page. Quotes are as returned by that tool. Where the tool summary looked imprecise, this is flagged. Three academic PDFs (C-30, C-31, C-32) and one further PDF (C-35) were read from extracted text directly.

---

## 1. Scope and questions

Streams: (1) privacy / data protection (UK first, EU second); (2) AI / automated-system regulation (EU AI Act, UK position); (3) cross-cutting: tracing law to engineering requirements.

Evidence questions derived from the assignment:

| # | Question |
| --- | --- |
| Q1 | What is the privacy professional's primary fact base, and how is it built and kept current (data mapping, ROPA)? |
| Q2 | How are controller / processor roles, lawful basis, DPIA, transfers, privacy notices and privacy by design actually worked, per the regulator? |
| Q3 | What does the regulator say about keeping the notice in line with actual processing, and about change (new purpose, new processor)? |
| Q4 | What did the Data (Use and Access) Act 2025 (DUAA) change, when did each part commence, and which ICO guidance pages are marked under review or updated? |
| Q5 | What is the EU AI Act application timeline as of September 2026, including the 2026 amendment? What are the chatbot and generated-content disclosure duties? |
| Q6 | Does the UK have a general AI statute? What does the ICO say on AI and automated decision-making (ADM)? |
| Q7 | What does requirements-engineering research say about deriving and tracing legal requirements: methods, failure modes, measured accuracy (including LLM-based work)? |
| Q8 | Do privacy engineering standards (ISO/IEC 27701, ISO 31700, NIST Privacy Framework) give a usable handoff structure? |
| Q9 | Do the findings support, qualify or contradict WG-OV-07, WG-OV-02, FF1-02, FF1-04, SC2-10 (and FF2-18 by comparison)? |
| Q10 | What do the five books miss for these streams? |

---

## 2. Evidence register

"Inspected = yes" means the page or document was fetched and its content examined in this session. "Snippet" means only a search result was seen; such rows are **not** evidence and are listed only as leads.

| ID | Source title | Type | URL | Date (publication / update) | Inspected? (retrieved) | Jurisdiction | Supports / contradicts |
| --- | --- | --- | --- | --- | --- | --- | --- |
| C-01 | ICO — Data (Use and Access) Act 2025 (landing page) | regulator | https://ico.org.uk/about-the-ico/what-we-do/legislation-we-cover/data-use-and-access-act-2025/ | no page date shown | yes (2026-09-18) | UK | Royal Assent 19 June 2025; "All the provisions affecting data protection law and [PECR] are now in force." |
| C-02 | ICO — DUAA: what does it mean for organisations | regulator | https://ico.org.uk/about-the-ico/what-we-do/legislation-we-cover/data-use-and-access-act-2025/the-data-use-and-access-act-2025-what-does-it-mean-for-organisations/ | published 19 June 2025; latest update 19 June 2026 | yes (2026-09-18) | UK | List of DUAA changes (recognised legitimate interests, ADM, research, cookies, SAR searches, children, complaints, compatibility, charity soft opt-in, transfers) |
| C-03 | ICO — Our plans for new and updated guidance | regulator | https://ico.org.uk/about-the-ico/what-we-do/our-plans-for-new-and-updated-guidance/ | no date shown | yes, partly (expandable sections not returned) (2026-09-18) | UK | "Because of the Data (Use and Access) Act, we have started work on new guidance... deprioritise and withdraw some of the planned guidance." |
| C-04 | ICO — guidance plans: Technology | regulator | https://ico.org.uk/about-the-ico/what-we-do/our-plans-for-new-and-updated-guidance/technology/ | no date shown | yes (2026-09-18) | UK | ADM and profiling guidance: status "Drafting", expected Winter 2026; Agentic AI: Spring 2027; Foundation models: Summer 2026 |
| C-05 | ICO — The right to be informed | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/individual-rights/the-right-to-be-informed/ | no date shown | yes (2026-09-18) | UK | Banner: under review. Notice content, timing, review duty, new uses |
| C-06 | ICO — Documentation (overview) | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/accountability-and-governance/documentation/ | no date shown | yes (2026-09-18) | UK | Banner: under review. ROPA duty; link to privacy notice |
| C-07 | ICO — How do we document our processing activities? | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/accountability-and-governance/documentation/how-do-we-document-our-processing-activities/ | no date shown | yes (2026-09-18) | UK | Data mapping as starting point; record is a "living document" |
| C-08 | ICO — Data protection impact assessments | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/accountability-and-governance/data-protection-impact-assessments-dpias/ | no date shown | yes (2026-09-18) | UK | Banner: under review. Triggers, seven steps, prior consultation, review on change |
| C-09 | ICO — Legitimate interests | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/legitimate-interests/ | updated 23 March 2026 | yes (2026-09-18) | UK | Banner: updated for DUAA. Three-part test; LIA; "What if our purposes change?" |
| C-10 | ICO — A guide to lawful basis | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/a-guide-to-lawful-basis/ | updated 02 April 2026 | yes (2026-09-19) | UK | Meaning of "necessary"; choose and document basis before processing; do not swap; state it in the notice |
| C-11 | ICO — Controllers and processors | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/controllers-and-processors/controllers-and-processors/ | no date shown | yes (2026-09-18) | UK | Banner: under review. Role follows actual activity, not contract label |
| C-12 | ICO — International transfers | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/international-transfers/ | no date shown | yes (2026-09-18) | UK | Three-step test; adequacy; IDTA / Addendum / BCRs; TRA now called "data protection test" in legislation |
| C-13 | ICO — Guidance on AI and data protection | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/ | updated 15 March 2023 | yes (2026-09-18) | UK | Banner: under review. Structure by principle; DPIA for AI; Article 22 content now superseded in statute |
| C-14 | ICO — AI and biometrics strategy update, March 2026 | regulator | https://ico.org.uk/about-the-ico/our-information/our-strategies-and-plans/artificial-intelligence-and-biometrics-strategy/ai-and-biometrics-strategy-update-march-2026/ | March 2026 | yes (2026-09-19) | UK | ADM guidance and an AI and ADM code of practice are in preparation; secondary legislation pending |
| C-15 | ICO — Data protection by design and by default | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/accountability-and-governance/guide-to-accountability-and-governance/data-protection-by-design-and-by-default/ | no date shown | yes (2026-09-19) | UK | Banner: **updated** for DUAA. Applies from planning through lifecycle |
| C-16 | ICO — Data protection audit framework (formerly accountability framework URL) | regulator | https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/accountability-and-governance/accountability-framework/ | no date shown | yes (2026-09-19) | UK | Banner: under review. Nine toolkits; control measures; following it "does not guarantee" compliance |
| C-17 | Data (Use and Access) Act 2025, s 142 (commencement) | primary law | https://www.legislation.gov.uk/ukpga/2025/18/section/142 | revised version; no outstanding effects shown | yes (2026-09-18) | UK | Three commencement modes in one section; powers to make regulations in force at Royal Assent |
| C-18 | DUAA 2025, s 80 (automated decision-making) | primary law | https://www.legislation.gov.uk/ukpga/2025/18/section/80 | revised version | yes (2026-09-18) | UK | Replaces UK GDPR Art 22 with Arts 22A–22D |
| C-19 | DUAA 2025 (Commencement No. 6 and Transitional and Saving Provisions) Regulations 2026, SI 2026/82 (C. 10) | primary law (SI) | https://www.legislation.gov.uk/uksi/2026/82/made | made 29 January 2026 | yes (2026-09-18) | UK | Split dates inside one SI (5 Feb 2026; s 103 on 19 June 2026); transitional rules; lists five earlier commencement SIs |
| C-20 | UK GDPR Art 6 on legislation.gov.uk | primary law (official revised text) | https://www.legislation.gov.uk/eur/2016/679/article/6 | "up to date with all changes known to be in force on or before 18 September 2026" | yes (2026-09-19) | UK | Art 6(1)(ea) shown; a "changes and effects yet to be applied" notice is still present |
| C-21 | DLA Piper, Privacy Matters — UK: commencement of the data protection provisions in the DUAA | practitioner | https://privacymatters.dlapiper.com/2026/02/uk-commencement-of-the-data-protection-provisions-in-the-data-use-and-access-act/ | 6 February 2026 | yes (2026-09-18) | UK | Secondary confirmation of C-19; practical to-do list (update notices, ROPA, DSAR policy, transfer assessments) |
| C-22 | European Commission — AI Act (regulatory framework page) | regulator / official | https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai | last update 3 August 2026 | yes (2026-09-18) | EU | Timeline; Omnibus agreed 7 May 2026, in force 27 July 2026 |
| C-23 | Regulation (EU) 2026/1744 (Digital Omnibus on AI) | primary law | https://eur-lex.europa.eu/eli/reg/2026/1744/oj/eng | act of 8 July 2026; OJ 24 July 2026 | yes (2026-09-18) | EU | Amends Reg (EU) 2024/1689: Annex III high-risk → 2 Dec 2027; Annex I → 2 Aug 2028; Art 50(2) grace period |
| C-24 | European Commission — FAQ: transparency obligations under Article 50 AI Act | regulator / official | https://digital-strategy.ec.europa.eu/en/faqs/transparency-obligations-under-article-50-ai-act | 24 July 2026 | yes (2026-09-18) | EU | Who owes which Art 50 duty; "obvious" exception; human review; grace period to 2 Dec 2026; guidelines non-binding |
| C-25 | Lewis Silkin — The Digital Omnibus on AI enters into force today | practitioner | https://www.lewissilkin.com/insights/2026/07/27/the-digital-omnibus-on-ai-enters-into-force-today-102nedo | 27 July 2026 | yes (2026-09-18) | EU | Secondary confirmation of C-23; AI-literacy duty softened; new prohibitions |
| C-26 | Osborne Clarke — Regulatory Outlook March 2026: AI | practitioner | https://www.osborneclarke.com/insights/regulatory-outlook-march-2026-artificial-intelligence | 26 March 2026 | yes (2026-09-18) | UK / EU | No UK AI bill mentioned; UK activity is on copyright and specific harms |
| C-27 | Bratby Law — Is there a UK AI Act? | practitioner (single small firm; weak-to-medium) | https://bratby.law/uk-ai-regulation-what-the-law-says/ | posted 10 April 2026; updated 17 July 2026 | yes (2026-09-18) | UK | "no AI Bill sits before Parliament"; existing law and regulators apply |
| C-28 | EDPB — Guidelines 1/2024 on Art 6(1)(f) GDPR (consultation page) | regulator (EU) | https://www.edpb.europa.eu/our-work-tools/documents/public-consultations/2024/guidelines-12024-processing-personal-data-based_en | consultation 9 Oct – 20 Nov 2024 | yes, page only, PDF not read (2026-09-18) | EU | Existence and status only: consultation version; final adoption **not verified** |
| C-29 | EDPB — Guidelines 07/2020 on controller and processor | regulator (EU) | https://www.edpb.europa.eu/our-work-tools/our-documents/guidelines/guidelines-072020-concepts-controller-and-processor-gdpr_en | final, adopted 7 July 2021 | yes, page only (2026-09-19) | EU | Roles are functional concepts based on factual influence |
| C-30 | Otto & Antón, "Addressing Legal Requirements in Requirements Engineering" | academic | https://www.cc.gatech.edu/~aianton/assets/2007_ieeere_law.pdf | 2007 (IEEE RE; year from file name and search record) | yes, text read (fetched 2026-09-18) | US-centred | Failure modes of legal text; required features of any legal-requirements system, incl. time-stamped trace links |
| C-31 | Breaux & Antón, "Analyzing Regulatory Rules for Privacy and Security Requirements" | academic | https://www.cc.gatech.edu/~aianton/assets/2008_ieeetse_hipaa.pdf | IEEE TSE vol 34 no 1, Jan/Feb 2008 | yes, text read (fetched 2026-09-18, read 2026-09-19) | US (HIPAA) | Statement-level extraction of rights, obligations, constraints; cross-reference handling; counts |
| C-32 | Massey, Rutledge, Antón & Swire, "Identifying and Classifying Ambiguity for Regulatory Requirements" | academic | https://userpages.umbc.edu/~akmassey/documents/papers/akmassey-re2014.pdf | RE 2014 | yes, text read (2026-09-19) | US | Six-type ambiguity taxonomy; low inter-rater agreement; legal expert must resolve |
| C-33 | Etezadi, Abualhaija, Arora & Briand, "Classifier or Prompt: A Case Study on Legal Requirements Traceability" | academic (preprint) | https://arxiv.org/abs/2502.04916 | submitted 7 Feb 2025; v8 12 March 2026 | yes, abstract page only (2026-09-18) | EU (GDPR) / US (HIPAA) | Measured accuracy of automated trace-link recovery |
| C-34 | Hassani, Sabetzadeh, Amyot & Liao, "Rethinking Legal Compliance Automation: Opportunities with LLMs" | academic (preprint) | https://arxiv.org/html/2404.14356v1 | 22 April 2024 | yes (2026-09-19) | general | Sentence-level analysis fails; context raises accuracy; hallucination risk |
| C-35 | Abualhaija et al., "LLM-assisted Extraction of Regulatory Requirements: A Case Study on the GDPR" (XTRAREG) | academic | https://orbilu.uni.lu/bitstream/10993/65265/1/2025-RE-ACSBLSVS.pdf | 2025 (file name suggests RE 2025; venue not confirmed in text) | yes, text read (2026-09-19) | EU | Expert baseline of 108 requirements from legislation + guidelines + case law; LLM coverage and citation accuracy |
| C-36 | NIST Privacy Framework (main page) | standard (voluntary framework) | https://www.nist.gov/privacy-framework | v1.0 16 Jan 2020; v1.1 Initial Public Draft | yes (2026-09-19) | US origin, jurisdiction-neutral | Voluntary; enterprise risk tool |
| C-37 | NIST Privacy Framework — Getting started | standard | https://www.nist.gov/privacy-framework/getting-started-0 | page updated 29 Aug 2025 | yes (2026-09-19) | as above | Five Functions; communicates "from the executive level to the implementation/operations level" |
| C-38 | ISO/IEC 27701:2025 (via ANSI, BSI, SGS search results) | standard | https://www.iso.org/standard/27701 | 2025 edition | **no** — iso.org and ANSI blog returned 403; snippet only | international | Lead only: said to be standalone PIMS with controller and processor control sets |
| C-39 | ISO 31700-1:2023 Privacy by design for consumer goods and services | standard | https://www.iso.org/standard/84977.html | 2023 | **no** — 403 | international | Not verified |
| C-40 | Zeni et al., "GaiusT" (Requirements Engineering 20, 2015) | academic | https://link.springer.com/article/10.1007/s00766-013-0181-8 | 2015 | **no** — snippet only | US / Italy | Lead only; accuracy figures not verified |
| C-41 | ICO consultation on draft ADM and profiling guidance | regulator | https://ico.org.uk/about-the-ico/ico-and-stakeholder-consultations/2026/03/ico-consultation-on-the-draft-guidance-about-automated-decision-making-including-profiling/ | March 2026; closed 29 May 2026 (per snippet) | **no** — snippet only; consistent with C-04 and C-14 | UK | Lead only |

Counts: 37 sources inspected (C-01 to C-37); 4 leads not inspected (C-38 to C-41).

Independence notes:
- C-21 repeats C-19; C-25 repeats C-23. They are confirmation that the tool summaries of the primary texts were read correctly, not independent evidence of the law.
- C-26 and C-27 are two separate practitioner statements on the UK AI position; no primary UK source was reached (see section 9).
- C-30, C-31, C-32 share an author (Antón) and a research programme. C-33, C-34, C-35 come from two other groups (Luxembourg / Ottawa; C-33 and C-35 share one author). The finding "legal text is hard to trace reliably" therefore has at least three research groups behind it.

---

## 3. Practice description per stream

### 3.1 Privacy / data protection (UK primary; EU where noted)

**Roles.** Controller, joint controller, processor are legal roles attached to the organisation per processing activity. The ICO states the role turns on what the organisation actually does, not the contract label (C-11). The EDPB says the same for the EU: "functional concepts" based on "factual influence" (C-29). Inside the organisation: DPO or privacy lead, product and engineering owners, security, procurement, legal. The ICO documentation guidance stresses that "people across your organisation" must be engaged so "nothing is missed" (C-07). Roles of external counsel vs in-house privacy team: not found in inspected sources.

**Professional duties.** Accountability: the controller must be able to demonstrate compliance. The ICO audit framework is organised around "control measures" and warns that following it "does not guarantee that your processing meets all the legal requirements" (C-16).

**Matter intake and fact gathering — the data-flow inventory is the fact base.** The ICO says: "A good way to start is by doing an information audit or data-mapping exercise to clarify what personal data your organisation holds and where." (C-07). The record must be "granular and meaningful", must "reflect the current situation", and is "a living document" (C-07). Every later step (role analysis, lawful basis, notice, DPIA, transfer, retention) takes a row of this inventory as input. The NIST Privacy Framework puts the same idea first (Identify-P) (C-37).

**Issue spotting.** Working sweep per processing activity, as evidenced across C-05 to C-15: purpose → role → lawful basis (with necessity) → special category / children → notice content → retention → recipients and processors → transfers → ADM / profiling → DPIA trigger → security → rights handling → complaints handling (new duty, DUAA s 103, in force 19 June 2026: C-19, C-02).

**Lawful basis.** Chosen before processing and documented: "must determine your lawful basis before you start... and you must document it" (C-10). "You should not swap to a different lawful basis at a later date without good reason" (C-10). Legitimate interests uses a three-part test — purpose, necessity, balancing — recorded in an LIA (C-09). Since 5 February 2026 there is a separate basis, UK GDPR Art 6(1)(ea) "recognised legitimate interests", with no balancing test for listed purposes (C-02, C-19, C-20). This basis is UK-only; it does not exist in the EU GDPR. A UK product offering into the EU cannot carry it across.

**DPIA.** Trigger: processing "likely to result in high risk". ICO steps: decide need → describe processing → consult → assess necessity and proportionality → identify risks → identify mitigations → conclude and sign off. Consult the ICO if high risk cannot be mitigated. Review when processing changes (C-08). The page is marked under review (C-08). For AI systems the ICO adds AI-specific DPIA content (C-13, also under review).

**Transfers.** ICO three-step test for whether there is a restricted transfer; then adequacy regulations, or appropriate safeguards (IDTA, Addendum, BCRs) with a transfer risk assessment, or an exception (C-12). DUAA changed the statutory test; the ICO notes the TRA "is now referred to in UK legislation as a 'data protection test'" (C-12). A practitioner source describes the new standard as "not materially lower than" UK protection (C-21; not verified at primary source in this session).

**Retention.** Retention periods are mandatory notice content (C-05) and therefore must exist per purpose. Method detail for building retention schedules: not found in inspected sources.

**Privacy notice drafting and review.** Required content includes "your purposes... your retention periods... and who it will be shared with" (C-05); lawful basis must be included (C-10). Timing: at collection, or within one month if obtained from another source (C-05). Maintenance: "You must regularly review, and where necessary, update your privacy information." and "You must bring any new uses of an individual's personal data to their attention before you start the processing." (C-05). The notice is therefore a **derived view of the inventory**, not an independent document. This page is marked under review because of DUAA (C-05); DUAA changed notice content rules for research reuse and "information to be provided" (C-02, C-19 search summary).

**Privacy by design.** "starts at the initial planning stages of any system, service, product or process and continues throughout its lifecycle" (C-15). The duty sits on the controller; processors support it (C-15).

**Handling change.** Evidence-backed triggers: new purpose (C-05, C-09, C-10), change in processing (C-08 DPIA review; C-07 record update), new recipient or processor (notice content, C-05; contract and role analysis, C-11), new transfer (C-12), law change (DUAA: C-21 to-do list — update notices, ROPA, DSAR policy, transfer assessments, ADM safeguards), and regulator guidance change (C-03, C-04).

**Source hierarchy (UK).** (1) UK GDPR, DPA 2018, PECR as amended — check the amended text and the commencement instrument (C-17, C-19, C-20). (2) Statutory codes (a code on AI and ADM is planned, not yet made: C-14). (3) ICO guidance — soft law with strong practical force, and currently in flux (section 4, FF2-18 comparison). (4) EDPB guidelines — not binding in the UK; relevant for EU-facing processing (C-28, C-29). (5) Practitioner notes — finding aids only (C-21, C-25).

**Filing / registration boundaries.** ICO prior consultation where DPIA shows unmitigated high risk (C-08). Breach notification, ICO fee registration, EU representative: not researched in this session.

**Risk communication.** Not found in inspected sources beyond the DPIA "sign off and record outcomes" step (C-08).

**Handoffs to engineering.** ISO/IEC 27701 (controller and processor control sets) and the NIST Privacy Framework Core (Function → Category → Subcategory outcomes) are the two common structures for turning obligations into implementable, auditable items. NIST describes its Core as a way of "communicating prioritized privacy protection activities and outcomes across an organization from the executive level to the implementation/operations level" (C-37). NIST is voluntary (C-36). ISO content was not verifiable (C-38, C-39: 403).

**Change monitoring.** The ICO publishes a guidance pipeline with statuses (Drafting, Consultation, Redrafting, Withdrawn, Published) (C-03, C-04). Commencement regulations must be tracked individually: DUAA has had at least six (C-19).

**Failure modes and repairs.** See section 6.

### 3.2 AI / automated-system regulation

**EU — Regulation (EU) 2024/1689 as amended by Regulation (EU) 2026/1744. Valid as of 2026-09-18.**

| Date | What applies | Source |
| --- | --- | --- |
| 1 Aug 2024 | Entry into force | C-22 |
| 2 Feb 2025 | Prohibited practices; AI-literacy duty | C-22 |
| 2 Aug 2025 | GPAI model obligations; governance | C-22 |
| 27 Jul 2026 | Omnibus (Reg 2026/1744) in force; OJ 24 Jul 2026 | C-22, C-23 |
| 2 Aug 2026 | General application, including Art 50 transparency duties | C-22, C-24 |
| 2 Dec 2026 | End of grace period for Art 50(2) machine-readable marking for generative systems already on the market before 2 Aug 2026; new prohibition (non-consensual intimate imagery / CSAM) per Commission page | C-23, C-24, C-25, C-22 |
| 2 Dec 2027 | Annex III (stand-alone) high-risk obligations — moved from 2 Aug 2026 | C-23, C-25 |
| 2 Aug 2028 | Annex I (product-embedded) high-risk obligations | C-23, C-25 |

Caution: the fetch tool's summary of C-23 described Annex III as "biometric AI". That is a summary error; Annex III covers several areas (C-25 lists "stand-alone high-risk systems"). The article-level wording of amended Art 111 and Art 113 should be re-read at source before any skill relies on it.

**Article 50 duties (C-24).**
- *Provider*, interactive systems (chatbots): design so people know they are interacting with AI "unless this is obvious"; the exception is to be "interpreted in a restrictive manner"; notice "from the start of the first interaction".
- *Provider*, generative systems: outputs "marked in a machine-readable format" and detectable. Exemptions include assistive editing and source code (per the Commission FAQ).
- *Deployer*: inform people exposed to emotion recognition or biometric categorisation; label deep fakes; label AI-generated text published on matters of public interest, unless there was "human review or editorial control". "Superficial, solely formal, or procedural checks" do not count.
- Content generated before 2 Aug 2026 need not be labelled retroactively.
- The Commission guidelines (adopted 20 July 2026 per search result; date not verified at source) and the Code of Practice are **non-binding**; the FAQ says non-signatories show compliance "through alternative adequate means".
- Fines up to EUR 15 million or 3% of worldwide turnover; enforcement by national market surveillance authorities (C-24).
- AI-literacy duty was softened by the Omnibus (C-25; not verified at article level).

**Role analysis is again the first step.** Provider vs deployer decides which Art 50 duty applies (C-24). This mirrors controller vs processor. A small product company that wraps a third-party model in its own chatbot must decide whether it is a provider of an AI system, a deployer, or both — a Zone B question for novel facts.

**UK. Valid as of 2026-09-18; primary verification incomplete.** Two practitioner sources say there is no general UK AI statute and no government AI bill before Parliament (C-26, C-27: "no AI Bill sits before Parliament"). A private member's "AI Regulation Bill" debate in the Lords on 4 June 2026 appeared in search results but could not be fetched (403). The House of Commons Library briefing CBP-10003 could not be fetched (403). Treat "no general UK AI statute" as a **well-supported but not primary-verified** proposition.

What does apply in the UK: UK GDPR Arts 22A–22D (C-18), in force 5 February 2026 (C-19). A "significant decision" based "solely" on automated processing — "no meaningful human involvement" — requires safeguards: information, representations, human intervention, ability to contest. Special category data carries a restriction. Decisions relying on Art 6(1)(ea) cannot be solely automated (C-18, per tool summary; re-check at source). The Secretary of State can make regulations on what counts as meaningful human involvement (C-18).

ICO position on AI: the main AI guidance dates from 15 March 2023 and is marked under review (C-13). ADM and profiling guidance: consulted on March–May 2026 (C-41 lead), status "Drafting", due Winter 2026 (C-04). An AI and ADM statutory code of practice is planned; the secondary legislation requiring it is still being developed (C-14). Agentic AI guidance: Spring 2027 (C-04).

**Practical consequence.** For a UK product with an AI chat feature offered into the EU, three different instruments apply to the same interface: UK GDPR transparency (C-05), UK ADM safeguards if decisions are significant (C-18), and EU AI Act Art 50(1) (C-24). The disclosure text must satisfy all three and match what the system really does.

### 3.3 Law-to-requirements traceability (cross-cutting)

**Methods in the literature.**
- *Frame / pattern-based manual extraction* (Breaux & Antón, C-31): go statement by statement; extract rights, obligations and constraints; follow every cross-reference; record ambiguities; assign priorities between rules and exceptions. Applied to the whole HIPAA Privacy Rule, it produced 1,894 constraints; 626 of the 861 non-parameterised constraints "require additional refinement and engineering" before software can test them (C-31). The authors say work is needed "on regulations outside the US" (C-31).
- *Required properties of any support system* (Otto & Antón, C-30): traceability from the originating law to requirements; cross-reference management; handling of exceptions and priorities; a data dictionary with per-regulation definitions; annotation of ambiguous sections for legal counsel; and, critically, the system "must also track the point in time at which that link was established" (C-30).
- *Ambiguity handling* (Massey et al., C-32): six types — lexical, syntactic, semantic, vagueness, incompleteness, referential. Engineers may resolve some intentional ambiguity using a standard; "Unresolved intentional ambiguities and all unintentional ambiguities must be disambiguated by a legal expert." (C-32).
- *Semi-automated annotation* (GaiusT; Nomos): referenced by C-34 as earlier semantic-metadata approaches. Not inspected; accuracy not verified (C-40).
- *LLM-based* (C-33, C-34, C-35): prompt-based trace-link recovery and requirement generation, with retrieval of legal sources.

**Known failure modes.**
- Cross-references ignored → "overlooking important exceptions or priorities and ultimately... non-compliance" (C-30). One earlier formal model assumed external references were satisfied by default; Breaux and Antón's study contradicted that (C-30).
- Supplemental guidance documents "do not have the same legal standing and may even contain misinterpretations" (C-30).
- Amendments: legal texts "are frequently amended"; a trace link without a date cannot support later change analysis (C-30).
- Sentence-level analysis loses definitions, context and cross-references (C-34).
- Non-lawyers cannot agree on ambiguity: 17 participants found on average 33.47 ambiguities in 104 lines; agreement on type was only "slight" (Fleiss' kappa 0.0446) and on count "fair" (ICC 0.316) (C-32). The abstract also reports prior findings that graduate engineers could not reliably judge legal compliance and professionals could not accurately classify cross-references (C-32).

**Evidence on accuracy (all figures as reported by the authors; none replicated here).**
- Trace-link recovery between requirements and legal provisions: best classifier F2 63%; LLM prompt approach average recall 84%, F2 61% (C-33). The authors conclude generic traceability techniques "not specifically designed for legal artifacts" are inadequate (C-33).
- Context matters: GPT-4-Turbo accuracy 41% at sentence level vs 81% with paragraph context (C-34). Risks listed: hallucination, bias, "needle in a haystack" with too much context (C-34).
- Requirement extraction from GDPR with RAG (C-35): generated requirements were 81.8% (access) and 85.7% (portability) correct, but **coverage was low** — 16 of 61 expert reference requirements for access — and the legal citations were correct only 68.2% and 50% of the time. Even with guidelines and case law supplied, "the LLM generates requirements predominantly from the GDPR" text. The expert baseline itself drew on legislation, EDPB guidelines, literature, case law and expert opinion, and tagged each requirement with its source type (L / G / T / J / E) (C-35).

**Reading for this project.** Correct-looking output with poor coverage and unreliable citations is the measured profile of current LLM extraction. Precision on what is produced is not the risk; **omission and mis-citation** are. This is independent support for the project's separate "authority" and "coverage" quality dimensions.

---

## 4. Challenge findings

### WG-OV-07 — Controls: effectiveness, not existence; `risk → requirement → control → evidence` (overview-derived)

| Item | Finding |
| --- | --- |
| Supporting evidence | ICO: records must "reflect the current situation" and be reviewed (C-07); notices must be regularly reviewed and new uses notified before processing (C-05); DPIAs reviewed on change (C-08); the audit framework is built on "control measures" and says following it "does not guarantee" compliance (C-16). NIST Core runs from executive level to operations (C-37). RE literature independently demands law → requirement trace links with dates (C-30) and shows that a third of extracted constraints need more engineering before they are testable (C-31). |
| Contrary / qualifying evidence | (1) In data protection the chain does not start at "risk". Many duties are rule-based and apply whatever the risk (notice content, lawful basis before processing, ADM safeguards: C-05, C-10, C-18). The chain is `legal provision → obligation → requirement → control → evidence`, with risk entering as a **trigger or scaling factor** (DPIA "high risk": C-08). Starting at risk invites treating a fixed duty as optional — the MVG-OV-03 concern. (2) The chain omits the **fact base**: without a data-flow inventory there is nothing to attach the requirement to (C-07). (3) The chain omits **time**: a link needs an as-at date (C-30). |
| Jurisdiction limits | Supporting regulator evidence is UK (ICO). NIST is US-origin and voluntary. The RE studies are US (HIPAA) and EU (GDPR). |
| Changes since the book | DUAA added duties that need operating evidence, e.g. complaints handling within set times from 19 June 2026 (C-02, C-19). |
| Disposition | **Adapt.** Keep "effectiveness, not existence". Replace the chain with `provision (as-at date, source type) → obligation → product fact (inventory row) → requirement → control / implementation → operating evidence`. Risk is a branch condition, not the root. |
| Evidential standing | **Supported finding** for "evidence of operation, not only a document" (regulator + academic, independent). **Context-dependent method** for the exact chain. |

### WG-OV-02 — Risk sits where the business acts (overview-derived)

| Item | Finding |
| --- | --- |
| Supporting evidence | The regulator's method starts from what the organisation really does: data mapping first (C-07); role decided by actual activity, not contract label (C-11, C-29); notice must follow new uses (C-05); privacy by design from "initial planning stages" (C-15); AI Act duties follow the actor's real role as provider or deployer (C-24). |
| Contrary / qualifying evidence | The obligation also moves when the **law or the guidance** moves with no change in business behaviour: DUAA commencement on 5 Feb and 19 June 2026 (C-19); AI Act dates moved by the Omnibus three weeks before they applied (C-23); ICO pages under review (C-05, C-06, C-08, C-11, C-13, C-16). Third parties also create exposure (processors, model providers). So "where the business acts" is one of three change sources: product, law, third party. |
| Jurisdiction limits | UK and EU evidence only. |
| Changes since the book | Not applicable (no verified book text). |
| Disposition | **Retain, with qualification.** Use as the fact-gathering rule: "start from actual behaviour". Do not use it as a complete change-monitoring model. |
| Evidential standing | **Supported finding** (as a fact-gathering principle); **practical heuristic** (as a statement about where risk "sits"). |

### FF1-02 — Enactment and commencement are separate; identify the commencement mode per provision

| Item | Finding |
| --- | --- |
| Supporting evidence (live test: DUAA) | One section, s 142, uses three modes: on Royal Assent (e.g. s 78 and regulation-making powers); two months after passing (ss 69, 82, 96, 97); by regulations for the rest (C-17). Powers-only commencement at Royal Assent is the book's "limited purposes" pattern. SI 2026/82 then split dates **inside one instrument**: most data protection sections on 5 Feb 2026; s 103 and Sch 10 on 19 June 2026 (C-19). At least six commencement SIs exist (C-19 lists 2025/904, 2025/982, 2025/996, 2025/1213, 2026/31). The Act's year, 2025, tells the reader nothing about when Art 22A–22D applied (5 Feb 2026). The same pattern appears in the EU: Reg 2024/1689 has staged application dates, and they were amended on 24 July 2026 for a date of 2 Aug 2026 (C-22, C-23). |
| Contrary / qualifying evidence | None against. Three **extensions** the book record does not state: (1) *Transitional and saving provisions* — SI 2026/82 keeps old time limits for requests received before 5 Feb 2026, leaves earlier automated decisions unaffected, and applies the complaints duty only to complaints received from 19 June 2026 (C-19). The right question is "which version applied to this event on this date?", not only "is it in force?". (2) *Amending Acts* — DUAA mostly operates by changing other instruments (UK GDPR, DPA 2018, PECR). The check must be run on the amended instrument too. (3) *Application dates can themselves be amended* before they arrive (C-23). |
| Jurisdiction limits | UK Acts and SIs; EU regulations use "entry into force" vs "application" — a parallel but different vocabulary. |
| Changes since the book | Tools changed (legislation.gov.uk replaces print tables). Method unchanged. |
| Disposition | **Retain and extend** (add transitional / saving check; add amended-instrument check; add EU "application date" equivalent). |
| Evidential standing | **Supported finding.** |

### FF1-04 — In-force status is per section / subsection; positive and negative check; bring up to date

| Item | Finding |
| --- | --- |
| Supporting evidence | SI 2026/82 commences by section number and includes a sub-section-level entry, "133(4)" (C-19). legislation.gov.uk's revised UK GDPR Art 6 shows Art 6(1)(ea) inserted **and** still carries a "Changes and effects yet to be applied" notice referring to a 2026 SI, alongside the statement that the text is "up to date with all changes known to be in force on or before 18 September 2026" (C-20). This is the book's "bring both up to date with the latest updating service" step, in modern form: the official revised text can lag, and the banner is the signal. |
| Contrary / qualifying evidence | The regulator summary "All the provisions affecting data protection law... are now in force" (C-01) is true at Act level but hides that subordinate pieces are not finished: the ICO says secondary legislation requiring the AI and ADM code is still being developed (C-14), and Art 22D gives a power to redefine "meaningful human involvement" later (C-18). An "all in force" statement from a regulator is a finding aid, not a provision-level check. |
| Jurisdiction limits | UK. |
| Changes since the book | Print tools are obsolete; the granularity rule and two-sided check are not. |
| Disposition | **Retain.** Add: record the "outstanding changes" banner state and the page's as-at date in the authority record. |
| Evidential standing | **Supported finding.** |

### SC2-10 — Pervasively vague wording vs open texture; "go somewhere else" when the words run out

| Item | Finding |
| --- | --- |
| Supporting evidence | "Necessary" and "legitimate interests" are pervasively vague terms in Schauer's sense: the text alone does not decide cases. The ICO supplies the supplement: necessary means "a targeted and proportionate way of achieving a specific purpose", and the basis fails "if you can reasonably achieve the purpose by some other less intrusive means" (C-10); legitimate interests is operationalised as a three-part test recorded in an LIA (C-09). "Meaningful human involvement" (C-18) and "unless this is obvious" (C-24) are further examples; the Commission fills the second with a "reasonably well-informed" average-person standard (C-24). Massey et al. independently treat vagueness as one of six ambiguity types, note some legal ambiguity is intentional, and show that engineers cannot agree on classification (C-32). Open texture is visible too: "solely automated" was precise enough until agentic and LLM-assisted workflows arrived; the ICO now plans agentic AI guidance (C-04). |
| Contrary / qualifying evidence | (1) Schauer frames the supplement as contested theory (purpose, intent, coherence, policy). In regulatory practice the first stop is settled: **regulator guidance**, then case law. The contest is about weight, not about where to look. (2) The legislature can convert a vague standard into a rule: DUAA created "recognised legitimate interests" — a list with no balancing test (C-02, C-09) — and took a power to define "meaningful human involvement" by regulations (C-18). Vagueness is therefore a **moving** property of the text; SC2-10 treats it as static. (3) The supplement is itself unstable and jurisdiction-split: ICO legitimate interests guidance was updated 23 March 2026 (C-09); EDPB Guidelines 1/2024 were a consultation version when last seen (C-28); after DUAA the UK and EU tests for the same words may diverge. (4) Massey: low agreement (kappa 0.0446) means the vague / open-textured tag will not be reliable if assigned by non-lawyers or by a model without review (C-32). |
| Jurisdiction limits | Schauer is US. UK and EU practice gives regulator guidance a central role that the US-centred account does not describe. |
| Changes since the book | DUAA (2025–26); AI Act Art 50 guidelines (2026). |
| Disposition | **Adapt.** Keep the two-type distinction and the "say which kind of indeterminacy" step. Add: (a) a fixed lookup order for regulated fields — statute → statutory code → regulator guidance (dated, status-checked) → case law → EDPB / Commission guidance for EU; (b) record that the term's meaning is supplied by soft law and give that soft law an as-at date; (c) monitor for rule-conversion by amendment. |
| Evidential standing | **Context-dependent method.** |

### FF2-18 (comparison) — Soft law: effect "uncertain until tested in court"

The caution is right on legal status: the Commission itself calls its Art 50 guidelines non-binding (C-24), and the ICO says following its framework "does not guarantee" compliance (C-16). But the book understates practical force. In data protection, guidance defines the operative tests (C-09, C-10), sets the DPIA method (C-08), and is what practitioners tell clients to monitor (C-21). Expert requirement extraction treats official guidelines as a named source class beside legislation and case law (C-35). Disposition: **qualify** — classify status as the book says, and add a second field, *practical weight*, plus *currency state* (current / under review / updated on date / consultation draft / withdrawn). Standing: supported finding.

---

## 5. Missing capabilities (absent from the five books)

| # | Capability | Evidence | Proposed handling | Standing |
| --- | --- | --- | --- | --- |
| M1 | **Data-flow inventory as the primary fact base.** Per processing activity: data categories, subjects, purpose, basis, recipients, processors, transfers, retention, systems. All privacy outputs derive from it. | C-07, C-06, C-37 | Matter intake for privacy work asks for or builds an inventory first. No notice drafting without it. Missing rows are recorded as unknowns (links to C2 fact discipline). | Supported finding |
| M2 | **Role analysis by function** (controller / joint / processor; AI provider / deployer), decided from facts, not labels, and decided per activity. | C-11, C-29, C-24 | A gating step before obligations are listed. Contract label that conflicts with facts is a finding. | Supported finding |
| M3 | **Derived-document consistency**: the notice, ROPA, DPIA, LIA, processor contracts and in-product disclosures are views of one fact base and must agree with it and each other. | C-05, C-07, C-10 | Consistency check: every notice statement maps to an inventory row; every inventory row that needs disclosure appears in the notice. | Supported finding |
| M4 | **Regulator guidance as soft law with a currency state.** Status banner and date are part of the authority record. | C-05, C-06, C-08, C-09, C-10, C-11, C-13, C-15, C-16; C-03, C-04 | Extend the source-standing model (C6) with `practical weight` and `currency state`. Quote the banner verbatim with retrieved-at. | Supported finding |
| M5 | **Transitional and saving provisions; amended-instrument check.** | C-19, C-20 | Extend C4 (legislation currency): ask "which version governed this event?"; check the amended instrument and its outstanding-changes banner. | Supported finding |
| M6 | **Change triggers from three directions**: product change, law / guidance change, third-party change. | C-05, C-08, C-19, C-23, C-21 | Change-impact skill needs a trigger list per direction, and a rule that a trace link carries its creation date (C-30). | Supported finding |
| M7 | **Multi-regime overlap on one interface** (UK GDPR transparency + UK ADM safeguards + EU AI Act Art 50). | C-05, C-18, C-24 | Requirements are tagged by regime and jurisdiction; the disclosure text is tested against each. Divergence (e.g. Art 6(1)(ea) is UK-only) is flagged. | Context-dependent method |
| M8 | **Legal-requirement extraction method**: statement-level coverage, cross-reference closure, exception priority, definitions dictionary, ambiguity annotation with escalation to a legal expert. | C-30, C-31, C-32 | Adopt as the core of any "law → requirement" capability. Each requirement carries: provision, source type (L / G / J / T / E, per C-35), as-at date, interpretation note, open ambiguity flag. | Supported finding (method); accuracy is context-dependent |
| M9 | **Coverage as a separate quality dimension** for extraction. | C-35, C-33 | Evaluate omission separately from correctness; verify every generated citation against the source text. | Supported finding |
| M10 | **Standards as handoff structures** (ISO/IEC 27701 control sets; NIST Core outcomes). | C-36, C-37; C-38 and C-39 not verified | Offer a mapping column, not a dependency. Do not quote ISO content until a copy is lawfully read. | Practical heuristic |
| M11 | **DPIA / LIA / TRA as structured assessment artefacts** with triggers, sign-off and review points. | C-08, C-09, C-12 | Templates are candidates for later stages; outputs must say the ICO method page is under review where that is so. | Supported finding |

---

## 6. Failure modes

| # | Failure | Evidence | How detected | Smallest repair |
| --- | --- | --- | --- | --- |
| F1 | Notice drafted from a template, not from actual processing; or product changes and the notice does not. | C-05, C-07 | Map each notice statement to an inventory row; diff inventory against last notice version | Update the affected notice section only; notify new use before it starts |
| F2 | Role taken from the contract label. | C-11, C-29 | Ask who decides purposes and essential means for this activity | Re-run obligations for the corrected role; flag the contract for amendment |
| F3 | Lawful basis chosen after the fact, or swapped later. | C-10 | Basis has no dated record; notice and ROPA disagree | Record basis with date; escalate if a swap is proposed |
| F4 | "Act is in force" treated as "this provision applied to this event". | C-17, C-19 | Authority record lacks commencing SI, date, transitional rule | Add provision-level entry with SI number and transitional check |
| F5 | Reliance on official revised text without reading the outstanding-changes banner. | C-20 | Authority record has no banner state | Re-fetch; record banner and as-at date; check the amending SI |
| F6 | Reliance on regulator guidance that is marked under review, without saying so; or on a superseded page (ICO AI guidance of March 2023 still describes old Art 22). | C-13, C-18, C-05 | Compare guidance date with commencement dates of amendments | State the banner; rely on the statute for the changed point; re-check when the pipeline page shows "Published" |
| F7 | Carrying a UK-only rule (Art 6(1)(ea); new UK transfer test; UK cookie exemptions) into EU-facing processing. | C-02, C-20, C-21 | Requirement lacks a jurisdiction tag | Split the requirement by jurisdiction |
| F8 | Stale AI Act dates: advice written before 24 July 2026 gives 2 Aug 2026 for Annex III high-risk. Opposite error: assuming the Omnibus delayed Art 50(1) — it did not. | C-23, C-24, C-25 | Check each date against the consolidated or amending text | Correct the date; cite Reg 2026/1744 |
| F9 | Summary-layer error: a tool or secondary summary mislabels the provision (the fetch tool called Annex III "biometric AI"). | C-23 vs C-25 | Cross-check a summary against the article text or a second source | Read the article; never rely on one machine summary for scope |
| F10 | Cross-references not followed; exception missed. | C-30, C-31 | Requirement cites a provision that contains "subject to", "as permitted by", or a reference, with no linked entry | Close the reference; record the priority between rule and exception |
| F11 | Sentence-level reading loses definitions and context. | C-34 | Defined terms in the provision have no dictionary entry | Add definitions and surrounding paragraph to the analysis unit |
| F12 | LLM extraction: plausible requirements, low coverage, wrong citations; guidance and case law ignored even when supplied. | C-35, C-33 | Coverage check against a provision checklist; citation check against source text | Add missed provisions; correct or remove unsupported citations |
| F13 | Non-lawyer (or model) resolves an unintentional ambiguity silently. | C-32 | Requirement has an interpretation but no ambiguity flag or reviewer | Flag; escalate with the competing readings |
| F14 | Trace link without a date; later amendment cannot be assessed. | C-30 | Link record lacks as-at | Add as-at date and version of the provision |
| F15 | "Human in the loop" asserted but the review is formal only. | C-18, C-24 | Ask what the human can change and whether they examine substance | Describe the real process; if not meaningful, apply ADM safeguards / label the content |

---

## 7. Glossary terms

| Term | Meaning | Source | Jurisdiction note |
| --- | --- | --- | --- |
| ROPA (record of processing activities) | The Art 30 record of what personal data is processed, why, by whom, shared with whom, kept how long. A "living document". | C-06, C-07 | UK and EU; ICO page under review |
| Data mapping / information audit | Exercise to find what personal data is held and where; the recommended start of documentation. | C-07 | UK guidance; general practice |
| Controller / processor / joint controller | Decides purposes and means / acts on the controller's behalf / decides jointly. Determined by facts. | C-11, C-29 | UK and EU |
| Lawful basis | The Art 6 ground for processing; fixed and documented before processing starts. | C-10 | UK and EU |
| Legitimate interests assessment (LIA) | Record of the purpose, necessity and balancing tests. | C-09 | UK term of practice; EU uses the same three conditions |
| Recognised legitimate interests | UK GDPR Art 6(1)(ea): listed purposes with no balancing test. In force 5 Feb 2026. | C-02, C-19, C-20 | **UK only** |
| Necessary | "a targeted and proportionate way of achieving a specific purpose"; fails if a less intrusive means is reasonably available. | C-10 | ICO wording; EU concept similar but separately sourced |
| DPIA | Assessment required where processing is likely to result in high risk; seven ICO steps; reviewed on change. | C-08 | UK; EU has its own lists |
| Restricted transfer | A transfer of personal data outside the UK that engages the transfer rules; tested by the ICO three-step test. | C-12 | UK |
| TRA / data protection test | Assessment of protection in the destination; "data protection test" is the post-DUAA statutory name. | C-12 | UK |
| IDTA / Addendum | UK transfer contract tools. | C-12 | UK |
| Significant decision | A decision with legal or similarly significant effect on the data subject (Art 22A). | C-18 | UK (post-DUAA) |
| Solely automated / meaningful human involvement | Decision with "no meaningful human involvement"; definable further by regulations (Art 22D). | C-18 | UK |
| Commencement regulations | SI that appoints the day a provision comes into force; may carry transitional and saving provisions. | C-17, C-19 | UK |
| Transitional / saving provision | Rule that decides which version of the law applies to events straddling commencement. | C-19 | UK |
| Outstanding changes banner | legislation.gov.uk notice that known amendments are not yet applied to the revised text. | C-20 | UK |
| Entry into force vs application | EU regulations enter into force on one date and apply on later, possibly staged, dates. | C-22, C-23 | EU |
| Provider / deployer | AI Act roles: places the system on the market / uses it under its authority. Decide which Art 50 duty applies. | C-24 | EU |
| Article 50 transparency duties | AI-interaction notice; machine-readable marking; emotion / biometric notice; deep-fake and public-interest text labels. | C-24 | EU; applies from 2 Aug 2026 |
| Digital Omnibus on AI | Regulation (EU) 2026/1744 amending the AI Act. | C-23 | EU |
| Under review (ICO banner) | "Due to changes made by the Data (Use and Access) Act, this guidance is under review and may be subject to change." | C-05, C-06, C-08, C-11, C-13, C-16 | UK |
| Legal requirements traceability (LRT) | Links between a legal provision and the software requirement derived from it. | C-30, C-33 | general |
| Cross-reference closure | Following every internal and external reference until the rule, its exceptions and priorities are complete. | C-30, C-31 | general |
| Ambiguity taxonomy (six types) | Lexical, syntactic, semantic, vagueness, incompleteness, referential. | C-32 | general; compare AD2-01 and SC2-11 |
| Coverage (extraction) | Share of the expert reference requirements that an automated method recovers. | C-35 | general |
| PIMS | Privacy information management system (ISO/IEC 27701). | C-38 (not verified) | international |
| Privacy Framework Core | NIST structure: Identify-P, Govern-P, Control-P, Communicate-P, Protect-P. | C-37 | voluntary; US origin |

---

## 8. Candidate quality dimensions and benchmark ideas (synthetic)

Quality dimensions suggested by this stream (additions or sharpenings to Stage 1 §8):

| Dimension | Pass condition |
| --- | --- |
| Inventory grounding | Every legal statement about processing maps to an inventory row; unknown rows are labelled unknown |
| Role gating | Role is decided from facts before obligations are listed |
| Provision-level currency | Record has commencing instrument, date, transitional rule, banner state, as-at date |
| Guidance currency | Guidance record has status label, practical-weight label, banner text, page date or "no date shown" |
| Jurisdiction tagging | Every requirement carries a regime and jurisdiction; UK-only rules are not exported |
| Coverage | Extraction is checked against a provision checklist; omissions are counted separately from errors |
| Citation fidelity | Every cited provision actually contains the proposition |
| Ambiguity handling | Vague and ambiguous terms are flagged with competing readings and escalated, not silently resolved |
| Link dating | Every law → requirement link has a creation date and provision version |
| Operating evidence | Each requirement names the evidence that would show it operates |

Benchmark ideas (all synthetic; no real company data):

1. **Notice vs inventory drift.** A fictional budgeting app's inventory gains a new analytics processor in a third country. The old notice is supplied. Pass: the agent finds the missing recipient and transfer, asks for the transfer mechanism, proposes a change to two notice sections only, and says new use must be notified before it starts.
2. **Label vs function.** A contract calls a vendor a "processor"; the facts show the vendor reuses the data for its own model training. Pass: role flagged as likely controller for that activity; contract label reported as a finding; escalation question framed.
3. **Straddling event.** A subject access request received 30 January 2026 and answered in March 2026; a complaint received 10 June 2026. Pass: the agent applies the transitional rules in SI 2026/82 rather than "DUAA is in force", and cites the SI.
4. **Banner trap.** Provide a captured page of an official revised provision with an outstanding-changes notice. Pass: the agent records the banner, identifies the amending instrument, and lowers confidence until checked.
5. **Guidance under review.** Ask for ADM advice using the ICO AI guidance dated March 2023. Pass: the agent notes the banner, relies on Arts 22A–22C for the changed point, and records that final ADM guidance is due Winter 2026.
6. **Stale AI Act date.** Supply a June 2026 memo stating Annex III obligations apply from 2 August 2026. Pass: corrected to 2 December 2027 with Reg 2026/1744 cited; Art 50(1) date left at 2 August 2026.
7. **Chatbot disclosure across regimes.** A UK company offers an AI support chat to EU consumers and makes automated refund decisions. Pass: requirements separated into EU AI Act Art 50(1), UK/EU GDPR transparency, and ADM safeguards; provider / deployer role reasoned; "obvious" exception not assumed.
8. **Export of a UK-only basis.** The user asks to rely on "recognised legitimate interests" for EU users. Pass: refused for the EU limb with reason; EU three-condition test proposed instead.
9. **Cross-reference closure.** A fictional regulation has an obligation "except as permitted by §12(b)", and §12(b) adds a condition. Pass: the requirement includes the exception and its condition with a priority note.
10. **Coverage test.** Give the full text of one right plus a regulator guideline and one case summary. Expert checklist has 20 requirements from all three sources. Pass: recall reported; requirements tagged L / G / J; no requirement cites a provision that does not contain it.
11. **Formal human review.** A workflow has a human click "approve" on every model decision in under five seconds. Pass: the agent does not accept "human in the loop"; treats the decision as solely automated unless shown otherwise.
12. **Ambiguity escalation.** A provision requires "appropriate" safeguards with no standard named. Pass: tagged vague (possibly intentional); candidate standard offered as an assumption; escalation question written; not silently resolved.

---

## 9. Failed retrievals and unresolved questions

Failed retrievals:

| URL | Result |
| --- | --- |
| https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/legitimate-interests/when-is-using-personal-information-necessary/ | 404 (guessed URL). "Necessary" wording taken from C-10 instead. |
| https://www.whitecase.com/insight-alert/eu-ai-omnibus-enters-force-amending-ai-act | 403 |
| https://commonslibrary.parliament.uk/research-briefings/cbp-10003/ and the PDF at researchbriefings.files.parliament.uk | 403 / HTML block page |
| https://www.twobirds.com/en/insights/2026/ai-in-the-kings-speech-2026-regulating-for-growth-bill-announced | 402 |
| https://hansard.parliament.uk/Lords/2026-06-04/debates/0A1BCBAE-E906-4071-AA92-BCE005D57121/AIRegulationBill | 403 |
| https://www.iso.org/standard/27701 ; https://www.iso.org/standard/84977.html ; https://blog.ansi.org/ansi/iso-iec-27701-2025-privacy-management-systems/ | 403 |
| https://orbilu.uni.lu/... (C-35) | fetch tool failed on TLS certificate; retrieved with curl and read from text |

Unresolved questions:

1. **UK AI statute — primary verification.** "No general UK AI statute; no government AI bill before Parliament" rests on two practitioner sources (C-26, C-27). The King's Speech 2026 content (a "Regulating for Growth Bill" appeared in a search title) and the Lords private member's bill were not read. Needs a gov.uk or parliament.uk source.
2. **Which ICO pages are under review — complete list.** Six pages were seen with the under-review banner (C-05, C-06, C-08, C-11, C-13, C-16) and three with an "updated" banner (C-09 on 23 March 2026, C-10 on 02 April 2026, C-15 undated). Most ICO pages showed no last-updated date in the fetched content. The expandable items of the ICO guidance pipeline (C-03) were not returned by the tool; only the Technology sub-page (C-04) was read.
3. **The instrument behind the C-20 banner.** The tool reported a pending effect from "S.I. 2026/386". That SI was not inspected; its subject is unknown.
4. **Article-level wording** of amended AI Act Arts 111 and 113, of the softened AI-literacy duty, and of the new prohibitions: read via summaries only.
5. **UK transfer test wording** ("not materially lower"): practitioner source only (C-21).
6. **EDPB Guidelines 1/2024** final adoption status: not verified (C-28 shows the consultation version only). EDPB guidance on DPIA lists, transfers (Recommendations 01/2020) and the EDPB opinion on AI models were not inspected.
7. **GaiusT and Nomos accuracy**: not inspected (C-40). Known only through C-34's citation.
8. **C-33 limitations** and dataset detail: only the arXiv abstract page was read; the 1,891-requirement HIPAA figure came from a search snippet and is not used as evidence.
9. **Enforcement evidence** of notice / practice mismatch (ICO or EU DPA decisions) was not researched; F1 rests on the regulator's stated duty, not on an observed enforcement case.
10. **Retention schedule method**, breach notification, ICO fee registration, EU representative, and children's code: not researched.
11. **Moorhead-style pressure questions** (MVG findings) were outside this assignment.
