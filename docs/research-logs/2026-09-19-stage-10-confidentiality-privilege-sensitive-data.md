# Stage 10 — Confidentiality, Privilege and Sensitive-Data Handling

**Stage:** 10 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 11  
**Governing section:** §16 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 1 (E4 SRA notice; Q6); Stage 4 (N21, C28, gaps G5, G6; log f §3.11); Stage 6 (A1 `sensitivity`; A8 routing); Stage 9 (trigger T17)

Supporting records:

| Log | Content | Inspected sources |
| --- | --- | --- |
| `2026-09-19-stage-10a-provider-data-handling.md` | Provider and tool data handling (evidence prefix `H-`) | 52, all read as raw page text |
| `2026-09-19-stage-10b-confidentiality-privilege.md` | Professional and legal rules (evidence prefix `I-`) | 39; 36 raw-text-verified, 3 fetch-summary only |

**Everything in this log is valid only as of 19 September 2026.** Provider terms changed at least twelve times in the preceding eighteen months (log a §3.8(c)); one change was nine days old when read. No statement here is a timeless property of a provider. A routing rule must cite a dated evidence ID and be re-verified before reliance.

---

## 1. Method and limits

1. Two research agents worked under the Stage 4 method rules. Because the fetch tool had been caught inventing and reversing content, both were told to read raw text. Stream H used no model-written summaries. Stream I downloaded and extracted 36 of 39 sources.
2. Text-verified this time, after failing in Stage 4: the Law Society generative-AI guide; the Bar Council guidance PDF; the judiciary AI guidance PDF (31 October 2025); the *Heppner* opinion itself (SDNY, February 2026); [2026] UKUT 81 (IAC) paragraphs 21 and 60. This closes most of Stage 4 gap G5.
3. Still not read at source: all three SRA pages (the Code paragraphs 6.3–6.5, the confidentiality guidance, the AI warning notice) returned 403 to direct download, so their quotations are "as reported"; ABA Formal Opinion 512; the OpenAI preservation orders; *Three Rivers (No 6)* (read only as quoted in another judgment); the CJEU judgment in *EDPS v SRB* (press release only); provider trust centres and sub-processor lists.
4. One practitioner source misstated the trade-secret test as "all reasonable steps". The regulation says "reasonable steps under the circumstances" (log b). Recorded as another instance of Stage 4 failure class T4.

---

## 2. What the evidence establishes

### 2.1 Providers and tools (log a)

