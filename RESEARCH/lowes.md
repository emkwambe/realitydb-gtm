# Lowe's Companies, Inc.

## Overview
Fortune 50 home-improvement retailer. HQ: Mooresville, NC
(Charlotte metro). ~1,700+ stores, 300,000+ associates,
millions of daily customer interactions. Operates a dedicated
Charlotte Technology Hub ("Charlotte Technology Hub 3505") —
its global technology center — actively hiring engineers, data
scientists, ML engineers, and architects.

Tech org led by Seemantini Godbole (EVP, Chief Digital &
Information Officer). Data/AI org led by Chandhu Nair (SVP,
Data, AI & Innovation), who reports to Godbole. Aggressive
AI-first modernization underway, driven from the top by CEO
Marvin Ellison. No dedicated "Chief Data Officer" title exists;
Chandhu Nair is the de facto data leader.

Hybrid data platform: Google Cloud (BigQuery) for e-commerce
and large-scale workloads, on-prem data centers for heavy model
training, and in-store edge GPU systems for inference/computer
vision. Legacy Teradata warehouse plus Hadoop/Spark/Kafka
ecosystem still visible in job postings.

## Data Team Signals
- **Chandhu Nair (SVP Data, AI & Innovation)** publicly leads a
  centralized data org spanning: an economics group, big-data
  engineering, data science, and an advanced analytics group.
  Explicitly consolidated to "centralize data collecting
  capabilities."
- Director/principal layer exists: Venkat Swarna (Principal
  Engineer/Director, Data — Mooresville) and a "Sr. Director,
  Data Engineering & AI" title appear on LinkedIn.
- Active, ongoing hiring across the Charlotte Tech Hub: Lead
  Data Engineer, Associate Data Engineering (Launchpad early-
  career pipeline), Data Scientist, Data Engineer - GCP, Data
  Engineer - Spark, Sr. Director Technology (Media/Customer
  Analytics, Measurement & Data Science). Signals sustained team
  growth, not a one-off.
- CDO Magazine (Nov 2025) profiled Lowe's data transformation:
  standardizing data management and governance across "thousands
  of stores and systems," building a semantic data layer.
- Quote (Nair, CDO Magazine): "We had severe technical debt to
  the point where we couldn't print our receipts." Signals a
  data estate still being consolidated and modernized.

## Technology Stack Signals
- **Cloud:** Google Cloud Platform (BigQuery for analytics /
  e-commerce). Hybrid on-prem data centers for model training;
  in-store edge GPU inference.
- **Warehouse:** BigQuery (modern); Teradata (legacy, still in
  job reqs).
- **Streaming:** Apache Kafka; Spark Streaming.
- **Processing / big data:** Apache Spark (incl. MLlib), Hadoop
  ecosystem — Hive, Pig, Sqoop, MapReduce, Ambari, Ranger.
- **Languages:** Python, Java, Scala, SQL.
- **ML/AI:** Enterprise gen-AI (Mylow / Mylow Companion
  associate assistant built with OpenAI); computer vision at
  edge; "AI Transformation Office" governance framework.
- **Supply chain:** Expanded partnership with Relex Solutions
  for AI forecasting, replenishment, and allocation; 3-year
  program to modernize inventory replenishment & demand planning.
- **MarTech:** Largely in-house core database + marketing tech,
  third parties for journey automation.

## Pain Signals
- **Customer purchase history + loyalty data is core and
  sensitive.** MyLowe's Rewards has 30M+ members who spend ~50%
  more than non-members; the loyalty program is described as the
  "spine" for personalization. This is exactly the SKU-level
  transaction + loyalty data that cannot be freely copied into
  dev/test/analytics sandboxes.
- Heavy technical debt and multi-year consolidation of "thousands
  of stores and systems" — many teams building pipelines against
  disparate/legacy sources need realistic test data.
- Large early-career and contractor data-engineering intake
  (Launchpad, GCP/Spark roles) → many new engineers needing
  safe, representative datasets to develop against without prod
  access.
- Supply-chain modernization (Relex + in-house, 3-year program)
  = active pipeline development for forecasting/replenishment/
  allocation — a natural fit for a synthetic supply-chain dataset.
- Data science + advanced analytics groups building
  personalization models need loyalty/transaction distributions
  they can share and iterate on without exposing PII.

## Recent News
- Oct 2025 (Forbes / Constellation Research): Lowe's positions AI
  as foundation for the future of home improvement; gen-AI to
  enhance associate + customer experience, drive traffic/sales.
- Nov 2025 (CDO Magazine): "Lowe's Data Transformation Playbook"
  — Chandhu Nair details hybrid cloud/on-prem/edge strategy,
  semantic data layer, AI Transformation Office, six "lighthouse"
  investment areas.
- 2025 Total Home Strategy: five growth pillars — Pro
  Penetration, Online Sales, Home Services, Loyalty Ecosystem,
  Space Productivity; new AI framework; first U.S. home-
  improvement product marketplace.
