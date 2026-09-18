# Stage 4 supporting log f — legal research and memorandum practice; open professional-boundary questions

**Stage:** 4 (supporting record for `2026-09-19-stage-04-professional-practice-challenge.md`)  
**Retrieved:** 18–19 September 2026 (each register row carries its own date)  
**Evidence ID prefix:** `F-`

## Reading notes

- This record was produced by one research agent working under a written brief. Sources were discovered with web search and inspected with a fetch tool, or by local text extraction of downloaded public PDFs.
- The fetch tool returns a model-written extract. Agents caught it misquoting, reversing a holding, and inventing content. Treat every quotation not marked as text-verified as "as reported". Re-check at the source before durable use.
- Legal propositions here are valid only as of the retrieval date, for the named jurisdiction. They are design evidence. They are not advice and not authority for a live matter.
- Dispositions here are the researcher's proposals. Accepted dispositions are in the main Stage 4 log.
- Benchmark ideas are synthetic.

---

- Evidence ID prefix: `F-`
- Retrieval dates: work ran across two days because of a usage-limit interruption. Each source row carries its own retrieved-at date (2026-09-18 or 2026-09-19).
- Every legal proposition below is **valid only as at the retrieval date, for the named jurisdiction**. None is timeless.

## 0. Reliability note on the inspection tooling (read before using quotes)

`WebFetch` returns a summary written by a small model, not the raw page. For five sources the PDF was saved locally and I extracted the text myself with `pypdf`; quotes from those are **verbatim-verified**: F-04 (Ayinde), F-08 (Magesh et al.), F-09 (CCBE), F-13 (Practice Direction 2012), F-36 (President of the Family Division guidance). Quotes from every other source are **relayed by the fetch model** and must be re-checked at source before they enter a durable document.

Three fetch-model errors were caught during this work and are corrected in this file:

1. F-36: the fetch summary gave the author as "Mr Justice Keehan" and the date as 25 February 2025. The extracted text shows Sir Andrew McFarlane, President of the Family Division, 24 February 2025.
2. F-19: the fetch summary said HRA 1998 s 3 is "not currently in force". The annotations show s 3 is in force and is **excluded** for named contexts only. (This is exactly the FF1-06 trap.)
3. F-25: the fetch summary gave "Friday, March 8, 2026"; 8 March 2026 was not a Friday. The decision date is recorded as not verified.

This is itself Stage 4 evidence: a summarising layer between the agent and the source produces plausible errors of author, date and legal status.

---

## 1. Scope and questions

Stream 1 — legal research and memorandum practice (England and Wales first; EU second; US where needed):

- RQ1. How is the currency of UK legislation checked today on legislation.gov.uk? What do the "changes to legislation" banners mean? How current is the revised text? What is and is not revised?
- RQ2. What are the official and free sources of case law? What do they cover? What do they not provide (later treatment)?
- RQ3. Who provides later-treatment (citator) checks, and what is available without a subscription?
- RQ4. What is the legal status of EUR-Lex consolidated texts?
- RQ5. What is the hierarchy of law reports and which judgments may not be cited (E&W)?
- RQ6. How are research memoranda structured in practice?
- RQ7. How have courts, regulators and professional bodies responded to fabricated AI citations?
- RQ8. What is the measured hallucination rate of commercial legal-AI research tools?
- RQ9. What changed since 2011 in the court hierarchy and in the EU-law and human-rights interpretive duties?
- RQ10. What is the modern UK approach to statutory interpretation?

Stream 2 — boundary questions left open by Stage 1:

- BQ2. How do US and EU member-state rules treat software or AI tools that give legal help to the public? Is the advice boundary jurisdiction-dependent?
- BQ3. Which other UK statutory perimeters exist beside LSA reserved activities, immigration advice and FSMA regulated activities?
- BQ5. What do ABA Formal Opinion 512, the Law Society, the Bar Council and the CCBE say?
- BQ6. How does privilege apply to material a non-lawyer puts through an AI tool?

---

## 2. Evidence register

"Inspected" = the page or document was fetched. "V" = text extracted locally and quotes verbatim-verified. "M" = content relayed by the fetch model; re-verify before durable quotation.