| # | Finding | Evidence | Standing |
| --- | --- | --- | --- |
| P1 | **The consumer / commercial line is the most consequential switch.** On the commercial tiers of all four providers inspected: no training on customer content by default; a data-processing agreement with transfer clauses; deletion of API content on roughly a 30-day horizon, absent a flag or legal hold. | H-12, H-15, H-08, H-25, H-26, H-34, H-39 | Supported finding (dated) |
| P2 | Consumer Claude plans train on chats **unless the user opts out**, may retain for up to five years where training is on, carry no comparable confidentiality undertaking, and the UK consumer terms say "Non-commercial use only". | H-13, H-14, H-01, H-06 | Supported finding (dated) |
| P3 | **Claude Code inherits whichever account is signed in.** A personal plan brings the consumer terms into a work repository. Managed settings can force an organisation login. | H-01, H-02 | Supported finding (dated) |
| P4 | **"Zero data retention" does not mean nothing is kept.** Flagged content is kept up to two years even under that option. The option needs approval and excludes consumer plans and standard team chat. | H-02, H-06, H-08 | Supported finding (dated) |
| P5 | Anthropic's current frontier models (listed as Claude Fable 5 / 5.1 and Mythos 5 / 5.1) are "Covered Models" with a mandatory 30-day minimum retention on every platform; zero retention is unavailable for them unless expressly authorised. AWS documentation confirms this independently. | H-06, H-07, H-22 | Supported finding (dated). *This applies to the model that ran this bootstrap.* |
| P6 | Anthropic first-party inference offers "global" or "us" only. No EU or UK residency option was found. | H-18 | Supported finding (dated) |
| P7 | Anthropic documentation is internally inconsistent on default API retention ("not retained by default" vs "30 days"). | H-06 vs H-08, H-01 | Unresolved → assume 30 days |
| P8 | A court preservation order overrode OpenAI's normal deletion for consumer and non-zero-retention API traffic between May and 26 September 2025. Some data from that period is still held. De-identified logs were ordered produced in January 2026. | H-28, H-35 (provider pages; the orders were not read) | Supported finding (provider's own account) |
| P9 | Gemini API unpaid tier: content is used for training and may be seen by human reviewers; the provider says not to submit sensitive or confidential information. Paid tier: abuse logs kept for 55 days. | Log a §3.3 | Supported finding (dated) |
| P10 | Microsoft 365 Copilot is opted out of abuse monitoring, but models supplied by a sub-processor are excluded from the EU Data Boundary. The Azure OpenAI abuse-monitoring retention period no longer appears on current pages. | Log a §3.4 | Supported / not found |
| P11 | **Provider retention is one of at least four copies.** A single agent turn can leave: provider logs; a local plaintext transcript; search and fetch traces; third-party tool copies. | H-03 to H-06, H-26, H-46 | Supported finding |
| P12 | Claude Code writes every message, tool call and file content it reads to **unencrypted plaintext** transcripts under the user's home directory, swept after 30 days by default. Command history and auto-memory persist until deleted by hand. | H-03, H-04 | Supported finding (dated) |
| P13 | Web tools leak separately. A web search sends the query to the provider's backend. A web fetch sends the host name to the provider and the full URL to the target site. **A search query can itself disclose a confidential fact** (who is asking about what, and when). | H-05; I-30 | Supported finding |
| P14 | Firecrawl caches scrapes (two-day default). Its 2024 privacy policy and terms say nothing about retention of uploaded documents. | H-43 to H-47 | Supported / not found |
| P15 | Local open-weight models keep prompts on the machine, but at least one common server has telemetry **on** by default. Capability limits of local models are a heuristic, not sourced. | Log a §3.6 | Supported / heuristic |
| P16 | **No provider page addresses privilege or solicitor confidentiality.** Anthropic's usage policy treats legal use as high-risk: a qualified professional must review, and AI use must be disclosed to consumers. OpenAI places a similar duty on the user. | H-17; log a §3.8(b) | Supported finding (dated) |

### 2.2 Professional and legal rules (log b)

| # | Finding | Evidence | Standing |
| --- | --- | --- | --- |
| L1 | **Legal advice privilege needs a lawyer.** A non-lawyer's own exchanges with an AI tool about their legal position are not privileged in England and Wales. | F-27 (*Prudential*); I-08 (*Three Rivers (No 5)*) | Decided law (E&W) as to the requirement; its application to AI chats is a direct consequence, not separately decided |
| L2 | Privilege depends on **what the material is**, and confidentiality is a precondition. Putting a lawyer's advice into a public or consumer tool risks loss of confidentiality and waiver. | I-07 (UKUT 81 para 21 — said without argument; does not bind the High Court); I-13 (*Heppner* fn 3, US) | Practical heuristic with judicial support; **not a binding E&W decision** |
| L3 | Whether enterprise confidentiality terms **preserve** privilege when a lawyer's advice is processed by an AI provider is **undecided** in England and Wales and in the US. Limited-waiver cases and one sentence in UKUT 81 about "closed source" tools point towards yes. | I-09, I-07 | **Inference only** |
| L4 | In *Heppner* the court treated a defendant's exchanges with consumer Claude as neither privileged nor work product, relying in part on the provider's privacy policy. | I-13 (opinion read) | Decided (one US district court) |
| L5 | A stored prompt or output is a disclosable "document" under the Civil Procedure Rules. US preservation orders have overridden user deletion. | I-36 (CPR 31.4, 31.8); P8 | Supported finding |
| L6 | Professional bodies' main control is **choice of tool**; redaction is a supplement. The Bar Council, Law Society and judiciary all warn against entering confidential or privileged information into public tools. | I-03, I-04, I-05, I-06 | Supported finding (E&W) |
| L7 | **Client consent:** no inspected E&W source *requires* it. The Law Society advises agreeing AI use with the client and checking the engagement terms. ABA Opinion 512 requires informed consent before client information goes into a self-learning tool — known only through a secondary source. | I-04; I-39 | Context-dependent; US point secondary only |
| L8 | **Guidance conflicts on logs.** The Law Society says to document inputs and outputs. The judiciary and the NCSC say to minimise and to disable history. | I-04 vs I-06, I-30 | Disputed → resolved by design in §6 |
| L9 | **Replacing names does not take a prompt outside UK GDPR** when the provider is your processor: "the status of the data in your hands is what matters". Pseudonymisation is a security measure. The EU position may be more recipient-relative (press release only). | I-23; I-22 | Supported finding (UK); EU unresolved |
| L10 | Redaction does not cure privilege, NDA or live-secret risk, and it can remove legally material detail. | Log b Q7 | Supported finding |
| L11 | Special category and criminal-offence data need stricter handling; a DPIA screening applies; ICO anonymisation and DPIA pages carry "under review" banners. | I-20, I-21, I-24, I-26 | Supported finding; guidance moving |
| L12 | UK–US transfers: the data-bridge regulations show no revocation on legislation.gov.uk, but only the as-made text is published there. Status on 19 September 2026 is **not positively verified**. | I-27 | Unresolved |
| L13 | Trade secrets need "reasonable steps under the circumstances" to stay protected. An approved-tool policy is evidence of such steps. Putting a secret into a tool that may train on it, or a third party's NDA material into any tool without checking the NDA, is a risk. | I-32 to I-35 | Supported (regulation read); the NDA rule is inference |
| L14 | No NCSC document specific to credentials in prompts was found. General NCSC guidance covers data leakage and prompt injection, including exfiltration by agents. | I-29 to I-31 | Supported / not found |