- Mylow / Mylow Companion AI associate tool (built with OpenAI)
  rolled out to stores.
- Supply chain: expanded Relex Solutions partnership to unify
  inventory planning + replenishment; new distribution-center
  network expansion.

## Compliance Context
US retailer handling payment + loyalty data:
- **PCI-DSS** — cardholder data cannot flow into dev/test.
- **State privacy laws** (CCPA/CPRA and successors) — customer
  purchase history and loyalty profiles are regulated personal
  information; minimization and purpose-limitation restrict use
  of real customer data in non-production environments.
- 30M+ loyalty members' behavioral data is a high-value,
  high-liability asset. Standard practice is to keep it out of
  developer sandboxes — creating demand for realistic synthetic
  substitutes.

## Entry Point Recommendation
Lead with the **supply-chain pack** as the low-friction entry
point: Lowe's has an active, named, multi-year supply-chain
modernization program (Relex + in-house, forecasting/
replenishment/allocation) where engineers are building pipelines
right now. A ready synthetic supply-chain dataset delivers
immediate value for those teams and requires no procurement
drama.

Then expand to the **custom us-retail pack** consulting play
($2,500–$10,000): SKU-level transactions, store performance,
inventory movement, and MyLowe's-style loyalty data — the exact
data domains Lowe's cannot freely replicate into dev/test/
analytics environments. Personalization + loyalty is Lowe's
stated strategic "spine," so a synthetic loyalty/transaction
generator maps directly onto a board-level priority.

Primary target: **Chandhu Nair (SVP, Data, AI & Innovation)** —
owns the whole data org and the modernization mandate. For a
warmer, more technical first touch, a Director/Principal in data
engineering (e.g., Venkat Swarna) is a better initial reply-rate
bet, then escalate.

## Personalization Angles

### Chandhu Nair (SVP, Data, AI & Innovation)
- Publicly framed the challenge as consolidating data across
  "thousands of stores and systems" with severe technical debt.
- Hook: teams modernizing that estate need realistic, shareable
  test data that never touches production loyalty/POS records.
- Reference his CDO Magazine "data transformation playbook" and
  the semantic-data-layer / governance narrative — synthetic
  data is a governance win (dev/test without PII exposure).
- Former CEO/co-founder of Cognitive Retail (AI retail analytics)
  — he already thinks in data-product terms; speak ROI + velocity.

### Director / Principal Data Engineering (e.g., Venkat Swarna)
- Building analytics application + data-engineering teams in
  Mooresville on GCP/BigQuery/Spark/Kafka.
- Hook: onboarding waves of new + early-career engineers
  (Launchpad) who need safe, representative data to build
  pipelines — synthetic supply-chain/retail data removes the
  prod-access bottleneck.

### Seemantini Godbole (EVP, CDIO) — executive air-cover
- Owns the enterprise tech transformation and AI-first strategy.
- Not the first-call buyer, but the name to reference for
  strategic alignment ("supports your data-and-AI transformation
  without expanding PII exposure").

## Contacts Found

| Name | Title | LinkedIn | Notes |
|------|-------|----------|-------|
| Chandhu Nair | SVP, Data, AI & Innovation (also Stores; leads data/analytics org, Innovation Labs, marketing tech) | https://www.linkedin.com/in/chandhunair/ | PRIMARY buyer. Reports to Godbole. Ex-CEO/co-founder Cognitive Retail. Joined Lowe's 2020. Public data-strategy spokesperson (CDO Magazine, DataIQ 100). URL matches profile in search; confirm before outreach. |
| Seemantini Godbole | EVP, Chief Digital & Information Officer | https://www.linkedin.com/in/seemantini-godbole-241a4a1/ | Owns enterprise tech + AI transformation. Executive sponsor / air-cover, not first call. Joined 2018, 25+ yrs tech. |
| Venkat Swarna | Principal Engineer / Director, Data (Mooresville) | https://www.linkedin.com/in/venkat-swarna-37029a28/ | CONFIRMED (2026-07-17) — profile title "Principal Engineer/Director, Data" at Lowe's, Mooresville NC; corroborated by ZoomInfo/RocketReach. Warm technical entry point. |
| Saurabh K | Sr. Director, Data Engineering & AI — Lowe's India (Bengaluru) | https://in.linkedin.com/in/saurabh-k-73319623 | UPDATED (2026-07-17) — India-based (Lowe's India / Bengaluru GCC), NOT Charlotte/Mooresville. No US-based namesake in this role found. De-prioritize for Charlotte outreach. |
| Naveen S. | Sr. Data Engineer (Charlotte) | https://www.linkedin.com/in/naveen-s-aa2b7179/ | IC-level, not a buyer. Useful for tech-stack validation only. |

## Outreach Messages

_From Eddy Mkwambe personally (Charlotte-area founder, @realitydb/cli). Framing: PCI-DSS + CCPA/CPRA keep real customer purchase/loyalty data out of dev/test. Entry = supply-chain pack; consulting play = custom us-retail pack (transactions, inventory, loyalty, store performance, SKU-level), $2.5K–$10K._