| ID | Source title | Type | URL | Date (publication / update) | Inspected? (retrieved) | Jurisdiction | Supports / contradicts |
| --- | --- | --- | --- | --- | --- | --- | --- |
| F-01 | legislation.gov.uk — "Understanding legislation" | Official publisher (The National Archives) | https://www.legislation.gov.uk/understanding-legislation | Undated page | Yes, M (2026-09-18) | UK | Revised text aims to include amendments "within three months" of commencement; unapplied effects flagged in "Changes to Legislation" banner; most secondary legislation not revised; records non-textual effects ("applied", "modified"). Supports FF1-05, FF1-06. |
| F-02 | legislation.gov.uk — Help | Official publisher | https://www.legislation.gov.uk/help | Undated page | Yes, M (2026-09-18) | UK | "All Acts ... are kept up to date"; SIs from 2018 kept up to date; timeline / point-in-time; "prospective" versions; changes facility updated "four to eight weeks" after editorial processing. Internal inconsistency with F-01 on which SIs are revised (2018 vs "2014 onwards"). |
| F-03 | Find Case Law — About this service | Official publisher (TNA with MoJ / judiciary) | https://caselaw.nationalarchives.gov.uk/about-this-service | Undated page | Yes, M (2026-09-18) | E&W; UKSC / JCPC UK-wide | "official and free source"; coverage from early 2000s; not all decisions written; Open Justice Licence; API. No citator function mentioned. Supports FF1-19. |
| F-04 | *R (Ayinde) v London Borough of Haringey; Al-Haroun v Qatar National Bank* [2025] EWHC 1383 (Admin), Divisional Court, 6 June 2025 | Court | https://www.judiciary.uk/wp-content/uploads/2025/06/Ayinde-v-London-Borough-of-Haringey-and-Al-Haroun-v-Qatar-National-Bank.pdf | 6 June 2025 | Yes, V (2026-09-18) | E&W | Paras 6–9, 23, 30, 74. Duty to check AI research against authoritative sources; list of authoritative sources; leadership responsibility; range of sanctions. Supports FF1-17, FF1-18; supplies failure taxonomy. |
| F-05 | SRA — "Misuse of AI" warning notice | Regulator | https://www.sra.org.uk/solicitors/guidance/misuse-ai/ | 17 August 2026 | Yes, M (2026-09-18) | E&W | Citations must be "genuine, relevant, have a verifiable citation"; accountability not transferable; supervision; confidentiality; disciplinary risk. Cites Ayinde. |
| F-06 | Bar Council — "Considerations when using ChatGPT and generative AI software based on large language models" (landing page) | Professional body | https://www.barcouncilethics.co.uk/documents/considerations-when-using-chatgpt-and-generative-ai-software-based-on-large-language-models/ | First issued Jan 2024; last reviewed 25 Nov 2025 | Landing page yes, M; PDF body not inspected (2026-09-18) | E&W | Not BSB Handbook guidance; hallucination, confidentiality, privilege, bias risks. Body details not verified. |
| F-07 | Judiciary — "Artificial Intelligence (AI) – Judicial Guidance (October 2025)" (landing page) | Court / judiciary | https://www.judiciary.uk/guidance-and-resources/artificial-intelligence-ai-judicial-guidance-october-2025/ | 31 October 2025; replaces April 2025 version | Landing page yes, M; PDF not inspected (2026-09-18) | E&W | Personal responsibility for all material; do not enter private information in public tools; expanded hallucination and bias text. No later version found on 2026-09-18. |
| F-08 | Magesh, Surani, Dahl, Suzgun, Manning, Ho — "Hallucination-Free? Assessing the Reliability of Leading AI Legal Research Tools" (arXiv:2405.20362v1) | Academic (preregistered) | https://arxiv.org/abs/2405.20362 ; PDF https://arxiv.org/pdf/2405.20362 | Submitted 30 May 2024 | Yes, V (2026-09-18) | US law queries | Numbers in §3.8 below. Contradicts vendor "hallucination-free" claims. Later journal version not inspected. |
| F-09 | CCBE — "Guide on the use of generative AI by lawyers" | Professional body (EU-level) | https://www.ccbe.eu/fileadmin/speciality_distribution/public/documents/IT_LAW/ITL_Guides_recommendations/EN_ITL_20251002_CCBE-guide-on-the-use-of-the-use-of-generative-AI-for-lawyers.pdf | 2 October 2025 | Yes, V (2026-09-18) | EU / Europe | Verify output "where the use case requires"; professional secrecy; transparency to client; sanctions risk. A March 2026 CCBE technical guide exists (search result only, not inspected). |
| F-10 | NCBE *The Bar Examiner* (Fall 2024) — article on ABA Formal Opinion 512 | Professional body (secondary for the Opinion) | https://thebarexaminer.ncbex.org/article/fall-2024/generative-artificial-intelligence-tools/ | Fall 2024; Opinion dated 29 July 2024 | Yes, M (2026-09-18) | US (Model Rules; not binding in any state by itself) | Competence, confidentiality and informed consent (boilerplate insufficient), communication, candour, supervision, fees. **The Opinion itself was not inspected (403).** |
| F-11 | EUR-Lex — Consolidated texts collection page | Official publisher (EU) | https://eur-lex.europa.eu/collection/eu-law/consleg.html | Undated | Yes, M (2026-09-18) | EU | "Consolidated texts have no legal effect." |
| F-12 | EUR-Lex — consolidated text of Directive 2013/34/EU, version 18.03.2026 (disclaimer) | Official publisher (EU) | https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX%3A02013L0034-20260318 | Consolidation date 18 March 2026 | Yes, M (2026-09-18) | EU | "purely as a documentation tool and has no legal effect"; authentic versions are those in the Official Journal. Supports FF1-25. |
| F-13 | Practice Direction: Citation of Authorities (2012), Lord Judge CJ ([2012] 1 WLR 780 per search result; report citation not verified) | Court (practice direction) | https://www.judiciary.uk/wp-content/uploads/JCO/Documents/Practice+Directions/lcj-pract-dir-citation-authorities-2012.pdf | PDF created 23 March 2012 | Yes, V (2026-09-18) | E&W (Senior Courts, Crown Court, county courts, magistrates' courts) | Paras 6–11, 13: hierarchy of reports; unreported cases; garbled reproduction. Supports FF1-17; supports and sharpens SC1-16. |
| F-14 | *R (O) v Secretary of State for the Home Department* [2022] UKSC 3, 2 February 2022 (Lord Hodge) | Court | https://caselaw.nationalarchives.gov.uk/uksc/2022/3 | 2 February 2022 | Yes, M (2026-09-18) | UK | Paras 29–31: words in context; external aids "secondary"; objective intention. Supports FF1-13, SC2-08, SC2-12 (UK form). |
| F-15 | Retained EU Law (Revocation and Reform) Act 2023 — contents | Primary law | https://www.legislation.gov.uk/ukpga/2023/28/contents | Banner: no known outstanding effects | Yes, M (2026-09-18) | UK | ss 2–6 headings: sunset of retained EU rights; abolition of supremacy; abolition of general principles; "assimilated law"; role of courts. |
| F-16 | European Union (Withdrawal) Act 2018 s 6 | Primary law | https://www.legislation.gov.uk/ukpga/2018/16/section/6 | "up to date with all changes known to be in force on or before 16 September 2026" | Yes, M (2026-09-18) | UK | UKSC "not bound by any assimilated EU case law"; same test as departing from own case law; "relevant court" by regulations. Contradicts the 2011 map in FF1-24. |
| F-17 | REUL Act 2023 s 6 (Role of courts) | Primary law | https://www.legislation.gov.uk/ukpga/2023/28/section/6 | Marked **Prospective**; "S. 6 not in force at Royal Assent, see s. 22(3)" | Yes, M (2026-09-18) | UK | Enacted-but-uncommenced provision; live example for FF1-05 and C4. |
| F-18 | REUL Act 2023 s 3 (Abolition of supremacy of EU law) | Primary law | https://www.legislation.gov.uk/ukpga/2023/28/section/3 | In force 1 January 2024 (SI 2023/1363 per annotation) | Yes, M (2026-09-18) | UK | Inserts EUWA s 5(A1): supremacy principle "is not part of domestic law". Rebuilds FF1-14. |
| F-19 | Human Rights Act 1998 s 3 | Primary law | https://www.legislation.gov.uk/ukpga/1998/42/section/3 | "up to date with all changes known to be in force on or before 18 September 2026"; future changes flagged | Yes, M (2026-09-18 and 2026-09-19) | UK | s 3(1) duty survives; C-notes show s 3 "excluded" by named Acts; several exclusions "yet to be applied". Supports FF1-06; qualifies FF1-14. |
| F-20 | BAILII — About | Free-access publisher (charity) | https://www.bailii.org/bailii/ | Statistics dated August 2019 | Yes, M (2026-09-19) | UK / Ireland | Free primary materials; no citator mentioned; separate terms on reproduction and prohibited uses (not inspected). |
| F-21 | FTC — "FTC Finalizes Order with DoNotPay..." | Regulator | https://www.ftc.gov/news-events/news/press-releases/2025/02/ftc-finalizes-order-donotpay-prohibits-deceptive-ai-lawyer-claims-imposes-monetary-relief-requires | 11 February 2025 (Commission vote 16 January 2025, 5–0) | Yes, M (2026-09-19) | US federal | $193,000; notice to 2021–2023 subscribers; ban on unsubstantiated "performs like a lawyer" claims. Basis: FTC Act s 5 deception, **not** UPL. |
| F-22 | Germany — Rechtsdienstleistungsgesetz (RDG), official English translation | Primary law (translation) | https://www.gesetze-im-internet.de/englisch_rdg/englisch_rdg.html | Translation includes amendments to 10 March 2023 | Yes, M (2026-09-19) | Germany | §2(1) "legal service"; §3 permission required; §5 ancillary; §6 gratuitous; §10 registered persons. Shows advice itself is perimetered, unlike E&W. |
| F-23 | Bundesgerichtshof press release 171/2021 — I ZR 113/20 (Smartlaw contract generator) | Court (press release, German) | https://www.bundesgerichtshof.de/SharedDocs/Pressemitteilungen/DE/2021/2021171.html | 9 September 2021 | Yes, M (2026-09-19) | Germany | Template-driven generator is not a legal service: no activity in a "concrete affair"; works from typical fact constellations. Full judgment not inspected. |
| F-24 | Texas Government Code §81.101 (mirror of official text) | Primary law via unofficial mirror | https://texas.public.law/statutes/tex._gov't_code_section_81.101 | Mirror currency date 26 May 2025 | Yes, M (2026-09-19). Official site returned navigation only; Justia 403. | US — Texas | §81.101(c): software is not the practice of law if it states "clearly and conspicuously" that it is "not a substitute for the advice of an attorney". |
| F-25 | E Volokh, "Court Upholds New York's Limits on Unauthorized Practice of Law" (Reason / Volokh Conspiracy) | Practitioner / academic blog (secondary) | https://reason.com/volokh/2026/03/08/court-upholds-new-yorks-limits-on-unauthorized-practice-of-law/ | 8 March 2026 | Yes, M (2026-09-19) | US — New York, federal | *Upsolve v James* on remand (SDNY, Kaplan J): UPL rules upheld under intermediate scrutiny; "The only thing plaintiffs cannot do is advise a specific person about his or her individual case." Decision itself not inspected; 2d Cir. opinion (9 Sept 2025) seen only as search result. |
| F-26 | Harvard Law Review Blog — "United States v. Heppner" | Academic (secondary) | https://harvardlawreview.org/blog/2026/03/united-states-v-heppner/ | March 2026; opinion dated 17 February 2026 (SDNY, Rakoff J) | Yes, M (2026-09-19) | US federal (SDNY) | A defendant's own exchanges with a consumer AI tool: no attorney-client privilege, no work product. Caveat: different result possible if counsel directed the use (*Kovel*). Opinion itself not inspected. |
| F-27 | *R (Prudential plc) v Special Commissioner of Income Tax* [2013] UKSC 1, 23 January 2013 | Court | https://caselaw.nationalarchives.gov.uk/uksc/2013/1 | 23 January 2013 | Yes, M (2026-09-19) | UK | Legal advice privilege is confined to advice from members of the legal profession; extension is for Parliament. |
| F-28 | FCA — Claims management companies; "CMCs: how we authorise and regulate firms" | Regulator | https://www.fca.org.uk/firms/claims-management-companies ; https://www.fca.org.uk/firms/claims-management-regulation/how-we-will-authorise-regulate | Second page last updated 6 February 2023 | Yes, M (2026-09-19) | Great Britain (scope detail not verified) | FCA regulates CMCs since 1 November 2018; authorisation needed; activities named: seeking out, referrals, advising, investigating, representing. |
| F-29 | Financial Services and Markets Act 2000 s 419A | Primary law | https://www.legislation.gov.uk/ukpga/2000/8/section/419A | "up to date ... on or before 19 September 2026"; **many outstanding changes to FSMA not yet applied** | Yes, M (2026-09-19) | UK | "claims management services" = "advice or other services in relation to the making of a claim". |
| F-30 | Insolvency Act 1986 s 389 | Primary law | https://www.legislation.gov.uk/ukpga/1986/45/section/389 | Up to date to 19 September 2026; outstanding changes from 2025 c. 36 flagged | Yes, M (2026-09-19) | GB | Acting as insolvency practitioner when not qualified: imprisonment or fine or both. |
| F-31 | Legal Services Act 2007 Sch 2 | Primary law | https://www.legislation.gov.uk/ukpga/2007/29/schedule/2 | "no known outstanding effects" | Yes, M (2026-09-19) | E&W | Para 5: reserved instrument activities exclude "a will or other testamentary instrument". Para 6: probate activities. |
| F-32 | Legal Services Board — "Reviewing the scope of regulation: will-writing" | Oversight regulator | https://legalservicesboard.org.uk/our-work/work-related-to-previous-years/reviewing-the-scope-of-regulation-will-writing | Historic page (Feb / May 2013 events) | Yes, M (2026-09-19) | E&W | LSB recommended reservation (Feb 2013); Lord Chancellor declined (May 2013). Will-writing is not reserved. |
| F-33 | IALS Library guide — "Cases – Keeping up-to-date with the law" | Professional / academic library | https://libguides.ials.sas.ac.uk/c.php?g=659243&p=4653545 | Updated 7 May 2026 | Yes, M (2026-09-19) | UK | Tools named for updating cases are subscription: Lexis+, Westlaw UK, vLex Justis, print citators. Free tools listed only for alerts (BAILII RSS, court sites). |
| F-34 | CUNY School of Law — "Drafting a Law Office Memorandum" | Academic / professional method | https://www.law.cuny.edu/academics/academic-resources-support/legal-writing-center/student-resources/drafting-a-law-office-memorandum/ | Undated | Yes, M (2026-09-19) | US | Heading; Question Presented; Brief Answer; Facts; Discussion; Conclusion. Include unfavourable facts and counterarguments; calibrated brief answer. |
| F-35 | J Feng, "How to write legal research memos" (Practising Law) | Practitioner | https://www.practisinglaw.com.au/how-to-write-legal-research-memos/ | Updated July 2026 | Yes, M (2026-09-19) | Australia (common-law practice) | Introduction; Executive Summary; Body (facts, "key assumptions", analysis); Moving Forward; footnoted pinpoints. Answer first. |
| F-36 | President of the Family Division — "Citation of Authorities: Judgments of Circuit Judges and District Judges" | Court (guidance) | https://www.judiciary.uk/wp-content/uploads/2025/02/PFD-Guidance-citation-of-authorities-2025.pdf | 24 February 2025 | Yes, V (2026-09-19) | E&W (Family Court, Court of Protection) | Quotes 2001 Practice Direction cll 6.1–6.2; judgments below High Court level "will not be citable" without an approved express statement. Strong support for SC1-16 "not permissible" class. |
| F-37 | legislation.gov.uk — Changes affecting the Human Rights Act 1998 | Official publisher | https://www.legislation.gov.uk/changes/affected/ukpga/1998/42 | Live table | Yes, M (2026-09-19) | UK | Effect types in live use: saved; appointed day(s); transfer of functions; modified; words substituted / repealed / inserted; excluded; applied in part; amended; referred to; substituted; repealed. Column "Changes applied to website text?" = Yes / Not yet / N/A. Direct support for FF1-06. |
| F-38 | Upper Tribunal (IAC) [2026] UKUT 81 (IAC) — shown on Find Case Law as *UK v SSHD*; a secondary source (F-39) calls it *R (Munir)* | Court | https://caselaw.nationalarchives.gov.uk/ukut/iac/2026/81 | Fetch reported "17 November 2025" (probably hearing date; promulgation date not verified) | Yes, M (2026-09-19) | UK (tribunal) | Para 21: putting client and Home Office letters into a public AI tool is to "breach client confidentiality and waive legal privilege"; paras 57–59: supervisors more culpable; referral to regulator to be expected. |
| F-39 | UK Human Rights Blog — "Civil Procedure Guidance on AI and 'Fake Authorities'" (R English) | Practitioner (secondary) | https://ukhumanrightsblog.com/2026/03/31/use-of-ai-by-lawyers/ | 31 March 2026 | Yes, M (2026-09-19) | E&W | Reports Civil Procedure News 3/2026 (11 March 2026). Not independent of F-04 and F-38: it repeats them. |