**Stage 1 question Q6 answered:** a founder's AI work product is not privileged in England and Wales (L1). Pasting a solicitor's advice into a consumer tool risks waiver (L2). Whether enterprise terms preserve privilege is undecided (L3). The skill must **ask** whether a lawyer is involved and whether material came from a lawyer; it must not assume.

---

## 3. Sensitivity classes

Adopted from log b §4, which justifies each row with evidence IDs. Material takes the **strictest** class that applies. A stricter route is always allowed.

| # | Class | Examples | Minimum handling |
| --- | --- | --- | --- |
| 0 | Public | Legislation, judgments, guidance; an abstract legal question with no matter context | **P.** Check whether the question itself reveals something (P13). |
| 1 | Privileged material | A lawyer's advice; instructions to lawyers; litigation preparation | Never P. **A or L only.** Non-lawyer user: warn first about waiver and that new AI exchanges are not privileged; suggest asking the lawyer. Redaction does not cure this. |
| 2 | Client-confidential, where the user is a regulated lawyer | Client instructions, documents, matter facts | Never P. **A or L**, with supplier due diligence, engagement terms covering the tool, and minimisation. |
| 3 | Special category or criminal-offence personal data | Health details; alleged offences; immigration decisions | Never P. **R** where identifiers are not legally needed; otherwise **A or L**. DPIA screening. Transfer mechanism checked per provider. |
| 4 | Ordinary personal data | Names, emails, job titles | Not P. **R by default**; otherwise A or L with a processing agreement and transfer check. |
| 5 | Own confidential commercial information and trade secrets | Source code, pricing, roadmap, fundraising terms | Not P where terms allow training or reuse. **A or L**, or R / abstraction. |
| 6 | Third-party confidential information under NDA or contract | Data-room documents; a customer's security answers | **N or R** until the NDA's permitted-recipient and purpose clauses are checked; then A or L only if permitted. Never P. |
| 7 | Live secrets | Credentials, keys, tokens, connection strings | **N always.** Strip before any route, including local logs. No legal task needs the value. |
| 8 | Descriptive security-sensitive material | Unpatched vulnerabilities; incident forensics; security architecture | Never P. **L preferred**; A if staff-access terms are known; abstract to what the legal question needs. |
| 9 | Regulatory, investigation or dispute-sensitive, not privileged | Internal notes on a suspected breach; a non-lawyer's own exposure analysis; draft admissions | Warn: these exchanges are disclosable and not privileged without a lawyer. Prefer a lawyer first (Stage 9 T4). If proceeding: A or L, minimal retention. |

Classes 1 and 9 are the two where the **user's status** changes the legal outcome. The skill asks.

---

## 4. Routes

