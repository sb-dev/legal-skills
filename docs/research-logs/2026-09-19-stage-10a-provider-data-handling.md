# Stage 10 supporting log a — provider and tool data handling

**Stage:** 10 (supporting record for `2026-09-19-stage-10-confidentiality-privilege-sensitive-data.md`)  
**Retrieved:** 19 September 2026 (each register row carries its own date)  
**Evidence ID prefix:** `H-`

## Reading notes

- Produced by one research agent under a written brief. Most sources were read as raw page or PDF text; the register marks the exceptions.
- Provider terms and professional guidance change often. Every statement here is valid only as of its retrieval date. Nothing here is a timeless property of a provider.
- Legal propositions are design evidence for the named jurisdiction and date. They are not advice and not authority for a live matter. The record separates decided law from inference.
- Dispositions and proposals here are the researcher's. Accepted positions are in the main Stage 10 log.

---

Retrieved-at for every source: **2026-09-19**. Everything below is valid-as-of that date only. Provider terms are contracts and product documentation, not law; they change without notice (see section 4.6). Nothing here is legal advice on whether a given use satisfies SRA, GDPR/UK GDPR or privilege requirements.

**Inspection method.** Every source marked "raw-text" was downloaded with `curl` and read as page text (HTML stripped locally, or the provider's own `.md` rendering). Sources marked "raw-text via reader" were blocked to direct download (HTTP 403) and were retrieved as page text through the `r.jina.ai` text-rendering proxy (a third-party renderer that returns the page text; not a model-written summary). **No model-written fetch summary was used for any figure in this file**: the two WebFetch attempts made both failed with 403 and contributed nothing. Every number is therefore marked **[TV] = text-verified**; there are no "as reported by fetch summary" figures. WebSearch was used for discovery only; search snippets are not cited as evidence. Raw text copies are in `stage10/raw/`.

---

## 1. Scope and questions

Scope: the execution providers and tools an agent running `legal-skills` would materially use — Anthropic (API, Claude Code, claude.ai consumer, Team/Enterprise, Bedrock/Vertex), OpenAI, Google, Microsoft, web tooling (built-in search/fetch, Firecrawl), local open-weight runtimes, and Claude Code's own on-disk storage.

Evidence questions:

- Q1. For each surface: what is sent, how long is it kept, is it trained on by default, who (human or automated) can review it, where is it processed, and what enterprise controls exist?
- Q2. Which account type / contract governs a given session (consumer vs commercial; first-party vs cloud platform), and how does a user tell?
- Q3. Does "zero data retention" actually mean nothing is kept, and for which models/features does it not apply?
- Q4. What leaves the machine when the agent searches or fetches the web?
- Q5. What stays on the local machine after a session, in what form, and how is it deleted?
- Q6. What do providers say about legal advice, confidentiality, or privilege?
- Q7. Which of these terms changed in 2025-2026 (change-sensitivity)?

---

## 2. Evidence register

Type key: PT = provider terms/policy (contract-grade); PD = provider product documentation; PH = provider help-centre article; PM = provider marketing/blog (weak); PR = practitioner commentary (secondary). All retrieved 2026-09-19.

| ID | Title | Type | URL | Page date | Inspected? | What it supports |
|---|---|---|---|---|---|---|
| H-01 | Claude Code — Data usage | PD | https://code.claude.com/docs/en/data-usage | none shown | raw-text | Claude Code training policy by account type, retention, telemetry, /feedback, WebFetch hostname check, provider defaults |
| H-02 | Claude Code — Zero data retention | PD | https://code.claude.com/docs/en/zero-data-retention | none shown | raw-text | ZDR scope, exclusions, disabled features, Covered Models, 2-year flagged retention |
| H-03 | Claude Code — Explore the .claude directory (Application data) | PD | https://code.claude.com/docs/en/claude-directory | none shown | raw-text | Local plaintext transcripts, paths, cleanupPeriodDays, `claude project purge` |
| H-04 | Claude Code — Memory | PD | https://code.claude.com/docs/en/memory | none shown | raw-text | Auto-memory location, machine-local, plain markdown |
| H-05 | Claude Code — Tools reference (WebFetch / WebSearch behaviour) | PD | https://code.claude.com/docs/en/tools-reference | none shown | raw-text | What WebFetch/WebSearch do, where search runs, 15-min cache |
| H-06 | Claude API — API and data retention | PD | https://platform.claude.com/docs/en/manage-claude/api-and-data-retention (requested via /build-with-claude/ path) | none shown | raw-text | ZDR scope and exclusions, feature eligibility table, Covered Models, who is processor on Bedrock/Google |
| H-07 | Covered Models (Claude Help Center) | PH | https://support.claude.com/en/articles/15425695 | "Updated over 2 weeks ago"; designations dated 9 Jun 2026 and 31 Aug 2026 | raw-text | 30-day minimum retention for Fable/Mythos models on every surface; ZDR unavailable; Enterprise Frontier Safeguards |
| H-08 | Privacy Center — How long do you store my organization's data? (commercial) | PH | https://privacy.claude.com/en/articles/7996866-how-long-do-you-store-my-organization-s-data | 1 Jul 2026 | raw-text | 30-day API deletion, exceptions, 2y/7y flagged retention, 5y feedback |
| H-09 | Privacy Center — How long do you store my data? (consumer) | PH | https://privacy.claude.com/en/articles/10023548-how-long-do-you-store-my-data | 1 Jul 2026 | raw-text | Consumer deletion within 30 days, 5-year de-identified training retention |
| H-10 | Privacy Center — Is my data used for model training? (commercial) | PH | https://privacy.claude.com/en/articles/7996868-is-my-data-used-for-model-training | 18 Aug 2026 | raw-text | Commercial no-training default; feedback exception |
| H-11 | Privacy Center — Is my data used for model training? (consumer) | PH | https://privacy.claude.com/en/articles/10023580-is-my-data-used-for-model-training | 16 Mar 2026 | raw-text | Consumer training conditions; safety-flag exception; connectors excluded; Incognito |
| H-12 | Anthropic Commercial Terms of Service | PT | https://www.anthropic.com/legal/commercial-terms | Effective 17 Jun 2025 | raw-text | "may not train models on Customer Content"; confidentiality clause E; DPA incorporated; 30-day update clause |
| H-13 | Anthropic Consumer Terms of Service (UK variant served) | PT | https://www.anthropic.com/legal/consumer-terms | Effective 8 Oct 2025 | raw-text | Training "unless you opt out"; consumer definition; "Non-commercial use only"; do not rely without verifying |
| H-14 | Anthropic Privacy Policy | PT | https://www.anthropic.com/legal/privacy | Effective 10 Sep 2026 | raw-text | Training opt-out and exceptions; transfers to US; SCCs/adequacy; flagged content handling |
| H-15 | Anthropic Data Processing Addendum | PT | https://www.anthropic.com/legal/data-processing-addendum | Effective 24 Feb 2025 | raw-text | Controller/processor roles, SCCs + UK Addendum, subprocessors, 48-hour breach notice, audit, deletion |
| H-16 | Anthropic news — Updates to Consumer Terms and Privacy Policy | PM (first-party announcement) | https://www.anthropic.com/news/updates-to-our-consumer-terms | 28 Aug 2025 | raw-text | The 2025 consumer change: training choice, 5-year retention, 8 Oct 2025 deadline, commercial/Bedrock/Vertex excluded |
| H-17 | Anthropic Usage Policy | PT | https://www.anthropic.com/legal/aup | Effective 15 Sep 2025 | raw-text | "Legal" is a High-Risk Use Case: qualified-professional review + AI disclosure |
| H-18 | Claude API — Data residency | PD | https://platform.claude.com/docs/en/build-with-claude/data-residency (redirects to manage-claude) | none shown | raw-text | inference_geo values "global"/"us"; workspace geo "us" only; 1.1x price |
| H-19 | Claude API — Web search tool | PD | https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-search-tool | none shown | raw-text | Server-side search; query visible in response; user_location; encrypted_content |
| H-20 | Privacy Center — Custom data retention controls for Enterprise | PH | https://privacy.claude.com/en/articles/10440198-custom-data-retention-controls-for-claude-enterprise | "Updated this week" | raw-text | Enterprise default = retained indefinitely; minimum custom period 30 days |
| H-21 | Claude Enterprise plan page | PM (weak) | https://claude.com/pricing/enterprise | none shown | raw-text | Lists SSO/SAML, SCIM, audit logs, Compliance API, RBAC, retention controls (Enterprise only) |
| H-22 | Amazon Bedrock — Abuse detection | PD | https://docs.aws.amazon.com/bedrock/latest/userguide/abuse-detection.html | none shown | raw-text | Bedrock ZDR/ZOA default; 30-day retention of all Claude Fable 5/5.1 traffic; AWS human review; not shared with model providers |
| H-23 | Amazon Bedrock FAQs | PM/PD | https://aws.amazon.com/bedrock/faqs/ | none shown | raw-text | Inputs/outputs not shared with model providers; not used to train |
| H-24 | Amazon Bedrock — Data protection | PD | https://docs.aws.amazon.com/bedrock/latest/userguide/data-protection.html | none shown | raw-text | Shared responsibility model; CloudTrail; TLS 1.2 (little provider-specific content) |
| H-25 | Google Cloud — Gemini Enterprise Agent Platform (formerly Vertex AI) and zero data retention | PD | https://cloud.google.com/vertex-ai/generative-ai/docs/data-governance | Last updated 2026-09-16 UTC | raw-text | Training restriction; abuse-monitoring prompt logging; 24h in-memory cache; Search grounding 3 days; Maps grounding 30 days; Interactions API store=true default |
| H-26 | OpenAI API — Data controls in the OpenAI platform ("Your data") | PD | https://platform.openai.com/docs/guides/your-data (redirects to developers.openai.com) | none shown | raw-text | No training since 1 Mar 2023; 30-day abuse logs; ZDR / Modified Abuse Monitoring by approval; per-endpoint table; data residency |
| H-27 | OpenAI — Enterprise privacy | PT/PM | https://openai.com/enterprise-privacy/ | Updated 8 Jan 2026 | raw-text via reader (direct = 403) | Business no-training default; admin retention; 30-day deletion; who at OpenAI can access; SSO, Compliance API, DPA, BAA |
| H-28 | OpenAI — How we're responding to The New York Times' data demands | PM (first-party statement) | https://openai.com/index/response-to-nyt-data-demands/ | Update dated 22 Oct 2025 | raw-text via reader (direct = 403) | Preservation order scope, end date 26 Sep 2025, residual Apr–Sep 2025 data, who was excluded |
| H-29 | OpenAI Help — Chat and file retention in ChatGPT | PH | https://help.openai.com/en/articles/8983778-chat-and-file-retention-policies-in-chatgpt | "Updated: 23 hours ago" | raw-text via reader | 30-day deletion; temporary chat copy up to 30 days; Library files survive chat deletion |
| H-30 | OpenAI Help — How your data is used to improve model performance | PH | https://help.openai.com/en/articles/5722486-how-your-data-is-used-to-improve-model-performance | "Updated: 3 days ago" | raw-text via reader | Consumer opt-out toggle; business no-training default |
| H-31 | OpenAI — Consumer privacy page | PM | https://openai.com/consumer-privacy/ | none shown | raw-text via reader | Temporary chats; training toggle; memory; ad controls exist on consumer product |
| H-32 | OpenAI Usage Policies | PT | https://openai.com/policies/usage-policies/ | Effective 29 Oct 2025 | raw-text via reader | No tailored legal advice "without appropriate involvement by a licensed professional"; rules "no substitute for ... professional duties" |
| H-33 | OpenAI Privacy Policy (rest of world) | PT | https://openai.com/policies/row-privacy-policy/ | Updated 6 Feb 2026 | raw-text | Consumer content may train models unless opted out; temporary chats 30 days; legal-retention carve-out |
| H-34 | OpenAI Services Agreement | PT | https://openai.com/policies/services-agreement/ | Effective 1 Jan 2026 | raw-text via reader | s4.2 no use of Customer Content to develop/improve; s7 confidentiality; update mechanism |
| H-35 | Jones Walker — OpenAI Loses Privacy Gambit: 20 Million ChatGPT Logs | PR | https://www.joneswalker.com/en/insights/blogs/ai-law-blog/openai-loses-privacy-gambit-20-million-chatgpt-logs-likely-headed-to-copyright-p.html | 6 Jan 2026 | raw-text | 5 Jan 2026 Stein J affirms order to produce 20m de-identified logs; "voluntarily submitted" reasoning |
| H-36 | Gemini API Additional Terms of Service | PT | https://ai.google.dev/gemini-api/terms | Effective 23 Mar 2026 | raw-text via reader (direct = empty 302) | Unpaid vs Paid Services; human review; UK/EEA/CH rule; Search grounding 30 days; "don't rely ... legal" |
| H-37 | Gemini API — Abuse monitoring / usage policies | PD | https://ai.google.dev/gemini-api/docs/usage-policies | none shown | raw-text via reader | 55-day retention of prompts, context, output; human review of flagged content |
| H-38 | Google Workspace — Generative AI privacy hub | PH | https://support.google.com/a/answer/15706919 | change log to 26 May 2026 | raw-text via reader | No training / no human review outside domain without permission; CDPA; admin retention (3/18/36 months or indefinite); feedback 18 months |
| H-39 | Microsoft — Data, privacy and security for Foundry Models sold by Azure (incl. Azure OpenAI) | PD | https://learn.microsoft.com/en-us/azure/ai-foundry/responsible-ai/openai/data-privacy | ms.date 2026-05-18; change log 3 Oct 2025 | raw-text | Not available to OpenAI; not used for training; geography; Global/DataZone; abuse-monitoring store; EEA reviewers |
| H-40 | Microsoft — Abuse monitoring (Foundry / Azure OpenAI) | PD | https://learn.microsoft.com/en-us/azure/ai-foundry/openai/concepts/abuse-monitoring | ms.date 2026-05-13 | raw-text | Automated (LLM) review default, human review on flagged samples, modified abuse monitoring by application |
| H-41 | Microsoft — Data, Privacy, and Security for Microsoft 365 Copilot | PD | https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy | ms.date 2026-07-09 | raw-text | No training on prompts/Graph data; Copilot opted out of abuse monitoring; EU Data Boundary; Anthropic subprocessor excluded from EUDB; Purview retention |
| H-42 | Microsoft — Data, privacy, and security for web search in Copilot | PD | https://learn.microsoft.com/en-us/copilot/microsoft-365/manage-public-web-access | ms.date 2026-08-18 | raw-text | Generated Bing queries; identifiers removed; example of a manager's name being sent; query logging/citations |
| H-43 | Firecrawl Privacy Policy | PT | https://www.firecrawl.dev/privacy-policy | Last revision 26 Dec 2024 | raw-text | Account PII only; retained until deletion requested; US transfer; silent on scraped/uploaded content |
| H-44 | Firecrawl Terms of Service | PT | https://www.firecrawl.dev/terms-of-service | Last revision 5 Nov 2024 | raw-text | No retention, training or customer-content confidentiality terms found |
| H-45 | Firecrawl docs — Enterprise | PD | https://docs.firecrawl.dev/enterprise | none shown | raw-text | ZDR (Enterprise, in-memory), SOC 2 Type II, DPA, SSO |
| H-46 | Firecrawl docs — Scrape (caching, ZDR) | PD | https://docs.firecrawl.dev/features/scrape | none shown | raw-text | Default cache maxAge 2 days; storeInCache:false; zeroDataRetention flag; screenshots need persistent storage |
| H-47 | Firecrawl docs — Parse (file upload) | PD | https://docs.firecrawl.dev/features/parse | none shown | raw-text | Local files are uploaded to Firecrawl; ZDR "support"; no non-ZDR retention period stated |
| H-48 | Ollama Privacy Policy | PT | https://ollama.com/privacy | Last updated March 2026 | raw-text | Local prompts not collected; cloud models processed transiently; limited metadata |
| H-49 | Ollama FAQ (repository docs) | PD | https://raw.githubusercontent.com/ollama/ollama/main/docs/faq.mdx | none shown | raw-text | Local-only mode: `disable_ollama_cloud` / `OLLAMA_NO_CLOUD=1` |
| H-50 | vLLM — Usage stats collection | PD | https://docs.vllm.ai/en/latest/usage/usage_stats.html | none shown | raw-text | Anonymous usage stats ON by default; opt-out variables |
| H-51 | llama.cpp README | PD | https://raw.githubusercontent.com/ggml-org/llama.cpp/master/README.md | none shown | raw-text | No telemetry statement found either way |
| H-52 | Debevoise Data Blog — SDNY rules AI-generated documents not protected by privilege (US v. Heppner) | PR | https://www.debevoisedatablog.com/2026/02/11/district-court-rules-ai-generated-documents-are-not-protected-by-privilege/ | 11 Feb 2026 | raw-text | US court: consumer Claude exchanges not privileged; DOJ relied on Anthropic privacy policy (training, third-party disclosure) |

Inspected sources: **52** (all raw page text; 0 model-summarised). Independence note: H-01/H-02/H-06/H-07/H-08 are all Anthropic first-party and partly restate one underlying policy; H-22 (AWS) is an independent first-party confirmation of the Covered Models rule. H-35 and H-52 are single practitioner notes on court rulings; the rulings themselves were **not** inspected.

---

## 3. Per-provider findings

"nf" = not found on the inspected pages. All figures [TV] (text-verified).

### 3.1 Anthropic

| Field | Claude API (commercial) | Claude Code | claude.ai Free / Pro / Max (consumer) | Team / Enterprise (Claude for Work) | Claude via Bedrock / Google Cloud |
|---|---|---|---|---|---|
| Governing terms | Commercial Terms + DPA (H-12, H-15) | Follows the signed-in account: consumer account = Consumer Terms; API key / Team / Enterprise = Commercial Terms (H-01) | Consumer Terms + Privacy Policy (H-13, H-14). UK text: consumer = acting "wholly or mainly outside your trade, business, craft or profession"; "Non-commercial use only" (H-13) | Commercial Terms + DPA (H-10, H-12) | The cloud provider "is the data processor"; Anthropic's ZDR/HIPAA arrangements do not apply; use that platform's terms (H-06). 2025 consumer change does not apply (H-16) |
| Data sent | Prompts, files, tool definitions/results, outputs | "all user prompts and model outputs", i.e. including file contents and command output that enter context; TLS 1.2+ (H-01). Separate: metrics, error reports, WebFetch hostname check, optional /feedback transcript (H-01) | Chats, files, coding sessions | Chats, projects, files, Claude Code sessions | Same payload, sent to AWS / Google endpoint |
| Retention | Inputs/outputs deleted "within 30 days" [TV] except longer-lived features (Files API until deleted; batch 29 days [TV]; code-execution containers up to 30 days [TV]), contract, Usage Policy enforcement, law (H-06, H-08). H-06 also says conversation content "is not retained by default" except Covered Models — inconsistent with H-08/H-01; see 7 | Commercial: "Standard: 30-day" [TV]; consumer with training on: 5 years [TV]; consumer with training off: 30 days [TV] (H-01). /feedback, /bug, /share transcripts: 5 years [TV]; survey-shared transcripts up to 6 months [TV] (H-01) | Deleted chats removed from back end within 30 days [TV]; if training allowed, de-identified data up to 5 years [TV] in training pipelines (H-09, H-16) | Retained in product; **Enterprise default = indefinitely** unless admin sets a period; minimum custom period 30 days [TV]; projects override chat retention (H-20). Deleted items gone from back end within 30 days [TV] (H-08). Compliance API local-session transcripts 6 years default [TV] (H-06) | Bedrock default: no storage of inputs/outputs; **but all Claude Fable 5 / 5.1 traffic retained up to 30 days** [TV], stored by AWS (H-22). Google: see 3.3; partner-model specifics nf |
| Flagged content | Up to 2 years inputs/outputs, 7 years classifier scores [TV], even under ZDR (H-06, H-08) | Same; "Even with ZDR enabled" up to 2 years [TV] (H-02) | Same 2y / 7y [TV] (H-09) | Same (H-08) | AWS: classifier-flagged Fable traffic "subject to potential human review performed by AWS" (H-22) |
| Training default | Off. "Anthropic may not train models on Customer Content from Services" (H-12). Exceptions: explicit feedback, opt-in programmes (H-10) | Follows account type (H-01) | **On unless the user opts out**: "unless you opt out of training through your account settings" (H-13). Even if opted out: feedback and safety-flagged material may be used (H-13, H-14). Incognito chats excluded; raw connector/MCP content excluded unless copied into chat (H-11) | Off by default (H-10); owners can disable thumbs feedback (H-10) | AWS: not used to train and not shared with model providers (H-22, H-23). Google: no training without permission (H-25) |
| Human review / abuse monitoring | Automated trust-and-safety classifiers; flagged material retained and may be re-identified for enforcement (H-14). Covered Models: "Automated review by default" (H-07). Who at Anthropic may view: nf on inspected pages | Same as the account | Same; flagged conversations may train safeguards models (H-11) | Same | AWS reviewers, not Anthropic (H-22) |
| Access controls | Workspaces, API keys; Trust Centre artefacts (not inspected) | Managed settings `forceLoginMethod` / `forceLoginOrgUUID` to stop personal-account sign-in (H-02) | Individual account; if a work-email account is linked to an enterprise org, admins may access Materials (H-13) | SSO/SAML, SCIM, RBAC, audit logs, Compliance API (H-21, weak) | IAM / CloudTrail (H-24); GCP IAM |
| Region / transfers | `inference_geo`: "global" (default) or "us" only; workspace geo "us" only [TV]; US-only priced 1.1x [TV] (H-18). **No EU or UK inference/storage option found.** Transfers: US servers; SCCs + UK Addendum (H-14, H-15) | Same as API/account | US and other countries; adequacy/SCCs/derogations (H-14) | Same as commercial | Region chosen in the cloud console; with Bedrock cross-region inference retained data sits in the destination region (H-22) |
| Enterprise controls | ZDR by sales approval, per organisation; HIPAA/BAA; DPA auto-incorporated; 48-hour breach notice [TV]; audit right (H-06, H-15) | ZDR only for "qualified accounts" on Claude for Enterprise or commercial API keys; not in the standard Enterprise plan; disables cloud sessions, Remote Control, Artifacts, /feedback (H-02) | None; ZDR expressly excludes Free/Pro/Max including Claude Code on those plans (H-06) | Team/Enterprise chat interfaces are **not** ZDR-eligible; only Claude Code inference is (H-02, H-06) | Cloud-platform controls; Enterprise Frontier Safeguards gives ZDR for Fable on Bedrock only to 31 Dec 2026 [TV] for eligible customers (H-22) |
| Covered Models | Claude Fable 5 / 5.1 and Mythos 5 / 5.1 require 30-day minimum retention [TV] "on every platform"; ZDR unavailable unless expressly authorised; transitional ZDR for eligible customers; EFS from "fall 2026" (H-06, H-07) | `best` alias falls back to Opus where Fable is unavailable (H-02) | n/a | Same | Confirmed independently by AWS (H-22) |
| Local / offline | None (hosted inference) | Client is local, inference is not | None | None | None |
| Confidentiality / privilege / legal advice | "Customer Content is Customer's Confidential Information"; need-to-know, reasonable care, destruction on request, compelled-disclosure notice (H-12 s.E). Usage Policy: Legal is High-Risk — "a qualified professional in that field must review" and AI use must be disclosed to consumers (H-17). Privilege: nf | — | No confidentiality undertaking comparable to s.E found; "You should not rely on any Outputs ... without independently confirming" (H-13). Privilege: nf in provider text; see H-52 | As API | Provider's own terms |

### 3.2 OpenAI

| Field | API platform | ChatGPT Free / Plus / Pro | ChatGPT Business (ex-Team) / Enterprise / Edu |
|---|---|---|---|
| Training default | Off since 1 Mar 2023 [TV] unless opted in (H-26); contract: s4.2 (H-34) | On unless "Improve the model for everyone" is turned off or privacy-portal request made; Temporary Chat never trains (H-30, H-31, H-33) | Off by default (H-27, H-30) |
| Retention | Abuse-monitoring logs up to 30 days [TV] "unless longer retention is required by law"; application state per endpoint (Responses API 30 days by default [TV]; files, vector stores, threads, batches "until deleted") (H-26) | Saved until deleted; deleted chats purged within 30 days [TV] unless already de-identified or legal/security hold; Temporary Chat copy up to 30 days [TV]; Library files survive chat deletion (H-29) | Enterprise/Edu: admin-set; Business: admin-controllable; deleted removed within 30 days [TV] (H-27) |
| ZDR | Zero Data Retention or Modified Abuse Monitoring, "subject to prior approval"; many endpoints ineligible; OpenAI reserves right to make models ineligible; CSAM-flagged images retained regardless (H-26) | None | Not offered as ZDR; admin retention only (H-27) |
| Human review | Authorised employees (support, abuse, legal) and "specialized third-party contractors ... solely to review for abuse and misuse" (H-27) | nf in detail | Enterprise: employees only for incidents, recovery with permission, or law; Business: employees plus contractors for abuse review (H-27) |
| Region | Data residency per project, by sales eligibility; non-US regions require abuse-monitoring controls and a Modified Retention amendment; 10% uplift [TV] for models released on/after 5 Mar 2026; system data excluded (H-26) | nf | nf in inspected text (residency offered; regions not verified) |
| Enterprise controls | DPA, BAA, SOC 2 Type 2 (H-27) | none | SAML SSO, Compliance API audit log of conversations, DPA (H-27) |
| Court-ordered retention | NYT litigation: order to keep consumer ChatGPT and API content indefinitely affected Free/Plus/Pro/Team and non-ZDR API; **not** Enterprise, Edu or ZDR API. OpenAI states obligations "ended on September 26, 2025" [TV]; it still holds "limited historical April–September 2025 user data" under legal hold; EEA/CH/UK-origin conversations stated as no longer required to be retained (H-28). Separately, on 5 Jan 2026 the district judge affirmed an order to produce 20 million [TV] de-identified ChatGPT logs to plaintiffs under protective order (H-35, secondary; ruling not inspected). Status after Jan 2026: not verified | | |
| Legal advice / secrecy | Usage Policies bar "tailored advice that requires a license, such as legal ... without appropriate involvement by a licensed professional"; rules are "no substitute for ... professional duties" (H-32). Services Agreement s7 mutual confidentiality (H-34). Privilege: nf | | |

### 3.3 Google

| Field | Gemini API / AI Studio — unpaid | Gemini API — paid | Vertex AI (now "Gemini Enterprise Agent Platform") | Gemini for Workspace |
|---|---|---|---|---|
| Training | Content used to "provide, improve, and develop Google products"; "**Do not submit sensitive, confidential, or personal information**" (H-36) | Not used to improve products; processed under the processor DPA (H-36) | No training or fine-tuning without permission (H-25) | No training or human review "outside your domain without permission" (H-38) |
| UK / EEA / CH rule | Paid-service data terms "apply to all Services", including free AI Studio and unpaid quota, for users in EEA/CH/UK (H-36). Practical caution: depends on Google's determination of location; not tested | — | — | — |
| Retention | nf for unpaid | Logged "for a limited period"; abuse-monitoring page: 55 days [TV] for prompts, context, output (H-37). Grounding with Google Search: 30 days [TV] (H-36) | In-memory cache 24h TTL [TV] (can be disabled); Search grounding logs up to 3 days [TV], cannot be disabled; Maps grounding 30 days [TV]; Interactions API `store` defaults to true; abuse prompt logging unless exception granted (H-25) | Admin-set auto-delete (3 / 18 / 36 months [TV]) or indefinite; feedback up to 18 months [TV] (H-38) |
| Human review | "human reviewers may read, annotate, and process your API input and output" (H-36) | Authorised Google employees on flagged content (H-37) | Per abuse-monitoring terms; exception available (H-25) | None without permission (H-38) |
| Region | nf | "may be stored transiently or cached in any country" (H-36) | Cache "adheres to all Data Residency requirements for the selected location" (H-25) | nf in inspected text |
| Enterprise controls | none | Cloud billing; DPA | CDPA, CMEK, IAM, ZDR by configuration plus approved exception (H-25) | CDPA, DLP/IRM labels restrict Gemini access, admin retention (H-38) |
| Legal advice | "Don't rely on the Services for medical, mental health, legal, financial, or other professional advice" (H-36) | same | nf | nf |

### 3.4 Microsoft

| Field | Azure OpenAI / Foundry "models sold by Azure" | Microsoft 365 Copilot |
|---|---|---|
| Training | Prompts/completions "NOT used to train any generative AI foundation models"; "NOT available to OpenAI" (H-39) | Prompts, responses and Graph data not used to train foundation LLMs (H-41) |
| Abuse monitoring | Automated (incl. LLM) review by default; flagged samples may be stored for human review by authorised Microsoft employees (SAW + JIT); EEA deployments reviewed by EEA staff; "modified abuse monitoring" by application under Limited Access (H-39, H-40). **Retention period of the abuse-monitoring store: not found** on either current page (the string "30" does not occur in H-40) | "Microsoft Copilot services have opted out of it" (H-41) |
| Retention | Stateful features (Responses API, threads, stored completions, files) stored in the customer's tenant until deleted (H-39) | Interaction history stored with other Microsoft 365 content; retention via Purview policies; eDiscovery (H-41) |
| Region | Customer-specified geography, except "Global" (any geography) and "DataZone" deployments (H-39) | EU Data Boundary for EU users; "Models provided by Anthropic as a subprocessor are currently excluded from the EU Data Boundary" (H-41). UK-specific commitment: nf |
| Web search | — | Generated Bing queries, tenant/user identifiers removed, not used to improve Bing; queries can still carry names or themes derived from internal documents; admin query logging available (H-42) |
| Enterprise controls | Product Terms + DPA, CMK, Entra ID | DPA, Product Terms, Purview audit/retention, admin toggles (H-41, H-42) |
| Privilege / legal advice | nf | nf |

### 3.5 Web tooling used by an agent

| Tool | What leaves the machine | Retention / other | Evidence |
|---|---|---|---|
| Claude Code `WebSearch` | The model-written query goes to Anthropic's web-search backend; up to eight backend searches per call [TV]; backend "not configurable". The downstream search provider is not named | API web search is ZDR-eligible except dynamic filtering; otherwise standard account retention | H-05, H-06, H-19 |
| Claude Code `WebFetch` | (1) hostname only to `api.anthropic.com` for a blocklist check, on every provider, not disabled by `CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC`; (2) the full URL (path and query string) goes to the target site with a `Claude-User` user-agent; (3) page content is passed to a small model for summarising | 15-minute local cache [TV]; result is lossy ("Claude receives that model's answer, not the raw page") | H-01, H-05 |
| API `web_fetch` | URL to publisher: "Website publishers may retain request data (such as fetched URLs and request metadata)" | ZDR-eligible except dynamic filtering; not HIPAA-eligible | H-06 |
| Firecrawl (scrape/search) | URL or query to Firecrawl, then to the target / upstream search provider | Results cached and served to later requests; default freshness window 2 days [TV]; `storeInCache:false` avoids storing; ZDR only on Enterprise plans by enablement, +1 credit/page [TV]; screenshots incompatible with ZDR | H-45, H-46 |
| Firecrawl `/parse` (local document upload) | The whole file is uploaded to Firecrawl | Retention period for non-ZDR uploads: **not found**. Privacy policy (2024) covers account PII only and is silent on customer content; ToS has no training or confidentiality undertaking for content | H-43, H-44, H-47 |
| M365 Copilot web search | Short generated query to Bing | Identifiers stripped; documented example sends a named individual | H-42 |

General point (inference from the above, not a provider statement): a search query or fetched URL is itself a disclosure. A query such as "[client name] insolvency petition [date]" reveals the client, the matter type and the timing to the search backend, to the agent provider's logs, and (for a fetch) to the target site's server logs — none of which are covered by the model provider's no-training or ZDR commitments (H-06: third-party integrations "not covered"). Microsoft's own documentation illustrates the mechanism: a prompt about a user's manager produces a Bing query containing the manager's name (H-42).

### 3.6 Local / offline execution (headline)

| Runtime | What stays local | Telemetry default | Evidence |
|---|---|---|---|
| Ollama | Local prompts and responses: "We do not collect, store, transmit, or have access". Cloud-hosted models and Ollama web search do send prompts (processed "transiently", not trained on). Local-only mode: `disable_ollama_cloud` / `OLLAMA_NO_CLOUD=1` | "limited device and usage metadata (such as app version and request counts)", no content | H-48, H-49 |
| vLLM | Inference local | **Anonymous usage stats collected by default** (hardware / model configuration); opt out with `VLLM_NO_USAGE_STATS=1`, `DO_NOT_TRACK=1`, or `~/.config/vllm/do_not_track` | H-50 |
| llama.cpp | Inference local | No telemetry statement found in README, either way | H-51 |

Practical limits (partly inference, flagged as such): no provider page compares capability, so this is a **practical heuristic, not a sourced finding** — open-weight models that fit on practitioner hardware are materially weaker than frontier hosted models on long-document legal reasoning; a local model has no web research unless a web tool is added, which reintroduces section 3.5 disclosure; a local runtime gives no DPA, no audit logs and no vendor breach duty, so security rests entirely on the machine. Note also that pointing Claude Code at a local model does not by itself stop the WebFetch hostname check to `api.anthropic.com` (H-01) unless `skipWebFetchPreflight` is set.

### 3.7 Agent-side storage: Claude Code on the local machine

| Item | Location | Default life | Evidence |
|---|---|---|---|
| Full transcript: "every message, tool call, and tool result" | `~/.claude/projects/<project>/<session>.jsonl` | Deleted after `cleanupPeriodDays`, default 30 days [TV], minimum 1 | H-03 |
| Large tool outputs | `projects/<project>/<session>/tool-results/` | same sweep | H-03 |
| Subagent transcripts | `projects/<project>/<session>/subagents/` | removed with parent | H-03 |
| Pre-edit file snapshots | `~/.claude/file-history/` | same sweep; 100 most recent checkpoints [TV] | H-03 |
| Large pastes | `~/.claude/paste-cache/` | same sweep | H-03 |
| **Prompt history** — "Every prompt you've typed, with timestamp and project path" | `~/.claude/history.jsonl` | **Kept until you delete it**; not swept | H-03 |
| **Auto memory** (plain markdown, on by default) | `~/.claude/projects/<project>/memory/` | **Not swept**; machine-local; user-editable | H-03, H-04 |
| Desktop / Cowork transcripts | same tree | Exempt from the age limit by default unless `desktopSessionCleanupPeriodDays` or managed `cleanupPeriodDays` is set | H-01, H-03 |
| Feedback bundles | `~/.claude/feedback-bundles/` | local until forwarded | H-01 |

Stated by the provider: "These files are plaintext. Anything that passes through a tool is written to a transcript on disk: file contents, command output, pasted text." and "Transcripts and history are not encrypted at rest. OS file permissions are the only protection." (H-03). Controls: lower `cleanupPeriodDays`; `CLAUDE_CODE_SKIP_PROMPT_HISTORY`; `--no-session-persistence` with `-p`; permission deny rules for sensitive paths; `claude project purge [path|--all]` deletes transcripts, tasks, file-history and matching `history.jsonl` lines for a project (H-03). If the sweep cannot determine the retention period (for example a broken settings file) it **pauses** (H-03).

Meaning for matter material: every client document the agent reads is copied verbatim into an unencrypted local transcript that persists for 30 days by default; prompts and memory persist indefinitely; backups and sync tools will replicate `~/.claude`. Matter closure or a deletion request therefore requires a local purge step in addition to any provider-side deletion. For Enterprise organisations the Compliance API can additionally hold local-session transcripts server-side for 6 years by default [TV] (H-06).

### 3.8 Additional items requested

**(a) Consumer vs commercial differences that matter to a solicitor or founder**

1. Training: consumer Claude and consumer ChatGPT train on content unless the user opts out; commercial/API/business tiers do not by default (H-13, H-12, H-30, H-27). Opting out on Claude consumer still leaves feedback and safety-flagged content usable (H-13).
2. Retention: consumer Claude with training allowed = up to 5 years; commercial API = 30 days (H-09, H-08).
3. Contractual confidentiality and a DPA exist only on commercial terms (H-12 s.E, H-15; H-34 s7). Consumer terms contain no equivalent undertaking (H-13).
4. Permitted use: the UK consumer terms say "You agree not to use our Services for any commercial or business purposes" and define a consumer as acting outside their profession (H-13). A solicitor or founder using a Pro/Max account for client or company work is, on the face of those terms, outside the intended use — and Claude Code inherits the account type (H-01).
5. ZDR, SSO, audit logs, admin retention and the NYT-order exclusion (Enterprise/Edu/ZDR API only) are all commercial-only (H-06, H-27, H-28).
6. Privilege risk: a US court treated consumer-Claude exchanges as not confidential, with the prosecution pointing to the privacy policy's training and disclosure terms (H-52; secondary source; US law, not England and Wales; ruling not inspected). Whether English legal professional privilege would be analysed the same way: not researched here.
7. A paid consumer subscription is still consumer: Pro/Max are excluded from ZDR even when used through Claude Code (H-06).

**(b) What providers say about legal advice or professional secrecy**

- Anthropic Usage Policy: legal interpretation/guidance is a High-Risk Use Case needing qualified-professional review before dissemination and AI disclosure to consumers (H-17).
- OpenAI Usage Policies: no tailored legal advice without a licensed professional; rules are no substitute for professional duties (H-32).
- Google Gemini API terms: do not rely on the service for legal advice (H-36); do not submit confidential information to unpaid services (H-36).
- Microsoft: abuse-monitoring page acknowledges customers who "don't have the right to permit Microsoft to store and conduct human review" of prompts and offers modified abuse monitoring (H-40) — the closest any provider comes to addressing professional secrecy.
- No inspected provider page mentions legal professional privilege, solicitor confidentiality, or the SRA. **Not found** for all four providers.

**(c) Change-sensitivity — terms that changed in 2025-2026**

| Date | Change | Evidence |
|---|---|---|
| 24 Feb 2025 | Anthropic DPA current version | H-15 |
| 17 Jun 2025 | Anthropic Commercial Terms current version | H-12 |
| May–Sep 2025 | OpenAI under court order to preserve consumer and non-ZDR API output indefinitely; ended 26 Sep 2025; residual Apr–Sep 2025 data still held | H-28 |
| 28 Aug / 8 Oct 2025 | Anthropic consumer terms: training-by-default with opt-out; 5-year retention | H-13, H-16 |
| 15 Sep 2025 | Anthropic Usage Policy version | H-17 |
| 3 Oct 2025 | Microsoft data-privacy page re-scoped to all "models sold by Azure"; abuse-monitoring text revised | H-39 |
| 29 Oct 2025 | OpenAI unified Usage Policies | H-32 |
| 1 Jan 2026 | OpenAI Services Agreement version | H-34 |
| 5 Jan 2026 | Order to produce 20m de-identified ChatGPT logs affirmed | H-35 |
| 8 Jan 2026 / 6 Feb 2026 | OpenAI enterprise-privacy page and privacy policy updated | H-27, H-33 |
| 10–17 Feb 2026 | US v. Heppner privilege ruling | H-52 |
| 5 Mar 2026 | OpenAI data-residency 10% uplift threshold date | H-26 |
| 23 Mar 2026 | Gemini API Additional Terms version | H-36 |
| 9 Jun and 31 Aug 2026 | Anthropic Covered Models designations: Fable/Mythos 5 then 5.1 — 30-day mandatory retention, ZDR withdrawn for those models on all platforms | H-07, H-22 |
| 10 Sep 2026 | Anthropic Privacy Policy new effective date (nine days before retrieval; diff against previous version not performed) | H-14 |
| "fall 2026" / 31 Dec 2026 | Enterprise Frontier Safeguards phased roll-out; Bedrock transitional ZDR for Fable ends | H-07, H-22 |
| Undated | Vertex AI documentation now titled "Gemini Enterprise Agent Platform"; OpenAI's current pages say "ChatGPT Business" where the 2025 NYT page said "ChatGPT Team" (rename inferred, not verified) | H-25, H-27 |

---

## 4. Cross-cutting findings — what a routing decision can and cannot rely on

4.1 **Can rely on (contract-grade, all four providers' commercial tiers):** no training on customer content by default (H-12, H-34, H-25, H-39); a DPA with SCCs/UK Addendum (H-15); deletion of API content on roughly a 30-day horizon absent a flag or legal hold (H-08, H-26). Standing: supported finding, valid as of 2026-09-19.

4.2 **Cannot rely on:** (i) "zero data retention" meaning nothing is kept — every provider carves out flagged content, legal holds, and named features; Anthropic keeps flagged inputs/outputs up to 2 years even under ZDR (H-02, H-06); (ii) ZDR being available for the best model — Anthropic's current frontier models (Fable 5/5.1) mandate 30-day retention on every platform, confirmed by AWS (H-07, H-22); (iii) the account being commercial — Claude Code silently inherits whichever account is signed in (H-01, H-02); (iv) EU/UK residency on Anthropic first-party (only "global" or "us") (H-18); (v) provider deletion promises surviving litigation — the NYT order overrode OpenAI's 30-day deletion for roughly five months and residual data is still held (H-28).

4.3 **Provider retention is only one of at least four copies.** A single agent turn can leave: provider-side logs; a local plaintext transcript (H-03); search/fetch traces at the search backend and target site (H-05, H-06); and third-party tool copies (Firecrawl cache, MCP servers) that sit outside every model-provider commitment (H-06, H-26, H-46).

4.4 **The route is determined by the most exposed tool in the turn, not by the model provider.** A ZDR model call combined with a Firecrawl `/parse` upload or a client-named web search is not a private route.

4.5 **The consumer/commercial line is the single most consequential switch** for training, retention, confidentiality undertakings, permitted business use and (in one US ruling) privilege (3.8(a)).

4.6 **These facts decay quickly.** Twelve-plus material changes in 18 months (3.8(c)), one of them nine days old. A routing rule must cite a dated evidence ID and carry a re-verification interval; it must never state a provider property as timeless.

4.7 **Provider terms do not answer the professional question.** No provider addresses privilege or solicitor confidentiality (3.8(b)); both Anthropic and OpenAI put the professional-review duty on the user. Whether a given route satisfies SRA confidentiality duties, UK GDPR or privilege is a separate legal analysis that this record does not perform.

---

## 5. Failure modes and smallest repair

| # | Failure mode | Evidence | How detected | Smallest repair |
|---|---|---|---|---|
| F1 | User runs Claude Code on a personal Pro/Max login believing commercial terms apply; content is trainable, retained up to 5 years, excluded from ZDR, and outside permitted "non-commercial" use | H-01, H-06, H-13 | `/status` or account check at session start | Routing skill asks/records account type before any confidential material enters context; organisations set `forceLoginOrgUUID` |
| F2 | "We have ZDR" assumed, but the session uses a Covered Model (Fable 5/5.1) with mandatory 30-day retention | H-02, H-07, H-22 | Model ID in session | Record model ID in the routing decision; treat Fable-class as "30-day retained" unless the contract says otherwise |
| F3 | Web search query discloses client identity or matter facts | H-05, H-42 | Review of outgoing queries | Redaction rule: queries must be framed on the legal question, never on party names or distinctive facts; deny `WebSearch` for non-disclosure matters |
| F4 | Fetch of a URL whose path/query encodes confidential data (share links, search URLs) | H-05, H-06 | URL inspection | Same redaction rule for URLs; WebFetch permission rules by domain |
| F5 | Client document uploaded to a third-party parser/scraper with no stated retention and no confidentiality terms | H-43, H-44, H-47 | Tool-call audit | Parse locally; third-party document tools only for public material unless a DPA/ZDR contract is recorded |
| F6 | Scraped page stored in a shared cache and served to others | H-46 | — | `storeInCache:false` / `maxAge:0`, or not used for non-public URLs |
| F7 | Matter closed or deletion requested, but local transcripts, `history.jsonl` and auto-memory persist in plaintext and in backups | H-03, H-04 | Inspect `~/.claude` | Matter-closure checklist: `claude project purge`, delete memory directory, check backups; lower `cleanupPeriodDays`; consider `CLAUDE_CODE_SKIP_PROMPT_HISTORY` |
| F8 | Retention sweep silently paused by a settings error, so transcripts accumulate | H-03 | `/status` warning; `retention_sweep` event | Periodic check of transcript age |
| F9 | User sends `/feedback`, `/bug`, `/share` or thumbs-down on a confidential session: transcript retained 5 years and may train, even on commercial terms | H-01, H-08, H-10 | — | Set `DISABLE_FEEDBACK_COMMAND=1`; org setting to disable chat rating |
| F10 | Enterprise chat assumed to auto-delete; default is indefinite retention | H-20 | Admin settings | Set an explicit retention period |
| F11 | Reliance on a provider's deletion promise defeated by a litigation hold | H-28, H-35 | Provider notices | Treat hosted routes as "may be preserved"; keep the most sensitive material on non-disclosure or local routes |
| F12 | Free Gemini API/AI Studio key used for convenience: content trains and is human-read | H-36 | Billing status of the project | Never route confidential material to unpaid tiers; do not rely on the UK/EEA carve-out without verification |
| F13 | Local runtime assumed silent: vLLM phones home by default; Ollama cloud models/web search send prompts | H-49, H-50 | Network monitor | Set `VLLM_NO_USAGE_STATS=1`, `OLLAMA_NO_CLOUD=1`, `skipWebFetchPreflight` where a fully offline route is claimed |
| F14 | Stale routing rule: a provider term has changed since the rule was written | 3.8(c) | Evidence date older than the re-verification interval | Every routing rule cites evidence ID + retrieved-at; re-verify before relying after a set interval or on any provider notice |
| F15 | Research agent trusts a model-written fetch summary for a retention figure | H-05 ("WebFetch lossy by design") | Compare against raw text | Verify figures from raw page text, as done here |
| F16 | Client or lay user puts privileged material into a consumer chatbot independently of counsel | H-52 (US, secondary) | Intake questions | Warn at intake; treat as possible loss of confidentiality pending jurisdiction-specific advice |

---

## 6. Glossary

| Term | Meaning | Source | Note |
|---|---|---|---|
| Zero data retention (ZDR) | Provider does not store prompts/responses at rest after the response is returned; always subject to carve-outs (flagged content, law, ineligible features/models) | H-06, H-26 | Approval-gated at Anthropic and OpenAI; configuration-plus-exception at Google |
| Covered Model | Anthropic designation for models needing extra safeguards; carries 30-day minimum retention on all surfaces | H-07 | Currently Fable 5/5.1, Mythos 5/5.1 |
| Enterprise Frontier Safeguards (EFS) | Anthropic programme pairing safety monitoring with customer-controlled storage of retained data; phased from fall 2026 | H-07, H-22 | Not yet generally available |
| Abuse monitoring | Logging and review of prompts/outputs to detect policy violations | H-26, H-37, H-40 | OpenAI 30 days; Gemini API 55 days; Azure period not found |
| Modified abuse monitoring | Approved exemption from content logging/human review (OpenAI, Azure) | H-26, H-40 | Application and eligibility required |
| Consumer terms / commercial terms | Anthropic's two contract families; account type, not product, decides which applies | H-01, H-12, H-13 | |
| Customer Content | Inputs and Outputs under Anthropic Commercial Terms; deemed Customer's Confidential Information | H-12 | |
| Data processor / controller | Under the Anthropic DPA the customer is controller and Anthropic processor; on Bedrock/Google the cloud provider is the processor | H-06, H-15 | |
| inference_geo / workspace geo | Anthropic API controls for where inference runs / where data is stored | H-18 | Only "global" or "us"; "us" only |
| EU Data Boundary | Microsoft commitment to keep EU traffic in the EU; Anthropic-as-subprocessor models excluded | H-41 | |
| Unpaid / Paid Services | Gemini API tiers with opposite training rules | H-36 | |
| Temporary Chat / Incognito chat | Consumer modes excluded from training; still retained up to 30 days for safety | H-29, H-11, H-08 | |
| Application state | Data an OpenAI endpoint stores to function (threads, files, stored responses), separate from abuse logs | H-26 | |
| cleanupPeriodDays | Claude Code setting for the age at which local transcripts are swept; default 30 | H-03 | |
| Auto memory | Claude Code's self-written markdown notes per project; not swept | H-04 | |
| WebFetch domain safety check | Hostname-only call to api.anthropic.com before each fetch | H-01 | Runs on every provider |
| Legal hold / preservation order | Court- or litigation-driven duty to keep data despite deletion policy | H-28 | |
| High-Risk Use Case (Anthropic) | Usage Policy category including Legal; requires professional review and AI disclosure | H-17 | |

---

## 7. Failed retrievals and unresolved questions

Failed or degraded retrievals:

- `openai.com/*` and `help.openai.com/*`: HTTP 403 to direct `curl` and to WebFetch. Retrieved as page text through the `r.jina.ai` reader instead (H-27 to H-32, H-34). Caveat: a third-party renderer sits between this record and the page.
- `web.archive.org`: 403 via `curl`; WebFetch refuses the domain. No archived versions obtained, so no before/after diffs of any terms.
- `ai.google.dev/gemini-api/terms` and `/docs/logs-policy`: empty 302 to direct `curl`; terms retrieved via reader (H-36); logs-policy page not retrieved.
- `support.google.com/a/answer/15706919`: direct attempt failed on shell quoting; retrieved via reader (H-38).
- Anthropic Trust Centre (trust.anthropic.com), OpenAI Trust Portal, Anthropic subprocessor list, Anthropic Service Specific Terms, Google Cloud Service Specific Terms, Microsoft Product Terms/DPA: **not inspected**.
- The NYT v. OpenAI orders and the US v. Heppner opinion: only one practitioner note each was inspected (H-35, H-52); the court documents were not.

Unresolved questions:

1. **Anthropic API default retention wording conflict.** H-06 says conversation content "is not retained by default" (except Covered Models), while H-08 (1 Jul 2026) and H-01 say inputs/outputs are deleted within 30 days / "Standard: 30-day retention". Until clarified, routing should assume up to 30 days.
2. Whether the Claude consumer training toggle is pre-set to on for new users: the terms say "unless you opt out" (H-13); the toggle's default state is not stated on the inspected pages.
3. Azure OpenAI abuse-monitoring retention period: not found on current pages (H-39, H-40). Earlier documentation is widely reported to have said 30 days; not verified.
4. Which search provider sits behind Anthropic's web search backend, and that backend's own retention of queries: not found (H-05, H-19).
5. Who at Anthropic can view retained commercial content, and under what access controls: not found on the inspected public pages (likely in Trust Centre artefacts).
6. Firecrawl retention of uploaded documents and scraped content outside ZDR: not found; its privacy policy and terms (both 2024) do not address customer content.
7. Claude on Google Cloud: partner-model-specific retention beyond Anthropic's statement that the Covered Models rule follows the model: not verified on a Google page.
8. OpenAI ChatGPT Enterprise data-residency regions and any UK option: not verified.
9. What changed in the Anthropic Privacy Policy effective 10 Sep 2026: no diff performed.
10. Status of the NYT v. OpenAI discovery dispute after 5 Jan 2026, and whether the residual April–September 2025 data has been produced or deleted: not verified.
11. How English law on legal professional privilege and the SRA confidentiality duty treat each route: outside this assignment; no provider addresses it.
12. Comparative capability of local open-weight models for legal work: no sourced evidence gathered; stated only as a practical heuristic.
