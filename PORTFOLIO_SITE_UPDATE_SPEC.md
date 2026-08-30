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

The current `CONNECTED REPOS` number is a weak metric because repository count can include small supporting repos, collaborative repositories, and forks.

Recommended metric block:

| Metric | Value |
|---|---:|
| Automation systems documented | 7 |
| Cloud platforms | 3 |
| Feature branches validated | 40+ |
| User roles regression tested | 6 |

## 2. Featured work

Featured cards should prioritise clearly authored, inspectable evidence.

### Featured card 1

**AI Agency Lead Capture & Qualification**  
Category: AI Automation  
Stack: n8n, Google Sheets, Gmail  
Proof: five tested routing outcomes, public portfolio-safe n8n JSON, architecture, and qualification logic  
Link: `https://github.com/Dudubynatur3/ai-automation-portfolio/tree/main/01-ai-agency-lead-qualification`

Suggested summary:

> Deterministic lead qualification system that classifies enquiries by timeline and budget, records the final status in Google Sheets, and triggers immediate customer acknowledgement. Five final routing outcomes were tested.

### Featured card 2

**WhatsApp AI Order Processor**  
Category: AI Automation  
Stack: n8n, Twilio pattern, OpenAI, Google Sheets, Stripe pattern, Telegram  
Proof: detailed README, workflow screenshot, importable demo JSON  
Link: `https://github.com/Dudubynatur3/whatsapp-order-processor`

Keep the repository's explicit `Demo Mode` wording so mocked integrations are not represented as live commercial integrations.

### Featured card 3

**AWS High-Availability 3-Tier System**  
Category: Cloud Infrastructure  
Stack: AWS, Terraform, EC2, ALB, RDS MySQL, NAT Gateway, Nginx, Next.js  
Link: `https://github.com/Dudubynatur3/aws-3tier-terraform-nextjs`

Why this is a stronger feature than the current fork-derived cards:

- original repository, not a fork
- clear architecture documentation
- three network tiers
- public and internal ALBs
- RDS Multi-AZ and read replica
- infrastructure teardown guidance
- screenshots and troubleshooting evidence already present

## 3. Cloud supporting work

Immediately below the three headline cards, surface a compact Cloud / DevOps row with:

### GCP End-of-Training Terraform Project

Link: `https://github.com/Dudubynatur3/gcp-exercise`

Evidence includes Terraform VPC/subnets, Compute Engine, IAM, Linux, Flask, Cloud SQL, GKE, GCP folder hierarchy, and hands-on screenshots.

### EpicBook Full-stack Infrastructure

Link: `https://github.com/Dudubynatur3/epicbook-fullstack`

Evidence includes Azure, Terraform, Ansible, Nginx, and infrastructure automation.

### Automated Developer Onboarding

Link: `https://github.com/Dudubynatur3/dev-onboarding-automation`

Evidence includes Terraform, AWS, Bash, Linux user/group management, and repeatable onboarding automation.

## 4. Remove two current cards from authored-work positioning

### `3-Tier-MERN-App`

GitHub metadata identifies `Dudubynatur3/3-Tier-MERN-App` as a fork of `AkingbadeOmosebi/Aksforge`.

User clarification confirms that it was only forked and no personal implementation work was performed in that repository.

**Decision: remove it from the portfolio site as personal engineering evidence.**

It does not need to be deleted from GitHub, but the portfolio should not claim its production, GitOps, security, or observability implementation as authored work.

### `Azure-Terraform-Project`

GitHub metadata identifies `Dudubynatur3/Azure-Terraform-Project` as a fork of `vincegwu/aks-terraform-project`.

User clarification: this was the final collaborative group project in the Cloud Advisory training. Vince created the shared repository and Aduroja Akintade completed his assigned project contribution.

**Decision: remove it from Featured Work.**

The experience can remain in career history as collaborative Cloud Advisory project work, but the entire repository should not be presented as independently authored. A future case study is acceptable only if the specific personal contribution can be isolated and evidenced.

## 5. New AI Automation Systems section

Add a dedicated section after Featured Work or immediately before Production Experience.

Heading suggestion:

> AI automation systems.  
> Built around operational failure points.

Include:

1. AI Agency Lead Capture & Qualification
2. MedFlow Intake OS
3. Cupid Errands Intelligent Email Routing
4. RAG & AI Agent Workflows
5. WhatsApp / Chatwoot CRM Automation
6. AI-Assisted Customer Support with Human Review
7. Self-Hosted n8n Platform
8. WhatsApp AI Order Processor, linked to its standalone repository

Each item should expose:

- business problem
- workflow architecture
- stack
- implementation classification
- evidence link
- testing / control evidence

## 6. MedFlow wording

The connected Airtable base is now the strongest data-model source of truth and directly confirms a **six-table relational system**:

- `Patients`
- `Intakes`
- `Cases`
- `Tasks`
- `Routing_Log`
- `Staff`

Correct public evidence:

- Jotform → Make.com → Airtable → Google Sheets → Gmail/Outlook → Google Calendar
- duplicate checking using email with normalized-phone fallback
- patient create/update plus separate intake records
- case creation from routed intakes
- task generation and staff assignment
- relational links across patients, intakes, cases, tasks, routing logs, and staff
- synthetic data only
- HIPAA-aware design discussion, not HIPAA compliance
- append-oriented audit logging
- consent and missing-data routing controls
- masked identifiers in routing/audit evidence

The earlier four-table note came from an incomplete documentation snapshot and should no longer be used for the portfolio or CVs.

Detailed schema evidence: `02-medflow-intake-os/DATA_MODEL.md`.

## 7. Production experience

Keep the YTRanker section substantially as it is.

Retain:

- private production code label
- March 2026 to July 2026 timeframe
- React, Supabase, Vercel platform context
- 40+ feature branches validated
- 6 user roles regression tested
- technical handover
- verified Upwork client feedback

Add a link to:

`https://github.com/Dudubynatur3/ai-automation-portfolio/blob/main/commercial-case-studies/ytranker.md`

Do not link to the private source repository.

## 8. Working philosophy

Keep:

> Automation is useful. Reliability is the product.

Supporting copy should explicitly mention:

- deterministic logic where AI is unnecessary
- AI classification where interpretation is required
- fallbacks and human review
- deduplication
- auditability
- testing
- documentation and handover

## 9. Repository hierarchy

Add the new repository prominently:

`https://github.com/Dudubynatur3/ai-automation-portfolio`

Do not enumerate every public repository as equal proof. Use four evidence tiers:

### Featured authored systems
High-confidence, inspectable work.

### Supporting authored repositories
Smaller app/infrastructure repositories supporting the engineering history.

### Collaborative training work
Group work with the user's own contribution described precisely.

### Forks / references
Not used as personal engineering evidence unless an independent contribution is explicitly documented.

See `CLOUD_REPOSITORY_AUDIT.md` for the current classification.

## 10. Navigation

Keep:

- Work
- Experience
- About
- Let's talk

Within Work, use:

`All | AI Automation | Cloud / DevOps | SaaS & Integrations`

## 11. Publication gate

Before the revised site is treated as application-ready:

- verify every project link
- remove the 3-Tier-MERN fork from personal work
- remove the Azure group-project fork from Featured Work
- add the new AI Automation Portfolio
- test mobile layout
- test every CTA
- confirm email / LinkedIn / GitHub links
- verify no screenshot exposes credentials or customer data
- ensure project classifications are visible
- verify AI Automation Portfolio links render correctly
- ensure MedFlow is consistently described as the verified six-table implementation