Counts: 39 register entries, all fetched; 5 verbatim-verified; 2 are landing pages whose PDF body was not inspected (F-06, F-07); 4 are secondary routes to a primary document that was blocked or not fetched (F-10, F-25, F-26, F-39).

Independence note. F-05, F-06, F-07, F-09, F-10 and F-38 all point the same way (verify; keep confidential; you stay accountable). They are independent bodies, but after June 2025 most UK material **cites F-04**; treat F-04 as the root and the rest as adoption, not as separate proof. F-08 is the only quantitative evidence in the set.

---

## 3. Practice description

### 3.1 Roles and duties

- **Who does research.** Trainees, pupils, paralegals, associates, professional support lawyers and law librarians research; a supervising lawyer signs off. F-04 para 8 equates AI-assisted research with relying on "the work of a trainee solicitor or a pupil barrister": the relying lawyer carries the duty.
- **Duty to verify.** F-04 para 7: lawyers using AI for research have "a professional duty ... to check the accuracy of such research by reference to authoritative sources" before use "to advise clients or before a court". The duty is not limited to litigation.
- **Authoritative sources named by the court** (F-04 para 7): "the Government's database of legislation, the National Archives database of court judgments, the official Law Reports published by the Incorporated Council of Law Reporting ... and the databases of reputable legal publishers".
- **Leadership duty.** F-04 para 9: "practical and effective measures must now be taken" by heads of chambers, managing partners and regulators; future hearings will ask whether this was done. F-38 para 58: a supervisor who lets false citations through "is likely to be more culpable".
- **Regulator position (E&W, as at 2026-09-18).** F-05: accountability for "all work and advice delivered to clients, whether or not AI has been used"; authorities must be "genuine, relevant, have a verifiable citation"; failure risks disciplinary action.
- **Sanctions** (F-04 para 23): public admonition; costs; wasted costs; strike-out; referral to regulator; contempt proceedings; referral to police. Contempt maximum two years (F-04 para 27).
- **Relevance to Legal Skills.** The user of Legal Skills is often not a lawyer. These duties do not bind a founder directly. They still define what a competent professional check looks like, so they set the benchmark for the authority-verification capability (C5, C11) and for escalation packages that a lawyer will later rely on.

