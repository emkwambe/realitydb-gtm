# Honeywell International

## Overview
Global HQ: Charlotte, NC (relocated from Morris Plains, NJ in 2019).
Diversified industrial conglomerate spanning automation, building
technologies, industrial IoT, and (historically) aerospace and
advanced materials.

MAJOR STRUCTURAL CHANGE — company split into three public companies:
- **Solstice Advanced Materials (SOLS)** — spun off Oct 2025.
- **Honeywell Aerospace (HONA)** — spun off June 29, 2026. Now a
  separate public company (premier aircraft systems/tech supplier).
- **Honeywell Technologies (HON)** — the remaining Charlotte-HQ core:
  a pure-play automation company (building automation, process/
  industrial automation, Honeywell Connected Enterprise / Forge).
  Strategy framed as "automation to autonomy."

~95,000 employees (pre-split figure cited in 2025-26). CEO/Chairman
Vimal Kapur. Snowflake is the enterprise data warehouse; Azure +
Databricks lakehouse in the data-engineering stack. Honeywell Forge
is the flagship industrial IoT / analytics / EPM platform.

IMPORTANT for targeting: two distinct data orgs now exist post-split.
Honeywell Technologies (Charlotte, automation/buildings/IoT) is the
primary fit for the industrial/IoT and supply-chain packs. Honeywell
Aerospace (separate co.) carries the ITAR/EAR export-control angle.

## Data Team Signals
- **Honeywell Connected Enterprise (HCE) / Honeywell Forge**: cloud
  industrial IoT + analytics platform for owners/operators of
  buildings, plants, and (in Aerospace) airlines. Dedicated data
  science, data management, and data engineering function.
- **Chief Digital Technology Officer org (Sheila Jordan)**: owns
  Enterprise Data, consolidated 4,500 apps → ~1,000, centralized
  data on Snowflake EDW (bookings, billings, backlog, inventory).
  16+ gen AI use cases in production.
- **Chief Data Science Officer (Alexander Ross)**: leads data
  science, data management, and data engineering for the Connected
  Enterprise business.
- **Supply Chain analytics org (Chen Lin)**: building an AI-powered
  autonomous supply chain — supply chain digitization + advanced
  manufacturing + sustainability analytics.
- **Aerospace AI/Data (Ash Dhupar)**: brand-new Chief AI & Data
  Officer for Honeywell Aerospace (announced May 2026), building
  enterprise AI/data strategy from scratch across aviation,
  satellites, and defense.
- Active, ongoing hiring for Data Scientists (I / Advanced), Data
  Engineers, and Senior Data Engineers across Atlanta, Charlotte,
  and Hyderabad (2026 postings).

## Technology Stack Signals
- **Enterprise data warehouse**: Snowflake (confirmed — Sheila
  Jordan public statements).
- **Data engineering / lakehouse**: Azure + Databricks (from Senior
  Data Engineer postings: "cloud-native data and AI platforms on
  Azure using Databricks," lakehouse architecture, DAG-based
  orchestration, AI/ML data pipelines).
- **Cloud**: Azure primary; AWS and GCP also referenced in data-
  scientist postings ("cloud services from AWS, Azure, or GCP").
- **IoT / industrial platform**: Honeywell Forge; Experion control
  systems ("Experion Cognition" — probabilistic AI in the control
  system).
- **Gen AI**: Microsoft 365 Copilot, GitHub Copilot, Moveworks,
  internal "Red" virtual assistant; LangChain / agent architectures
  in newer postings.
- **Enterprise apps**: Salesforce (CRM), SAP (ERP).
- **Data science methods**: clustering, classification, regression,
  decision trees, neural networks, anomaly detection — explicitly
  for predictive/decision-making AI and (per Forge) predictive
  maintenance.

## Pain Signals
- **IoT / equipment simulation data**: Forge and predictive-
  maintenance models need realistic sensor readings, equipment
  telemetry, fault codes, and asset-health data for model
  development and testing WITHOUT waiting on real equipment or
  live customer deployments. This is the core custom-pack fit.