| Route | Meaning | Conditions |
| --- | --- | --- |
| **P** Public research | Any tool, including consumer tools and web search | Only class 0 content, and only queries that reveal nothing about the matter |
| **R** Redact or abstract, then send | Replace parties with roles; remove identifiers; state the legal question in general form; use synthetic facts | Keep a private key of what was changed. Check that no legally material detail was lost. Does not downgrade classes 1, 6 or 7. Does not remove UK GDPR duties where the provider is a processor (L9). |
| **A** Approved private provider | A provider the user or their organisation has approved against the checklist below | Approval is the user's decision, recorded with a date. Legal Skills never approves a provider. |
| **L** Local execution | Open-weight model on the user's own machine; no web tools | Check telemetry defaults (P15). Expect lower capability and no research. Local transcripts still exist. |
| **N** Non-disclosure | The material is not processed by any AI tool | The workflow continues on what can be shared, or stops and says so |

**Approval checklist for route A** (a checklist, not a brand list; log b §4 note; log a §4):

```text
account type is commercial, not consumer            (verify: the agent inherits the signed-in account)
no training on inputs by default; opt-in only
confidentiality undertaking covers customer content
retention period for inputs and outputs; flagged-content carve-out; legal-hold carve-out
whether zero retention is really available for the model in use
who at the provider may view content, and when
sub-processors and underlying cloud platform
inference and storage location; transfer mechanism for UK / EU personal data
processing agreement in place; breach notification period
what happens under legal process; notice of compelled disclosure
every other tool in the turn meets the same bar      (search, fetch, scrape, connectors)
date checked; evidence IDs; re-check date
```

---

## 5. Routing procedure

```text
before any material leaves the user's machine:
1. classify the material (strictest class wins); ask about lawyer involvement and the origin of
   any advice (classes 1, 9); ask about NDAs for third-party material (class 6)
2. strip class 7 content (pattern-match keys, tokens, connection strings) — always
3. list every tool the turn would use; THE ROUTE IS SET BY THE MOST EXPOSED TOOL, not by the model
4. compare the class's minimum handling with the route actually available:
     available route ≥ required → proceed
     can be met by redaction or abstraction → do that, keep the private key, check nothing material is lost
     cannot be met → stop (Stage 9 trigger T17): say which material, which class, which route is needed
5. web research is a separate disclosure: search with the abstract legal question,
   never with party names, product code names or matter facts
6. record the routing decision (§6) — the decision, not the content
7. the human decides before sensitive material is sent (Stage 1 §7; Stage 9 §6)
```

Permitted and prohibited matter classes per route:

| Route | Permitted | Prohibited |
| --- | --- | --- |
| P | Class 0 | Classes 1–9 |
| R → P or A | Classes 3, 4, 5, 8 where the redacted form carries no identifying or secret content | Classes 1, 6, 7 cannot be downgraded by redaction |
| A | Classes 1–5, 8, 9 (class 6 only after the NDA check) | Class 7; class 6 without the check |
| L | Classes 1–6, 8, 9 | Class 7 |
| N | — | — |

---

## 6. Logs, retention and deletion

Design resolution of the conflict in L8:

| Keep | Do not duplicate |
| --- | --- |
| **An audit record**: who, when, which tool and account type, which sensitivity class, which route, what was redacted (by reference), the human decision, the matter ID | The confidential content itself in a second place |

Rules:

1. Matter artefacts (Stage 6) live in the consuming project and are as sensitive as their contents. Their location is a project decision.
2. **Local agent transcripts are copies** (P12): plaintext, unencrypted, swept by default after 30 days, with history and memory persisting longer. The skill tells the user this exists when class 1, 2, 3, 6, 8 or 9 material is involved, and how to purge it. It never writes matter content into agent memory.
3. Stored prompts and outputs are disclosable documents (L5). For class 9 material this is said **before** the work starts.
4. Deletion by the user does not guarantee deletion by a provider under legal hold (P8).
5. Retention periods are the consuming project's decision. Legal Skills sets none.

---

## 7. Redaction and minimisation

Methods that professionals use (log b Q7): role labels for parties; removal of direct identifiers; abstraction of the legal question; synthetic facts that preserve the legal structure; excerpting only the clause in issue.

Documented limits:

- Re-identification from context, dates, amounts or rare facts.
- Loss of legally material detail (for example a date that decides which version of a provision applied).
- No cure for privilege, NDA or live-secret risk (L10).
- No exit from UK GDPR while the sender can re-identify (L9).