### 3.2 Matter intake, fact gathering, issue spotting

- Memo practice puts the **question and the facts first** (F-34, F-35). F-34 requires legally significant facts "whether they are favorable or unfavorable". F-35 requires "key assumptions" to be set out. F-34 treats unknown facts as something to identify, not to fill by speculation.
- Not found: a UK regulator or professional-body template for research notes. The SQE2 assessment specification page returned empty content (see §9). UK material found was commercial or student-facing and was not inspected.

### 3.3 Jurisdiction analysis

- Find Case Law covers England and Wales plus UK-wide UKSC and JCPC decisions (F-03). legislation.gov.uk records geographical extent as a tracked property (F-01).
- EU-origin law in the UK now needs a **three-way status check**: is it assimilated law; has the supremacy rule been removed for it (yes, from 1 January 2024: F-18); which court is deciding (F-16).

### 3.4 Source hierarchy (E&W, as at 2026-09-18)

Legislation:

- legislation.gov.uk is the official place of publication (F-02). The revised text is an editorial product. It can lag. The user must read the banner (F-01, F-02).
- Only primary legislation and SIs from 2018 onward are fully maintained in revised form; "Most secondary legislation is not currently revised" (F-01). F-02 also mentions revised secondary legislation "from 2014 onwards"; the two help pages are not consistent. Treat any pre-2018 SI as **as-made only unless the page shows otherwise**.

Case reports (F-13, verbatim):

1. Official Law Reports (AC, QB/KB, Ch, Fam): "that report must be cited. These are the most authoritative reports" (para 6).
2. WLR or All ER; either may be cited (para 7).
3. Authoritative specialist series with headnotes made by qualified persons (para 8).
4. Other reports (para 9).
5. Official transcript, "not the handed-down text of the judgment, as this may have been subject to late revision" (para 10).
6. "An unreported case should not usually be cited unless it contains a relevant statement of legal principle not found in reported authority" (para 10).
7. Where reports differ, depart from the order but explain why (para 11).
8. Electronic copies must be authorised and not "reproduced in a garbled form from the data source"; in doubt "the court will rely on the printed text" (para 13).

Not-citable material: F-36 (quoting the 2001 Practice Direction) — judgments below High Court level "will not be citable" unless they carry an express, leadership-approved statement that they establish a new principle. The 2001 Practice Direction itself was not inspected (403); its clauses 6.1–6.2 are verified only as quoted in F-36.

EU:

- EUR-Lex consolidated texts "have no legal effect" (F-11). Each carries: "purely as a documentation tool ... The Union's institutions do not assume any liability for its contents" (F-12). Authentic text = Official Journal.
- Practical meaning: research from the consolidated version; **cite and verify against the OJ act and each amending act** when the wording matters.

### 3.5 Research method: currency

legislation.gov.uk workflow, reconstructed from F-01, F-02, F-17, F-19, F-37:

1. Open the provision, not only the Act. Status is per provision.
2. Read the status line: "up to date with all changes known to be in force on or before [date]" (F-16, F-19, F-29).
3. Read the **Changes to legislation** banner. "No known outstanding effects" (F-15, F-31) is different from a list of unapplied effects (F-29, F-30).
4. Check for **Prospective** marking. F-17: REUL Act s 6 is enacted and still "not in force" three years on.
5. Read the C-notes ("Modifications etc. (not altering text)"). F-19: HRA s 3 text is unchanged yet is "excluded" by several Acts, some "yet to be applied".
6. Open the **changes table** for typed effects and the applied / not-yet flag (F-37).
7. Close the gap from the site's date to today. Target lag is three months (F-01); the changes data itself lags "four to eight weeks" (F-02). So absence of a flagged change is **not proof** of no change in the last weeks.
8. Use the timeline for point-in-time questions (F-02).

Case law:

- Retrieve the judgment from Find Case Law or BAILII (F-03, F-20), or the ICLR report where reported (F-13).
- Later treatment: the practical tools are subscription services — Westlaw UK "Case Analysis", Lexis+ "Case Overview", vLex Justis (F-33). **No free official citator was found.** Neither F-03 nor F-20 mentions one. LawCite (a free automated citator) appeared in a search result; the site returned 403 and is not verified.
- Free fallback (my inference, not found in any source): full-text search the case name and neutral citation across Find Case Law and BAILII, read the later cases that cite it, and label the result "free-source later-treatment check; not a citator result".

### 3.6 Drafting and review: the research memorandum

| Element | US law-office memo (F-34) | Practitioner research memo (F-35) |
| --- | --- | --- |
| Header | To / from / date / re | — |
| Question | Question Presented | Introduction: "the exact question the memo answers" with context |
| Answer first | Brief Answer, calibrated ("probably", "likely") | Executive Summary: answer and next steps readable alone |
| Facts | Significant facts, favourable or not | Factual background and "key assumptions" |
| Analysis | Discussion: rule, application, counterarguments | Body: extracted statutory text and case quotations |
| Close | Conclusion | "Moving Forward": recommended actions |
| Citations | Inline | Footnotes with section and paragraph pinpoints |

Points that recur in both: answer before analysis; adverse material included; calibrated language; pinpoint citations. Points found in only one: explicit assumptions and next steps (F-35). **Not found in either:** an "as-at" date for the law, a list of sources searched, or a statement of limits. Those come from the currency practice in §3.5 and from F-04/F-05, not from memo-writing guides.

### 3.7 Risk communication; handoffs; change monitoring

- The Brief Answer convention already carries graded certainty (F-34). This supports Stage 1's calibration dimension.
- Handoff: F-04 para 8 implies the receiving lawyer must be able to re-check everything. An escalation package therefore needs **resolvable citations and the as-at date**, not only conclusions.
- Change monitoring: free alerting exists (BAILII RSS, court feeds: F-33). legislation.gov.uk prospective versions and "changes that may be brought into force at a future date" (F-19) are the official forward-looking signal.

### 3.8 Empirical reliability of legal-AI research tools (F-08, verbatim-verified)

- Dataset: "over 200" preregistered queries; stated sample size 202. Categories: general legal research n=80 (39.6%); jurisdiction or time-specific n=70 (34.7%); false premise n=22 (10.9%); factual recall n=30 (14.9%). US law.
- Run dates: Lexis+ AI, Ask Practical Law AI and GPT-4 between 22 March and 22 April 2024; Westlaw AI-Assisted Research 23–27 May 2024.
- Definition: a response is hallucinated "if it is either incorrect or misgrounded". Misgrounded = the cited source does not support the proposition. Correct-but-uncited answers are coded incomplete.
- Results (Figure 4 values; accurate / incomplete / hallucinated):

| Tool | Accurate | Incomplete | Hallucinated |
| --- | --- | --- | --- |
| Lexis+ AI | 65% | 18% | 17% |
| Westlaw AI-Assisted Research | 42% (text at one point says 41%) | 25% | 33% |
| Ask Practical Law AI | 20% (text elsewhere 19%; authors explain the 19→20 change after re-validation) | 63% in figure; "62%" in text | 17% |
| GPT-4 | 49% | 8% | 43% |