- **Brand-new AI/data leadership at Aerospace** (Ash Dhupar,
  May 2026): building strategy from zero, needs tooling and safe
  data fast — classic early-tenure buying window.
- **Predictive maintenance / anomaly detection at scale**: models
  for rare fault/failure events are starved of labeled failure
  data; synthetic fault-injection data accelerates development.
- **Snowflake + Databricks pipeline development**: newly
  centralized platforms need realistic non-production test data to
  build and validate pipelines (same pattern as other Snowflake
  shops).
- **Customer data sensitivity**: Forge processes operational data
  from customers' buildings/plants — can't freely reuse it for
  internal model dev; synthetic stand-ins reduce governance risk.
- **Autonomous supply chain program** (Chen Lin): building AI-
  driven supply chain needs realistic supply-chain/inventory data
  for simulation and scenario testing → direct supply-chain pack fit.

## Recent News
- **June 29, 2026**: Honeywell Aerospace spin-off completed;
  Honeywell Technologies launched as independent pure-play
  automation company (Charlotte HQ).
- **Oct 2025**: Solstice Advanced Materials spun off; updated
  business segment structure announced ahead of aerospace split.
- **May 6, 2026**: Ash Dhupar appointed Chief AI & Data Officer,
  Honeywell Aerospace (from Analog Devices CDAO; ex-BAE Systems CDO).
- **Feb 2026**: Sheila Jordan (SVP, Chief Digital Technology
  Officer) received 2026 IT Leadership Award.
- **Jan 2026**: Honeywell at NRF 2026 pushing "data to decisions"
  automated-retail story.
- Ongoing: "See, Think, Act, Learn" AI framework; Experion
  Cognition probabilistic-AI control system rollout.

## Compliance Context
- **Aerospace (HONA)**: ITAR / EAR export-control regime applies to
  defense, satellite, and aviation technical data. Real technical/
  operational data is export-controlled and cannot move freely to
  contractors, offshore dev teams, or open dev/test environments —
  synthetic data is a compliant substitute for model development.
- **Industrial data governance**: customer operational data from
  buildings/plants carries contractual confidentiality; internal
  reuse for model training is restricted.
- **Global workforce**: significant India (Hyderabad) engineering
  footprint — cross-border data movement heightens the case for
  synthetic rather than production data in offshore development.

## Entry Point Recommendation
Two parallel tracks; lead with the industrial/IoT consulting play
into Honeywell Technologies:

1. **PRIMARY — Alexander Ross (Chief Data Science Officer / VP Data
   Science, Connected Enterprise).** He owns data science + data
   engineering for Forge/HCE — the exact buyer for a custom
   industrial/IoT pack (sensor telemetry, fault codes, asset
   health). Ex-Capital One + GE Digital/Healthcare: already fluent
   in synthetic-data value and industrial IoT. Pitch a $5K–$15K
   custom pack engagement for predictive-maintenance model dev.

2. **SECONDARY — Chen Lin (VP & Chief Data Analytics Officer,
   Supply Chain Digitization).** Owns the autonomous-supply-chain
   program → immediate supply-chain pack value plus custom
   manufacturing/inventory data.

3. **HIGH-URGENCY / SEPARATE CO. — Ash Dhupar (Chief AI & Data
   Officer, Honeywell Aerospace).** Brand-new (May 2026), building
   from scratch, and the ITAR/EAR export-control angle makes the
   synthetic-data-for-model-dev pitch especially sharp. Worth a
   parallel approach even though it's now a separate entity.

Sheila Jordan (CDTO) is the enterprise-data/Snowflake owner — a
strong exec sponsor angle but higher in the org; better as a
"top-down" reference than first touch.

## Personalization Angles

### Alexander Ross (Chief Data Science Officer)
- Owns data science + engineering for Honeywell Connected
  Enterprise / Forge.
- Career at GE Digital (VP Data Science Services), GE Healthcare,
  and Capital One VP Data Science — has lived both industrial IoT
  AND a synthetic-data-heavy banking culture.
