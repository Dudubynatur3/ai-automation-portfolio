# Portfolio Site Update Specification

This document defines the next update to the existing engineering portfolio site after creation of the AI Automation Portfolio repository.

## Keep the current visual system

The existing site already has a strong visual identity:

- cream / black / lime palette
- large editorial typography
- clear systems-engineering positioning
- distinct production-experience section
- direct GitHub / LinkedIn / email calls to action

A rebuild in another website builder is not required at this stage. The priority is evidence accuracy and stronger automation representation.

## 1. Hero section

Keep:

> I engineer the systems behind the outcome.

Keep the supporting positioning around AI Automation with a Cloud / DevOps foundation.

### Replace the repository-count metric

The current `CONNECTED REPOS` number is a weak metric because repository count can include small supporting repos and forks.

Recommended metric block:

| Metric | Value |
|---|---:|
| Automation systems documented | 7 |
| Cloud platforms | 3 |
| Feature branches validated | 40+ |
| User roles regression tested | 6 |

This is more meaningful and less likely to become stale when a repository is added.

## 2. Featured work

The featured cards should prioritise authored, inspectable evidence.

### Recommended featured card 1

**AI Agency Lead Capture & Qualification**  
Category: AI Automation  
Stack: n8n, Google Sheets, Gmail  
Proof: five tested routing outcomes, public portfolio-safe n8n JSON, architecture and qualification logic  
Link: `https://github.com/Dudubynatur3/ai-automation-portfolio/tree/main/01-ai-agency-lead-qualification`

Suggested summary:

> Deterministic lead qualification system that classifies enquiries by timeline and budget, records the final status in Google Sheets, and triggers immediate customer acknowledgement. Five final routing outcomes were tested.

### Recommended featured card 2

**WhatsApp AI Order Processor**  
Category: AI Automation  
Stack: n8n, Twilio pattern, OpenAI, Google Sheets, Stripe pattern, Telegram  
Proof: detailed README, workflow screenshot, importable demo JSON  
Link: `https://github.com/Dudubynatur3/whatsapp-order-processor`

Keep this card, but preserve the repo's explicit `Demo Mode` wording so mocked integrations are not represented as live commercial integrations.

### Recommended featured card 3

**EpicBook Full-stack Infrastructure**  
Category: Cloud / Infrastructure as Code  
Stack: Azure, Terraform, Ansible, Nginx  
Link: `https://github.com/Dudubynatur3/epicbook-fullstack`

This repository is not a GitHub fork and is the cleaner cloud project to feature prominently.

## 3. Remove two current featured cards from authored-work positioning

### `3-Tier-MERN-App`

GitHub metadata identifies `Dudubynatur3/3-Tier-MERN-App` as a **fork** of `AkingbadeOmosebi/Aksforge`.

The fork's current head is an upstream-authored commit. It should therefore **not** be presented as an authored production-grade platform project unless separate, verifiable personal contributions are identified.

Recommended action: remove it from Featured Work. If retained anywhere, label it clearly as a forked lab/reference project and specify only independently verified personal contributions.

### `Azure-Terraform-Project`

GitHub metadata identifies `Dudubynatur3/Azure-Terraform-Project` as a **fork** of `vincegwu/aks-terraform-project`.

The fork and upstream repository currently point to the same main-branch commit. It should therefore **not** be presented as an independently authored `Azure Internal Developer Platform` project.

Recommended action: remove it from Featured Work. Do not use it as primary portfolio evidence unless personal changes are later documented separately.

## 4. New AI Automation Systems section

Add a dedicated section after Featured Work or immediately before production experience.

Heading suggestion:

> AI automation systems.  
> Built around operational failure points.

Include cards / rows for:

1. AI Agency Lead Capture & Qualification
2. MedFlow Intake OS
3. Cupid Errands Intelligent Email Routing
4. RAG & AI Agent Workflows
5. WhatsApp / Chatwoot CRM Automation
6. AI-Assisted Customer Support with Human Review
7. Self-Hosted n8n Platform
8. WhatsApp AI Order Processor (standalone repository)

Each item should expose:

- business problem
- system / workflow architecture
- stack
- implementation classification
- evidence link
- testing / control evidence

## 5. MedFlow wording

Use the recovered project package as the source of truth.

Correct public evidence:

- Jotform → Make.com → Airtable → Google Sheets → Gmail/Outlook → Google Calendar
- Airtable tables documented in the original package: `Patients`, `Intakes`, `Routing_Log`, `Staff`
- synthetic data only
- HIPAA-aware design discussion, not HIPAA compliance
- append-only audit log
- consent and missing-data routing controls
- minimal-data-routing for notifications and audit evidence

Do not describe MedFlow as a six-table system unless another later implementation with direct evidence is separately recovered.

## 6. Production experience

Keep the YTRanker section substantially as it is.

Strengths to retain:

- private production code label
- March 2026 to July 2026 timeframe
- React, Supabase, Vercel platform context
- 40+ feature branches validated
- 6 user roles regression tested
- technical handover
- verified Upwork client feedback

Add a link to the public case-study write-up:

`https://github.com/Dudubynatur3/ai-automation-portfolio/blob/main/commercial-case-studies/ytranker.md`

Do **not** link to the private production source repository.

## 7. Working philosophy

Keep:

> Automation is useful. Reliability is the product.

This is strongly aligned with the evidence architecture in the new repository.

The supporting copy should explicitly mention:

- deterministic logic where AI is unnecessary
- AI classification where interpretation is required
- fallbacks and human review
- deduplication
- auditability
- testing
- documentation and handover

## 8. Repository links

Add the new repository prominently:

`https://github.com/Dudubynatur3/ai-automation-portfolio`

The site should no longer simply enumerate every public repository as equal proof. Use three evidence tiers:

### Featured authored systems
High-confidence, inspectable work.

### Supporting repositories
Smaller app/infrastructure repos that support the engineering history.

### Forked / learning references
Only if useful, explicitly labelled as forks or labs. Never present these as independently authored systems.

## 9. Final portfolio navigation

Recommended top navigation remains simple:

- Work
- Experience
- About
- Let's talk

Within Work, add filter labels:

`All | AI Automation | Cloud / DevOps | SaaS & Integrations`

## 10. Publication gate

Before the revised site is treated as application-ready:

- verify every project link
- remove or relabel fork-derived claims
- test mobile layout
- test every CTA
- confirm email / LinkedIn / GitHub links
- verify no screenshot exposes credentials or customer data
- ensure project classifications are visible
- ensure new AI Automation Portfolio links render correctly