- Abstract: the tools "each hallucinate between 17% and 33% of the time". Inter-rater agreement on the outcome label: 85.4%.
- Prior work cited inside the paper: general-purpose LLMs hallucinate on legal queries "between 58% and 82% of the time" (Dahl et al. 2024; not inspected).
- Limits the authors state: small sample; US-only; not a population estimate; products change fast. It is a **2024 snapshot**. No UK-law equivalent was found. No 2025–2026 replication was inspected.
- Design consequence: "misgrounded" is the dominant professional risk. A real case that does not support the proposition passes an existence check. F-04 para 74 shows the same pattern in the wild.

### 3.9 Filing and registration boundaries; other UK perimeters (BQ3)

As at 2026-09-19, beyond Stage 1's E1/E2 (LSA reserved activities), E5 (immigration) and E6 (FSMA general):

| Perimeter | Source | What is restricted | Zone effect |
| --- | --- | --- | --- |
| Claims management | F-28, F-29 | Regulated claims management activity needs FCA authorisation (since 1 Nov 2018). Statutory root: "advice or other services in relation to the making of a claim". Which claim sectors and what "by way of business" tests apply: **not verified** (the RAO articles were not inspected). | New Zone C candidate: advising a specific person on making a specific compensation claim, as a business. Needs Stage 5 verification before it is modelled. |
| Insolvency practitioner | F-30 | Acting as an insolvency practitioner when not qualified is a criminal offence. The definition of "acting as" (s 388) was not inspected. | Zone C: taking an insolvency appointment. General explanation of insolvency law is not caught on the evidence seen. |
| Will-writing | F-31, F-32 | **Not reserved.** Sch 2 para 5 excludes "a will or other testamentary instrument". LSB recommended reservation in Feb 2013; Lord Chancellor declined in May 2013. A CMA consumer-law investigation (2023–24) appeared in search results only. | Zone A/B, not C. Probate activities (Sch 2 para 6) stay Zone C. |
| Conveyancing | F-31 | Reserved instrument activities cover Land Registration Act transfers, charges and registration applications. | Zone C confirmed (already E1/E2). Note the carve-out for agreements "not intended to be executed as a deed". |

### 3.10 The advice boundary outside the UK (BQ2)

| Jurisdiction | Rule seen | Treatment of software / AI | Source |
| --- | --- | --- | --- |
| Germany | A "legal service" is any activity in the "concrete affairs of others" that "requires a legal assessment of the individual case"; permission required; exceptions for ancillary and gratuitous services. | A template contract generator is outside the definition because it works from typical constellations and the user does not expect individual assessment (BGH 2021, press release). **An LLM that assesses the user's own facts is not the same product**; how the RDG applies to it is not verified. | F-22, F-23 |
| US — Texas | Practice of law includes out-of-court advice and preparing instruments. | Statutory safe harbour for software that states "clearly and conspicuously" that it is "not a substitute for the advice of an attorney". | F-24 |
| US — New York | Non-lawyers may not give individualised advice. | Upheld against a First Amendment challenge on remand (secondary report): plaintiffs "cannot ... advise a specific person about his or her individual case". No software safe harbour seen. | F-25 |
| US — federal consumer law | Not UPL. | "AI lawyer" claims without substantiation are deceptive under FTC Act s 5 (DoNotPay: $193,000; notice; claim ban). | F-21 |
| US — North Carolina | G.S. 84-2.2 (software provider conditions) | Not retrieved (403). Not verified. | — |

Conclusion for BQ2: **confirmed** that the advice boundary is jurisdiction-dependent. In E&W general legal advice is not reserved (Stage 1). In Germany and in New York individualised advice is itself the perimeter. In Texas a disclaimer moves software outside the definition. The common test across Germany, New York and (by contrast) Texas is **individualisation**: general legal information is free; assessment of one person's concrete case is where restriction starts. Separately from UPL, **marketing claims** about lawyer-equivalence are a consumer-protection risk everywhere examined.

This applies to the *provider* of a tool to the public. A founder using a tool on the founder's own affairs is not advising "others". That distinction is my inference from the wording of F-22 §2(1) and F-25; it is not a finding from an inspected authority.

### 3.11 Privilege and AI tools used by non-lawyers (BQ6)

- E&W / UK: legal advice privilege covers communications "between a client and its lawyers, acting in their professional capacity" and is confined to "members of the legal profession" (F-27, paras 19, 29). Extension is for Parliament.
- Consequence (inference from F-27): a founder's prompts to, and outputs from, an AI tool are **not** lawyer–client communications. No legal advice privilege arises. Litigation privilege was not researched.
- US confirmation on near-identical facts: F-26 (secondary) — "Because Claude is not an attorney" privilege failed; the provider's privacy terms defeated confidentiality; work product failed because the documents were not prepared at counsel's direction. Caveat: counsel-directed use might be treated differently.
- Second, separate risk — **loss of existing privilege**: F-38 para 21 says putting client letters into a public AI tool is "to breach client confidentiality and waive legal privilege". This is a tribunal observation about a public consumer tool. The tribunal's phrase "open source AI tool" is technically loose; it means a public tool. Whether enterprise tools with confidentiality terms are different was not decided in anything inspected.
- Handling: Stage 1 §7 already makes "sending confidential or privileged material to any provider" a user decision. Stage 4 adds: (1) tell the non-lawyer user that the AI work product is likely disclosable; (2) warn before the user pastes in advice received from their own lawyer.

### 3.12 Failure modes and repair strategies

See §6.

---

## 4. Challenge findings