- Hook: "Forge predictive-maintenance models need realistic sensor
  telemetry and fault-code data before real equipment data exists —
  a custom RealityDB industrial pack generates it, export-safe."

### Chen Lin (Chief Data Analytics Officer, Supply Chain)
- Leading Honeywell's AI-powered autonomous supply chain +
  advanced manufacturing analytics.
- Active public "future shaper" voice on data analytics (ISC
  Analytics Summit, AME keynote).
- Hook: RealityDB supply-chain pack for immediate scenario/
  simulation testing, plus custom manufacturing-telemetry data.

### Ash Dhupar (Chief AI & Data Officer, Honeywell Aerospace)
- Brand-new role (May 2026); 2X Fortune 500 CAIDO, $300M+
  documented ROI, CDO Magazine Global Board.
- Ex-Analog Devices CDAO, ex-BAE Systems CDO — deep aerospace/
  defense + semiconductor data background.
- Hook: Building Aerospace AI/data strategy from zero under ITAR/
  EAR — synthetic sensor/telemetry/fault data lets teams (incl.
  offshore) develop models without touching export-controlled data.

### Sheila Jordan (SVP, Chief Digital Technology Officer)
- "You can't have a gen AI strategy without a data strategy."
- Consolidated to Snowflake EDW; runs 16+ gen AI use cases.
- Hook (exec-sponsor framing): safe synthetic data to feed the
  centralized Snowflake/Databricks platform for pipeline and model
  development without production/customer data exposure.

## Contacts Found

| Name | Title | LinkedIn | Notes |
|------|-------|----------|-------|
| Alexander Ross | Chief Data Science Officer / VP Data Science, Honeywell Connected Enterprise | https://www.linkedin.com/in/alexandersross/ | CONFIRMED (2026-07-17) — profile shows CDSO/VP Data Science at Honeywell, prior VP Data Science at Capital One + GE Digital/Healthcare. PRIMARY target. Owns DS + data engineering for Forge/HCE. |
| Chen Lin | VP & Chief Data Analytics Officer, Supply Chain Digitization & Advanced Manufacturing | https://www.linkedin.com/in/chenclin/ | SECONDARY. Autonomous supply chain program. URL corroborated across multiple sources — high confidence. |
| Ash Dhupar | Chief AI & Data Officer, Honeywell Aerospace | https://www.linkedin.com/in/ash-dhupar-048502/ | HIGH-URGENCY (new role May 2026, separate co.). Ex-Analog Devices, BAE Systems. ITAR/EAR angle. URL from search result — verify photo/name match. |
| Sheila Jordan | SVP & Chief Digital Technology Officer | https://www.linkedin.com/in/jordansheila | CONFIRMED (2026-07-17) — Honeywell leadership page + LinkedIn (vanity "jordansheila", Charlotte NC) confirm SVP & CDTO. Enterprise Data + Snowflake owner; exec sponsor. |
| Suresh Venkatarayalu | SVP, CTO & President, Honeywell Connected Enterprise | VERIFY MANUALLY (no personal URL found) | CANNOT CONFIRM URL (2026-07-17) — title/employer verified on honeywell.com/leadership (now "Honeywell Technologies", Charlotte), but no personal linkedin.com/in/ profile locatable. Senior sponsor over Forge. |
| David Trice | Chief Product Officer & GM, Honeywell Connected Enterprise (Forge) | https://www.linkedin.com/in/david-trice-a69973 | CONFIRMED (2026-07-17) — CPO & GM for HCE/Forge (Atlanta). Note: Crunchbase lists "CPO & GM, Connected Safety & Productivity" + possible parallel role — confirm current tenure before outreach. |

## Outreach Messages

_From Eddy Mkwambe personally (Charlotte founder, @realitydb/cli). CONSULTING play. Framing: custom industrial/IoT pack (sensor readings, equipment telemetry, maintenance records, fault codes, asset health), $5K–$15K; Forge predictive-maintenance angle; Alexander Ross already sold on synthetic data from his Capital One background. Supply-chain pack for immediate value. Compliance: ITAR/EAR export control on real technical data._