Rule: after redaction, run the materiality test on what was removed (Stage 6 A2). If a removed detail is material, either a stricter route is needed or the conclusion is labelled "insufficient facts".

---

## 8. Public benchmarks and examples

All public fixtures, examples and benchmarks in this repository use **public or synthetic data only**. Synthetic fixtures are labelled synthetic. No supplied book text, no real matter, no real personal data. This restates a bootstrap acceptance gate and binds Stages 16–18.

---

## 9. Provider claims discipline

From Stage 4 N26 and P16: the skill never describes itself or the model as a lawyer or as lawyer-equivalent. Where the provider's usage policy requires professional review of legal outputs and disclosure of AI use to consumers (H-17), consumer-facing deployments of Legal Skills outputs carry that duty to the deploying project. Legal Skills states it; it does not police it.

---

## 10. Failure modes

Thirty failure modes are listed in the supporting logs. The ones that drive the design:

| Failure | Evidence | Smallest repair |
| --- | --- | --- |
| Personal-plan agent used in a work repository (consumer terms apply silently) | P2, P3 | Check account type before classes 1–6, 8, 9; force organisation login |
| "Zero retention" assumed to mean nothing is kept, or assumed available for the model in use | P4, P5 | Read the carve-outs; record the model |
| Private model call combined with a public search or a document upload to a scraper | P11, P13, P14 | Most-exposed-tool rule |
| Search query names the client or the secret | P13 | Abstract the query |
| Founder pastes a solicitor's advice into a consumer tool | L2, L4 | Warn first; route A or L; suggest asking the solicitor |
| Non-lawyer assumes AI analysis of a dispute is privileged | L1, L5 | Say it is disclosable before starting |
| Names replaced, then treated as anonymous | L9 | Treat as personal data still |
| Third-party NDA material sent without reading the NDA | L13 | Class 6 default N or R |
| Credentials in context or transcripts | P12; class 7 | Strip always; purge transcripts |
| Provider property stated as timeless | Log a §4.6 | Dated evidence ID and re-check date |
| Full content logged twice "for the audit trail" | L8 | Audit record without content |
| Local route chosen, telemetry left on | P15 | Check defaults |

---

## 11. Bounded gaps

| # | Gap | Bound |
| --- | --- | --- |
| G1 | SRA Code 6.3–6.5 and SRA guidance not read as raw text (403) | Quotations marked "as reported"; the design does not depend on their exact wording |
| G2 | Whether enterprise terms preserve privilege is undecided (L3) | Stated as inference in every output that touches it; class 1 handling is conservative |
| G3 | UK–US data-bridge status not positively verified (L12) | Transfer mechanism is checked per provider at approval time, not assumed |
| G4 | EU view of pseudonymised data read from a press release only | UK rule applied; EU marked unresolved |
| G5 | Provider trust centres, sub-processor lists and service-specific terms not inspected | The checklist asks the approver to check them |
| G6 | ABA Opinion 512 still secondary only | US consent point marked secondary |
| G7 | Identity of the search backend behind the agent's web search not found | Treated as an external disclosure |
| G8 | Local-model capability limits are heuristic | Stage 11 and Stage 12 assess |
| G9 | Anthropic default API retention documented inconsistently | Assume 30 days |

---

## 12. Exit verification

| Requirement (bootstrap §16) | Where | Met |
| --- | --- | --- |
| Researched: confidentiality, privilege, personal data, commercial secrets, security-sensitive information, provider retention / training, connector access, logs, prompt / output storage, local / private execution, redaction, minimisation, retention / deletion | §2; logs a and b | Yes |
| Per material provider or tool: data sent; storage / retention; training use; access controls; region / transfer; enterprise controls; local option; permitted and prohibited matter classes | Log a §3 (per-provider tables for Anthropic, OpenAI, Google, Microsoft, web tooling, local options, agent-side storage); §5 table | Yes, dated; gaps in §11 |
| The workflow can select public research, redaction, approved private provider, local execution or non-disclosure | §3 classes; §4 routes; §5 procedure | Yes |
| Public benchmarks use public or synthetic data | §8 | Yes |
| **Exit: legal work can be routed without casually exposing confidential or privileged information** | §5 (classification before disclosure; most-exposed-tool rule; abstract queries; human decision; stop condition) | Yes |