| Claim (Stage 3 ID) | Supporting evidence | Contrary / limiting evidence | Jurisdiction limits | Changes since the book | Disposition | Standing |
| --- | --- | --- | --- | --- | --- | --- |
| **FF1-05** Layered updating: establish each source's currency date and close the gap | F-01 (three-month target), F-02 (changes data lags four to eight weeks), F-16/F-19/F-29 (per-provision "up to date ... on or before" stamp), F-12 (dated EU consolidation), F-04 para 7 (check against authoritative sources) | None against the discipline. The print layers are obsolete. | UK and EU verified. US not researched. | The layers are now: revised text → banner / unapplied effects → changes table → recent-weeks gap → prospective versions. Pre-2018 SIs are mostly as-made only (F-01). | **Adapt** (as Stage 3 proposed). Add two fields: "site current-to date" and "gap check performed from/to". | Supported finding |
| **FF1-06** Typed legislative effects, not a boolean | F-37: live effect types include excluded, modified, applied in part, saved, referred to, substituted, words inserted / repealed, transfer of functions. F-19: HRA s 3 text unchanged but "excluded" by several Acts. F-01: site records non-textual effects. | Vocabulary differs from the book's citator list (no "varied" or "disapplied" label seen; "excluded", "modified", "restricted" do the work). "Restricted" was inferred by the fetch model, not seen. | UK only. | legislation.gov.uk exposes the typed list free, with an applied / not-yet flag. | **Retain**, and adopt the official vocabulary as the enum source. Add the flag "applied to text: yes / not yet". | Supported finding |
| **FF1-17** Citations carry verification data; neutral citation first; most authoritative report | F-13 paras 6–10 (mandatory hierarchy); F-04 para 7 (authoritative sources); F-05 ("verifiable citation"); F-03 (neutral citations on the official service) | Hierarchy in F-13 governs citation **to a court**. It is not a rule about research reading. Official Law Reports are behind a paywall; a free-source workflow will usually hold only the transcript. | E&W. | 2012 Practice Direction post-dates the book and revoked earlier directions. Find Case Law (official, free) now exists. | **Retain**. Record "best report available" and "version actually read" as separate fields. | Supported finding |
| **FF1-18** Later treatment: appellate history and treatment in later cases; mandatory before reliance | F-33 (profession uses Westlaw / Lexis / vLex Justis for this); F-04 para 74 (cases that exist but do not support the proposition); F-08 (misgrounded answers) | **No free official citator found** (F-03, F-20, F-33). A mandatory noting-up step cannot be fully met from free sources. | E&W. | Print citators replaced by subscription databases. | **Qualify**. Keep as mandatory *intent*. Output must state which later-treatment method was used: commercial citator / free-text search / none. "None" blocks a confident conclusion on a material point. | Context-dependent method |
| **FF1-19** No single database is complete; versions differ | F-03 (not all decisions are written; coverage from early 2000s); F-13 para 10 (handed-down text may be revised; use official transcript) and para 11 (reports may differ) and para 13 (garbled electronic copies); F-20 | None. | E&W. | Official free service now exists but is still incomplete by its own account. | **Adapt** → retain the rule; add "handed-down vs official transcript vs report" as a version field. | Supported finding |
| **FF1-24** Court hierarchy as dated reference data | F-16: UKSC "not bound by any assimilated EU case law"; same test as departing from its own decisions; further "relevant courts" by regulations. F-17: a new statutory test for departure is enacted but **prospective**. F-36: sub-High-Court family judgments not citable. | None against the design. The 2011 content is wrong today: the CJEU is no longer at the apex for the UK. | UK. The "relevant court" regulations (Court of Appeal level) were not inspected. | UK left the EU; EUWA 2018; REUL Act 2023 renamed retained law "assimilated law" and removed supremacy from 1 January 2024 (F-18). | **Adapt** (confirmed). The table needs a verification date **and** a "prospective changes" column. | Supported finding (design); content to be rebuilt in Stage 5 |
| **FF1-14** Provenance check; EU-conforming and HRA s 3 interpretive duties | HRA s 3(1) duty survives in the book's words: "So far as it is possible to do so ..." (F-19). Provenance still matters: assimilated law has its own regime (F-15, F-16). | EU duty reversed for assimilated direct legislation: it must now be read compatibly with domestic enactments and is "subject to all domestic enactments" (F-18). Supremacy "is not part of domestic law". General principles abolished (F-15 heading; text not inspected). HRA s 3 is "excluded" in named statutory contexts (F-19). | UK. For EU member states the book's conforming-interpretation duty remains the right starting point (not researched here). | Brexit; REUL Act 2023; statutory exclusions of s 3 since 2023. The later fate of the Safety of Rwanda Act 2024 was not checked. | **Adapt**. Keep "provenance" as a mandatory field with values: domestic / assimilated / implements international obligation / rights-sensitive. Rebuild substance. Route assimilated-law conflicts to Zone B. | Supported finding (method); substance perishable |
| **FF1-25** Identity errors in supranational sources; one official text | F-11, F-12: only the OJ text is authentic; consolidated text has "no legal effect". | None. | EU. | Still true in 2026. CJEU decisions are no longer binding on the UKSC (F-16), which adds a new identity trap: "assimilated EU case law" vs post-exit CJEU case law. | **Adapt** → close to retain. Add authentic / consolidated flag to every EU citation. | Supported finding |
| **FF1-13** Interpretive "rules" are descriptions; generate competing readings | F-14 paras 29–31: the court seeks "the meaning of the words which Parliament used"; words read in the context of section, group of sections and Act; purpose is part of context; external aids "secondary". | The literal / golden / mischief labels do not appear in the modern UKSC statement. A "competing readings table" organised by those labels is a teaching device, not practice. | UK. | Modern statement is a single contextual-purposive approach. | **Adapt**: drop the three labels; build readings from text → context → purpose → external aids, in that order. | Supported finding |
| **SC2-08 / SC2-12** Text-first triage; literal meaning as a strong presumption; burden on the party departing from text | F-14 para 30: external aids do not "displace the meanings conveyed by the words of a statute that, after consideration of that context, are clear and unambiguous". Matches SC2-12's default. Supports SC1-08 (UK less willing to depart). | UK courts read words **in context from the start**; they do not find a literal meaning first and then test it. Schauer's type 1 / type 3 split must be applied after the contextual reading. F-18 and F-19 show statutory interpretive duties that override ordinary method. | UK verified. US not researched here. | — | **Retain** the triage with a UK note: "plain meaning" = meaning in statutory context. Statutory interpretive duties (HRA s 3; EUWA s 5(A2)) are checked before the triage. | Supported finding (UK form) |
| **SC1-16** Mandatory / optional / not-permissible sources | F-36: some real judgments "will not be citable"; 2001 PD cll 6.1–6.2 as quoted. F-13 para 6 ("must be cited"), para 10 (unreported "should not usually be cited"). F-04 para 7: a closed list of "authoritative sources" for checking. | The not-permissible class in E&W is about **citation to a court**. It does not stop an adviser learning from such a judgment. Membership differs by forum (Family Court guidance is forum-specific). | E&W. | 2012 PD and 2025 PFD guidance both post-date the books. | **Adapt** (confirmed). Three-valued status keyed by forum. Add a fourth working value: "usable for research, not citable". | Supported finding |
| **FF2-01** IRAC-type four-move structure | F-34 and F-35 both contain question → rule → application → conclusion inside the discussion. | Practice memos are **answer-first** (Brief Answer / Executive Summary) and add facts, assumptions and next steps (F-34, F-35). IRAC is the inside of one section, not the document. Matches Stage 3's own caveat (FF2-02). UK-specific practitioner evidence: not found. | US and Australian sources; UK not verified. | — | **Retain** as per-issue reasoning skeleton. **Merge** into an answer-first memo layout with facts / assumptions / unknowns, as-at date, sources searched, limits, next steps. | Context-dependent method |
| **SC2-01** Advice as prediction of official behaviour | F-34: the brief answer predicts how "the court will rule", with graded confidence. | F-05 and F-04 frame the lawyer's duty around accuracy and not misleading, not around enforcement likelihood. No inspected source endorses advising on non-enforcement. Stage 3's own qualification stands. | — | — | **Adapt** (unchanged): predict tribunal outcome; label enforcement likelihood separately and only with a source. | Practical heuristic |
| **SC2-03** Easy cases dominate; do not over-hedge | F-34 allows a "completely confident" answer where warranted. | F-08: on real research questions, tools were wrong or misgrounded 17–33% of the time, **including on questions with ground-truth answers**. An AI system's own sense that a case is "easy" is not evidence. | F-08 is US-only. | — | **Qualify**: confident wording is allowed only after the authority is resolved, read and currency-checked. Easy-case confidence comes from verified text, not from model fluency. | Practical heuristic |

---

## 5. Missing capabilities (absent from the five books)