### Alexander Ross — Chief Data Science Officer / VP Data Science, Connected Enterprise (PRIMARY)

**LinkedIn connection request (299 chars)**
> Alex — coming from Capital One you already know synthetic data's value; the same play fits Honeywell Forge. Predictive-maintenance and anomaly models need realistic sensor telemetry and fault codes without real equipment data. RealityDB does exactly that. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Alex — you saw at Capital One how synthetic data unblocks model development without touching sensitive production records. The same pattern fits Honeywell Forge: predictive-maintenance and anomaly-detection models need realistic sensor telemetry, equipment readings, fault codes and asset-health data — and real equipment data is slow, sparse on failures, and export-controlled.
>
> RealityDB (@realitydb/cli) generates synthetic industrial/IoT datasets with controllable fault and edge-case distributions, deterministically seeded for reproducible model tests. A custom industrial pack ($5K–$15K) maps to Forge's exact telemetry schema.
>
> Happy to build a free Forge-relevant sample so your DS team can validate against it.
>
> Worth 15 minutes?
> — Eddy (Charlotte)

### Sheila Jordan — SVP & Chief Digital Technology Officer (SECONDARY / EXEC SPONSOR)

**LinkedIn connection request (290 chars)**
> Sheila — as CDTO you own Honeywell's enterprise data and Snowflake estate, where every team needs realistic data to build on without exposing real equipment or customer records. RealityDB generates production-shaped synthetic industrial/IoT data. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Sheila — across Honeywell's Snowflake estate, analytics and AI teams keep hitting the same blocker: they need realistic industrial and IoT data to build and test against, but real equipment telemetry is sparse on failures and often export-controlled.
>
> RealityDB (@realitydb/cli) generates synthetic industrial/IoT datasets — sensor readings, equipment telemetry, fault codes, asset health — deterministically seeded and loadable straight into Snowflake. Supply-chain data too, for immediate wins. Custom packs map to your teams' exact schemas.
>
> It's a governed, safe data layer for Forge and enterprise analytics development.
>
> Could I send your data teams a free Honeywell-relevant sample to try?
> — Eddy (Charlotte)

## Sources
- Honeywell leadership page: https://www.honeywell.com/us/en/company/leadership
- CDO Magazine — Ash Dhupar appointment: https://www.cdomagazine.tech/leadership-moves/honeywell-aerospace-appoints-ash-dhupar-as-chief-ai-data-officer
- Ash Dhupar LinkedIn (search result): https://www.linkedin.com/in/ash-dhupar-048502/
- Alexander Ross LinkedIn (search result): https://www.linkedin.com/in/alexandersross/
- Chen Lin LinkedIn: https://www.linkedin.com/in/chenclin/
- Honeywell Technologies spin-off press release (June 2026): https://www.honeywell.com/us/en/news/press-releases/2026/06/honeywell-technologies-launches-independent-pure-play-automation-company-following-honeywell-aerospace-spin-off
- Honeywell segment restructure ahead of aerospace spin-off: https://www.honeywell.com/us/en/press/2025/10/honeywell-announces-updated-business-segment-structure-ahead-of-aerospace-spin-off
- CIO.com — Honeywell transforms with gen AI (Sheila Jordan, Snowflake): https://www.cio.com/article/3816457/honeywell-transforms-with-gen-ai.html
- Sheila Jordan 2026 IT Leadership Award: https://mill-all.com/digital-diary/sheila-jordan-svp-chief-digital-technology-officer-at-honeywell-recognized-with-the-2026-it-leadership-award/
- Honeywell Forge platform: https://www.honeywell.com/us/en/solutions/honeywell-forge
- Honeywell Careers (data science): https://careers.honeywell.com/en/sites/HoneywellCareerSite/jobs?keyword=Data-Science
- Advanced Data Scientist posting (Atlanta): https://www.ziprecruiter.com/c/Honeywell/Job/Advanced-Data-Scientist/-in-Atlanta,GA?jid=63dfc89046872275
- Suresh Venkatarayalu profile (Honeywell): https://www.honeywell.com/us/en/company/leadership/suresh-venkatarayalu