### Chandhu Nair — SVP, Data, AI & Innovation (PRIMARY)

**LinkedIn connection request (297 chars)**
> Chandhu — MyLowe's Rewards and SKU-level purchase data are the spine of your personalization work, but PCI-DSS and CCPA keep that real customer data out of dev/test. RealityDB generates production-shaped synthetic retail data so teams build safely. Charlotte-area founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Chandhu — your data/AI modernization runs on loyalty and SKU-level transaction data, and PCI-DSS/CCPA mean none of it can safely sit in dev, test or analytics sandboxes.
>
> RealityDB (@realitydb/cli) generates production-shaped synthetic retail data — transactions, inventory, loyalty, store performance, SKU-level detail — deterministically seeded so pipelines and models are reproducible, with zero real customer PII. My supply-chain pack is a fast first win for the forecasting/replenishment work; a custom us-retail pack ($2.5K–$10K) matches your exact schema.
>
> Happy to generate a free Lowe's-shaped sample so your team can drop it into a lower environment and see the fit.
>
> Worth 15 minutes?
> — Eddy (Charlotte)

### Seemantini Godbole — EVP, Chief Digital & Information Officer (EXEC SPONSOR)

**LinkedIn connection request (300 chars)**
> Seemantini — as you drive Lowe's enterprise tech and AI transformation, one recurring blocker is realistic data teams can build on without putting real customer purchase/loyalty records (PCI-DSS/CCPA) into lower environments. RealityDB solves exactly that. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Seemantini — every AI and analytics initiative under your org eventually hits the same wall: teams need production-shaped data to build against, but PCI-DSS and CCPA keep real customer purchase and loyalty data out of dev, test and vendor environments.
>
> RealityDB (@realitydb/cli) generates synthetic retail data — transactions, inventory, loyalty, store/SKU-level — deterministically seeded and free of real PII. It's a supply-chain pack for immediate wins, with custom us-retail datasets built to Lowe's schema.
>
> It accelerates every team that's currently waiting on safe data access.
>
> Could I send your data leaders a free Lowe's-relevant sample to try?
> — Eddy (Charlotte)

### Venkat Swarna — Principal Engineer / Director, Data (WARM TECHNICAL ENTRY)

**LinkedIn connection request (298 chars)**
> Venkat — building Lowe's analytics/data-eng pipelines means constantly needing realistic data for dev/test, and real customer purchase/loyalty data can't go there (PCI-DSS/CCPA). RealityDB generates production-shaped synthetic retail data in one command. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Venkat — hands-on pipeline work needs production-shaped test data, and PCI-DSS/CCPA keep real customer purchase and loyalty records out of dev, test and QA.
>
> RealityDB (@realitydb/cli) generates synthetic retail data — transactions, inventory, loyalty, store/SKU-level — from one command, deterministically seeded so a failing pipeline test reproduces exactly. It loads straight into BigQuery/Spark, no prod-data request needed. My supply-chain pack is the quickest way to see it work.
>
> Happy to generate a free sample shaped to one of your pipelines so you can try it locally.
>
> Want me to send it over?
> — Eddy (Charlotte)

## Sources
- https://corporate.lowes.com/who-we-are/lowes-leadership/senior-leadership/chandhu-nair
- https://corporate.lowes.com/who-we-are/lowes-leadership/executive-leadership/seemantini-godbole
- https://www.cdomagazine.tech/digital-transformation/lowes-data-transformation-playbook-how-a-retail-giant-is-modernizing-for-an-ai-first-future
- https://www.forbes.com/sites/randybean/2025/10/28/at-lowes-ai-is-laying-the-foundation-for-the-future-of-home-improvement/
- https://www.constellationr.com/insights/news/lowes-betting-ai-drive-customer-experience-optimize-multiple-processes
- https://corporate.lowes.com/newsroom/stories/inside-lowes/tech-transformation-lowes-chooses-charlotte-global-technology-center
- https://talent.lowes.com/us/en/job/JR-02491283/Lead-Data-Engineer
- https://talent.lowes.com/us/en/data-analytics-consumer-insights-jobs
- https://builtin.com/job/data-engineer/3631414
- https://www.marketingdive.com/news/lowes-mylowes-rewards-loyalty-personalization-retail-media-network/710766/
- https://www.modernretail.co/operations/how-lowes-created-an-ecosystem-of-different-loyalty-programs-for-pros-and-homeowners/
- https://www.supplychaindive.com/news/lowes-taps-tech-to-unify-inventory-planning-replenishment/817704/
- https://www.dataiq.global/dataiq100/chandhu-nair-senior-vice-president-data-and-ai-innovation-labs-and-marketing-technology-lowes-inc/
- https://www.linkedin.com/in/chandhunair/
- https://www.linkedin.com/in/seemantini-godbole-241a4a1/
- https://www.linkedin.com/in/venkat-swarna-37029a28/