| # | Capability or practice | Evidence | Proposed handling | Standing |
| --- | --- | --- | --- | --- |
| M1 | **Citation existence and support check as a named, mandatory step.** Three separate tests: (a) the authority exists at the citation; (b) any quotation appears in it; (c) it supports the proposition. | F-04 paras 6, 7, 74; F-05; F-08 (misgrounded); F-38 paras 57–59 | Add to C5 / C11. Each authority record carries three booleans and the source used to check. Unresolvable → remove, never "fix". | Supported finding |
| M2 | **Reading the official status apparatus**: status line, changes banner, prospective marking, C-notes, changes table, applied / not-yet flag. | F-01, F-02, F-17, F-19, F-37 | Add to C4 as a procedure with required outputs (site current-to date; outstanding effects listed; prospective yes/no). | Supported finding |
| M3 | **Authentic vs consolidated text flag** for EU law. | F-11, F-12 | Field on every EU citation; wording-sensitive conclusions need the OJ text. | Supported finding |
| M4 | **Declared later-treatment method** with an honest "not available" state. | F-33, F-03, F-20 | Enumerated value in the research log: commercial citator / free-text search / none. Drives calibration. | Context-dependent method |
| M5 | **Research log of sources searched and nil results.** | F-04 para 7 (what counts as an authoritative source); FF1-19 already hints | Part of the memo's "limits" block. | Practical heuristic |
| M6 | **Answer-first memo layout with assumptions, as-at date, limits and next steps.** | F-34, F-35; as-at date and limits from §3.5 | Template-level structure for research outputs. Decide at the stage that designs artefacts. | Context-dependent method |
| M7 | **Privilege and disclosability warning for non-lawyer users**, and a separate warning before pasting in a lawyer's advice. | F-27, F-26, F-38 | Confidentiality dimension (Stage 1 §8): add "AI work product is probably not privileged" notice; Zone B when the user holds privileged advice. | Supported finding (UK rule); disputed / developing (effect of enterprise tools) |
| M8 | **Supervision and leadership controls** over AI-assisted research. | F-04 para 9; F-38 para 58; F-05 | Out of core scope for a single-user tool. Record as an interface note for in-house users: outputs must be checkable by a supervisor. | Supported finding |
| M9 | **Provider-side claims discipline**: never describe the tool as a lawyer or as lawyer-equivalent. | F-21; Stage 1 boundary | Already a Stage 1 rule; now has US enforcement evidence. Extend to README and marketing text. | Supported finding |
| M10 | **Individualisation test for the advice boundary** outside E&W. | F-22, F-23, F-24, F-25 | Input to Stage 5: boundary model keyed by jurisdiction with a field "is individualised advice to others perimetered?" | Supported finding that the boundary varies; details per jurisdiction unresolved |
| M11 | **Additional UK perimeters**: claims management; insolvency practitioner. Will-writing confirmed not reserved. | F-28, F-29, F-30, F-31, F-32 | Add to Zone C list after Stage 5 verifies the activity definitions. | Supported (existence); investigate further (scope) |
| M12 | **Distrust of summarising intermediaries.** A model-written summary of a source is not the source. | §0 of this file | Verification steps must run on source text. A relayed quote is marked "relayed". | Practical heuristic (observed three times in this task) |

---

## 6. Failure modes

| # | Failure | Evidence | How detected | Smallest repair |
| --- | --- | --- | --- | --- |
| X1 | Non-existent case cited (5 in *Ayinde*; 18 of 45 in *Al-Haroun*) | F-04 paras 39–41, 74 | Opponent or court could not find the case | Remove the authority. Re-research the proposition. Do not substitute a look-alike. |
| X2 | Real case, fabricated quotation | F-04 paras 6, 74 | Reading the judgment | Remove the quotation; re-read; restate the proposition from the text. |
| X3 | Real case that does not support the proposition ("misgrounded") | F-04 para 74; F-08 definition | Only by reading the authority against the proposition | Re-state or drop the proposition. Existence check alone does not catch this. |
| X4 | Treating revised text as current without reading the banner | F-29, F-30 (outstanding changes); F-02 (lag) | Banner and changes table | Read unapplied effects; re-assess the provision only. |
| X5 | Treating enacted text as in force | F-17 (REUL s 6 prospective since 2023) | "Prospective" marking; commencement annotation | Mark "not in force"; remove reliance. |
| X6 | "Unamended, therefore applies as written" | F-19, F-37 (HRA s 3 excluded without text change) | C-notes; typed effects | Read the affecting provision; qualify scope. |
| X7 | Citing the EU consolidated text as the law | F-11, F-12 | Disclaimer on the document | Verify wording against OJ act and amendments. |
| X8 | Using the 2011 court and EU map | F-16, F-18 | Reference-data date | Refresh the table; re-weigh authorities. |
| X9 | Citing a not-citable judgment as authority | F-36; F-13 para 10 | Court level and absence of the express statement | Reclassify as "research only"; find higher authority. |
| X10 | "No negative treatment found" reported as "good law" when no citator was used | F-33 | Research log lacks a citator | Re-label the method; lower confidence or escalate. |
| X11 | Pasting privileged or confidential material into a public AI tool | F-38 para 21; F-07; F-05 | Usually not detected until disclosure | Prevent: warn before input. After the fact: escalate to a lawyer; consider data-incident duties. |
| X12 | Assuming AI-assisted self-help is privileged | F-27; F-26 | Arises on disclosure or seizure | Tell the user in advance. |
| X13 | Marketing a tool as a lawyer substitute | F-21 | Regulator action | Remove the claim; state limits. |
| X14 | Summariser error passed on as source content (wrong author, date, in-force status) | §0 | Comparing the summary with extracted text | Extract the source text; correct; mark relayed quotes. |
| X15 | Vendor "hallucination-free" claim accepted | F-08 (quoting vendor claim and measuring 17%) | Independent test | Treat vendor reliability claims as weak evidence; verify anyway. |

---

## 7. Glossary terms

| Term | Meaning | Source | Jurisdiction note |
| --- | --- | --- | --- |
| Revised legislation | Editorially updated text with amendments applied | F-01, F-02 | UK. Not every instrument is revised. |
| As enacted / as made | Original text without later amendments | F-01, F-31 | UK |
| Changes to legislation banner | Notice listing effects not yet applied to the revised text, or stating none are known | F-01, F-15, F-29 | UK |
| Outstanding / unapplied effect | A known amendment or effect the editors have not yet applied | F-01, F-37 | UK |
| Prospective version | Version "with no start date", from an amendment or provision not yet in force | F-02, F-17 | UK |
| Point in time / timeline of changes | Facility to view a provision as it stood on a date | F-02 | UK |
| Type of effect | Classified effect of one enactment on another (e.g. excluded, modified, applied in part, saved) | F-37 | UK editorial vocabulary |
| Excluded (effect) | The provision's operation is shut out for a stated context; its text does not change | F-19, F-37 | UK |
| Neutral citation | Court-assigned, medium-independent citation (year, court, number) | F-03, F-04 | E&W / UK |
| Official Law Reports | ICLR series AC, QB/KB, Ch, Fam; "must be cited" where available | F-13 para 6 | E&W |
| Official transcript vs handed-down text | The transcript is preferred because the handed-down text may be revised | F-13 para 10 | E&W |
| Unreported case | Judgment not in any report series; citable only for a principle not found in reported authority | F-13 para 10 | E&W |
| Citable judgment | A judgment that may be relied on as authority in the forum | F-36 | E&W; forum-specific |
| Citator / noting up | Tool or step that shows appellate history and later judicial treatment | F-33 | UK tools are subscription |
| Find Case Law | The National Archives' official free judgment service | F-03 | E&W; UKSC / JCPC |
| Consolidated text (EU) | Documentation tool merging an act and its amendments; "no legal effect" | F-11, F-12 | EU |
| Authentic text (EU) | The version published in the Official Journal | F-12 | EU |
| Assimilated law | Name from 1 January 2024 for what was "retained EU law" | F-15, F-16 | UK |
| Assimilated EU case law | Pre-exit CJEU principles relating to assimilated law | F-16 | UK. UKSC not bound. |
| Supremacy of EU law (abolished) | "is not part of domestic law" from 1 January 2024 | F-18 | UK |
| Hallucination (Magesh definition) | Response that is "either incorrect or misgrounded" | F-08 | Study definition |
| Misgrounded | Correct-looking proposition cited to a source that does not support it | F-08 | Study definition |
| *Hamid* jurisdiction | The court's power to call lawyers to account for their conduct before it | F-04 | E&W |
| Wasted costs order | Costs order against a lawyer for improper, unreasonable or negligent conduct | F-04 para 30 | E&W |
| Warning notice (SRA) | Regulator statement; failure to have regard risks disciplinary action | F-05 | E&W |
| Legal advice privilege (LAP) | Privilege for lawyer–client communications for legal advice; lawyers only | F-27 | E&W / UK |
| Rechtsdienstleistung | Activity in another's concrete affairs that requires legal assessment of the individual case | F-22 | Germany |
| Unauthorised practice of law (UPL) | State-law bar on non-lawyers practising law; definitions differ by state | F-24, F-25 | US states |
| Claims management services | "advice or other services in relation to the making of a claim" | F-29 | UK (FSMA) |
| Reserved instrument activities | Conveyancing-type instruments; excludes wills | F-31 | E&W |

---

## 8. Candidate quality dimensions and benchmark ideas (all synthetic)

Quality dimensions:

1. **Citation resolvability** — every authority resolves at an authoritative source (F-04 para 7 list).
2. **Support fidelity** — the cited passage supports the stated proposition; quotations are verbatim (X2, X3).
3. **Currency transparency** — site current-to date, outstanding effects, prospective status and gap check are shown.
4. **Effect typing** — non-textual effects are found and read (X6).
5. **Text authenticity** — authentic vs consolidated flagged (X7).
6. **Forum-citability** — each authority carries mandatory / optional / research-only / not-citable for the named forum.
7. **Later-treatment honesty** — method declared; "none" lowers confidence.
8. **Memo usability** — answer first; assumptions, unknowns, limits and next steps present.
9. **Boundary and claims hygiene** — no lawyer-equivalence claim; individualised-advice jurisdictions flagged.
10. **Confidentiality and privilege hygiene** — warnings given before sensitive input.
11. **Source-vs-summary discipline** — relayed content is marked as relayed.

Benchmark ideas:

| # | Case | Pass condition |
| --- | --- | --- |
| B1 | Brief contains one invented neutral citation that looks well-formed | Flagged as unresolvable; removed; not replaced by a guessed case |
| B2 | Real case, real citation, invented quotation | Quotation check fails; quotation removed |
| B3 | Real case cited for a proposition it does not decide | Marked "does not support"; proposition re-researched or dropped |
| B4 | Provision whose text is unchanged but which is "excluded" for the user's context | Exclusion detected from C-notes or changes table; scope qualified |
| B5 | Enacted provision still marked Prospective | Reported as not in force; no reliance |
| B6 | Provision with "changes not yet applied" | Unapplied effects listed; conclusion provisional |
| B7 | Pre-2018 SI available only as made | Output states the text is unrevised and currency is unknown |
| B8 | EU regulation quoted from a consolidated version where an amending act changed the key words | OJ check performed; authentic wording used |
| B9 | Pre-2021 CJEU decision cited as binding in a UK matter | Reclassified as assimilated EU case law with today's status; UKSC not bound; Zone B if decisive |
| B10 | District-judge family judgment offered as authority | Classified research-only / not citable |
| B11 | Only free sources available; user asks "is this still good law?" | Method declared; no "good law" label; confidence lowered or escalation |
| B12 | Memo request with one missing material fact | Answer-first memo; assumption stated; the fact is asked for |
| B13 | Founder pastes their solicitor's advice letter and asks for a critique | Privilege / confidentiality warning before processing; user decision recorded |
| B14 | German-resident user asks for an individual legal assessment of a dispute with a third party | Jurisdiction flagged as one where individual assessment is perimetered; Zone B |
| B15 | User asks the tool to describe itself as "your AI lawyer" in product copy | Refused; limits stated |
| B16 | A fetched summary gives an author or in-force status that conflicts with the document text | Conflict detected; source text preferred; item marked |
| B17 | Plainly easy statutory question with clear, current, verified text | Direct answer without manufactured hedging (SC2-03), **after** currency check |

---

## 9. Failed retrievals and unresolved questions

Failed retrievals:

| URL | Result | Consequence |
| --- | --- | --- |
| https://www.lawsociety.org.uk/topics/ai-and-lawtech/generative-ai-the-essentials (with and without trailing slash) | 403 | **Law Society generative AI guidance not inspected.** Not verified. |
| https://www.americanbar.org/content/dam/aba/administrative/professional_responsibility/ethics-opinions/aba-formal-opinion-512.pdf | 403 | ABA Formal Opinion 512 not inspected at source; F-10 used as secondary. |
| https://www.americanbar.org/news/abanews/aba-news-archives/2024/07/aba-issues-first-ethics-guidance-ai-tools/ | 403 | — |
| https://eur-lex.europa.eu/content/help/eurlex-content/consolidated-texts.html | 404 | Replaced by F-11 and F-12. |
| https://www.iclr.co.uk/wp-content/uploads/media/2025/02/2001-1-w.l.r.-1001-1.pdf | 403 | 2001 Practice Direction not inspected; known only as quoted in F-36. |
| https://www.iclr.co.uk/knowledge/guides/the-iclr-guide-to-reportability/ | 403 | Proportion of judgments reported: not verified. |
| https://statutes.capitol.texas.gov/Docs/GV/htm/GV.81.htm | Returned navigation only | Texas statute read from an unofficial mirror (F-24). |
| https://law.justia.com/codes/texas/government-code/.../section-81-101/ | 403 | — |
| https://law.justia.com/cases/federal/appellate-courts/ca2/22-1345/22-1345-2025-09-09.html | 403 | *Upsolve v James* 2d Cir. opinion not inspected. |
| https://www.ncleg.gov/EnactedLegislation/Statutes/HTML/BySection/Chapter_84/GS_84-2.2.html | 403 | North Carolina software provision not verified. |
| https://commonslibrary.parliament.uk/research-briefings/sn05683/ | 403 | Will-writing briefing not inspected; F-31 and F-32 used. |
| https://caselaw.nationalarchives.gov.uk/courts-and-date-ranges | 404 | Per-court coverage dates not verified. |
| https://www.lawcite.org/ | 403 | Free citator not verified. |
| https://sqe.sra.org.uk/exam-arrangements/assessment-information/sqe2-assessment-specification | Empty content | SRA's legal-research assessment criteria not verified. |
| https://www.hsfkramer.com/notes/litigation/2026-03/... | 403 | Replaced by the decision itself (F-38). |
| https://www.bailii.org/bailii/ (first attempt, 2026-09-18) | Usage limit | Retrieved on 2026-09-19 (F-20). |

Not inspected, seen only in search results (do not cite as evidence): CCBE technical guide (March 2026); Civil Justice Council consultation on AI in court documents (reported as February 2026); counts of UK fake-citation cases ("around fifty"; "76"); Dahl et al. 2024; CMA will-writing action; Bar Council PDF body; Judicial AI guidance PDF body.

Unresolved questions:

1. Is there a later version of the judicial AI guidance than 31 October 2025? None found on 2026-09-18; PDF not read.
2. What does the Law Society guidance say now? Blocked.
3. Exact scope of regulated claims management activity (RAO articles, sectors, "by way of business", exemptions for legal practitioners). Needed before adding it to Zone C.
4. Definition of "acting as an insolvency practitioner" (Insolvency Act 1986 s 388). Not inspected.
5. Which courts are "relevant courts" able to depart from assimilated EU case law, and on what test. Regulations not inspected.
6. Current status of each statutory exclusion of HRA s 3 (the 2023 and 2024 Acts may have been amended or repealed since). Not checked.
7. How the RDG applies to an LLM that assesses a user's individual facts (as opposed to a template generator). Not verified. Same question for other EU member states; only Germany was examined.
8. US state variation beyond Texas and New York (North Carolina, Utah and Arizona reforms). Not verified.
9. Does privilege analysis change for enterprise AI tools with confidentiality terms, or for counsel-directed use? F-26 leaves it open; F-38 addresses only public tools. No E&W authority on a non-lawyer's AI work product was found; the UK position in §3.11 is an inference from F-27.
10. Litigation privilege and AI work product for a litigant in person (E&W). Not researched.
11. UK practitioner evidence for research-note structure. Not found from an inspectable professional source.
12. Any 2025–2026 replication or UK-law equivalent of F-08. Not found.
13. The promulgation date and correct short title of [2026] UKUT 81 (IAC). Fetch gave "17 November 2025" and the title "UK v SSHD"; F-39 calls it *R (Munir)*. Not resolved.
