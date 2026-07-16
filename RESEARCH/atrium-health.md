# Atrium Health

## Overview
Atrium Health is a Charlotte, NC-headquartered health system operating under Advocate Health, the third-largest nonprofit integrated health system in the US (created in Dec 2022 by combining Atrium Health and Advocate Aurora Health). Advocate Health spans eight states with ~155,000 teammates, 69 hospitals, and 1,000+ care locations; Atrium is its Southeast brand covering the Carolinas, Georgia, and Alabama. Charlotte is the enterprise headquarters, making it the center of gravity for corporate data, analytics, and IT leadership.

## Data Team Signals
- **Centralized enterprise data & analytics org under a dedicated CDO.** Tina Esposito is SVP & Chief Data Officer of Advocate Health (in the CDO role since April 2023; previously Chief Health Information Officer at Advocate Aurora 2018–2023). Her org explicitly spans **cloud data engineering, data governance, and data science** — a clearly centralized, functionally-structured data organization rather than embedded pods.
- **Modern Data Platform initiative.** Esposito oversees a "modern data platform" originally envisioned to enable advanced analytics and AI, now also used to democratize integrated data on a cloud-based architecture; once business rules are applied it becomes the source for integrated data across the merged entities.
- **Post-merger data integration is an active, named priority.** Esposito has spoken publicly (Healthcare IT News, Becker's podcast, Truveta) about the "thoughtful and pragmatic" work of integrating disparate data assets from the Atrium + Advocate Aurora merger — reconciling two large systems' data into one platform.
- **Executive sponsorship above the CDO.** Rasu B. Shrestha (Enterprise EVP & Chief Strategy and Transformation Officer) provides executive leadership for enterprise data and analytics at Atrium/Advocate. Andy Crowder (SVP, Chief Digital Officer & CIO Southeast Region; former Atrium Chief Information & Analytics Officer) leads digital/IT for the Southeast region from Charlotte.
- **A distinct "Enterprise Operational Intelligence (EOI)" department** exists and is undergoing technical transformation (per the Analytics Solution Architect posting).
- **Active hiring across data roles** — dozens of data engineering, BI developer, analytics architect, and data analyst postings open (Indeed, Glassdoor, careers.atriumhealth.org), a strong pain/growth signal.

## Technology Stack Signals
From public job postings and press:
- **EHR:** Epic (system-wide; Atrium migrated off Cerner to Epic, rollouts 2021–2023). Epic analytics layer = **Clarity, Caboodle (enterprise data warehouse), and Cogito**.
- **Cloud data warehouse:** **Snowflake** (SnowPro certification listed as preferred in postings).
- **BI / reporting:** **Power BI** (and Microsoft Fabric), plus legacy **BusinessObjects** and **SSRS** — indicating a mixed/transitional BI estate.
- **Cloud platform:** cloud-based modern data platform (Snowflake-centric; industry pattern is Snowflake on Azure/AWS). Microsoft Fabric certifications preferred.
- **Governance/practices:** data governance, RBAC security models, and DevOps for analytics environments explicitly called out.
- The Analytics Solution Architect role (leading the EOI technical transformation) requires 5+ yrs data/analytics, 3+ in healthcare analytics architecture, spanning Epic Cogito + Snowflake + Power BI.

## Pain Signals
- **Two-system data reconciliation** post-merger — integrating Atrium and Advocate Aurora data assets is publicly acknowledged as ongoing and non-trivial.
- **Transitional BI estate** (BusinessObjects/SSRS → Power BI/Fabric; on-prem Epic Clarity/Caboodle → Snowflake cloud) means constant need to validate/test data pipelines against realistic-but-safe data.
- **Heavy compliance exposure around real PHI** (see below) — a direct driver of demand for HIPAA-safe synthetic data in dev/test, analytics prototyping, and vendor/partner data sharing where real records shouldn't be used.
- **Aggressive M&A pipeline** (proposed WakeMed combination, OrthoCarolina expansion) implies repeated future data-integration cycles — recurring need for safe test datasets.
- **Sustained data-engineering/analytics hiring** signals capacity strain on the data org.

## Recent News
- **July 2026:** Atrium Health + OrthoCarolina expand affiliation to build a regional/national orthopedic destination (aligning Atrium's Musculoskeletal Institute with OrthoCarolina).
- **May 2026:** Atrium/Advocate proposes a combination with **WakeMed** (Raleigh), pledging $2B+ investment in the Triangle — another large data-integration event ahead.
- **May 2026:** Atrium Health begins notifying patients of the **Oracle Health/Cerner legacy-server breach** (breach occurred Jan 2025; ~15-month notification delay) — Atrium Health Navicent among affected.
- **July 2025:** Advocate Health expands **Aidoc** AI imaging platform enterprise-wide after a 22-site pilot (WI + NC).
- **2025:** Advocate screened ~1M patients for cancer, partnered with an AI startup on clinical-trial matching.
- **March 2024:** Advocate Health became a founding member of the **Trustworthy & Responsible AI Network (TRAIN)** — a public commitment to responsible/governed AI.

## Compliance Context
- **HIPAA** is the governing regime (covered entity). Multiple recent incidents raise the compliance temperature:
  - **Oracle/Cerner business-associate breach** (2.65M+ Atrium patients cited across reporting; SSNs among exposed fields for some) with a notably delayed notification — squarely a HIPAA business-associate accountability issue now before HHS OCR.
  - **Web tracking technologies** on the patient portal (2015–2019) reported to HHS as a breach affecting ~586,000 individuals; **$1.8M** settlement.
- These make Atrium acutely sensitive to where and how **real PHI** flows into analytics, testing, and third-party/vendor environments — the exact wedge for HIPAA-safe synthetic data (ICD-10-CM, MS-DRG-coded) in non-production and data-sharing use cases.
- TRAIN membership signals appetite for **governed, auditable** data practices around AI.

## Entry Point Recommendation
**Primary: Tina Esposito, SVP & Chief Data Officer, Advocate Health.** She owns the exact functions RealityDB serves — cloud data engineering, data governance, and data science — and is publicly focused on integrating disparate post-merger data on a modern cloud platform. HIPAA-safe synthetic data for dev/test, pipeline validation, and safe data democratization maps directly to her mandate.

**Secondary / champion-level: the Enterprise Operational Intelligence (EOI) / analytics architecture leadership** (target via the Analytics Solution Architect function) — practitioners who feel the Epic Cogito → Snowflake → Power BI migration test-data pain daily and can sponsor a bottom-up pilot.

**Executive air cover:** Rasu Shrestha (enterprise data & analytics sponsor) and Andy Crowder (Charlotte-based SVP/CDO/CIO Southeast) for a top-down motion.

## Personalization Angles
1. **Post-merger data integration + M&A pipeline.** Reference Esposito's "thoughtful/pragmatic" modern-data-platform work and the pending WakeMed/OrthoCarolina integrations: every integration cycle needs realistic, HIPAA-safe test data to validate pipelines without touching real PHI across newly merged systems.
2. **Epic Cogito → Snowflake → Power BI migration.** Speak directly to the EOI transformation and BusinessObjects/SSRS → Power BI/Fabric modernization — synthetic ICD-10-CM/MS-DRG datasets let teams build and test Caboodle/Snowflake models and BI reports before real data (and its HIPAA constraints) are wired in.
3. **Compliance-driven "keep real PHI out of dev/test."** Tie to the Oracle/Cerner breach and the $1.8M web-tracker settlement plus TRAIN membership: RealityDB gives analytics/AI teams governed, HIPAA-safe data so PHI never leaves production for prototyping, vendor demos, or model development.

## Contacts Found

| Name | Title | LinkedIn | Notes |
|------|-------|----------|-------|
| Tina Esposito | SVP & Chief Data Officer, Advocate Health | https://www.linkedin.com/in/tina-esposito-19287412/ | **Top target.** Owns cloud data engineering, data governance, data science. Leads the modern data platform + post-merger data integration. In CDO role since Apr 2023; prior CHIO at Advocate Aurora. Chicago-area based but enterprise-wide (Charlotte-HQ org). Active public speaker (Becker's, Truveta, Healthcare IT News). |
| Rasu B. Shrestha | Enterprise EVP & Chief Strategy and Transformation Officer, Advocate Health / Atrium Health | Search: "Rasu Shrestha Advocate Health" LinkedIn (exact URL not verified) | Executive sponsor for enterprise data and analytics. Top-down air-cover contact. Based in Charlotte. |
| Andy Crowder | SVP, Chief Digital Officer & CIO Southeast Region, Advocate Health | https://www.linkedin.com/in/andycrowder | Charlotte-based. Former Atrium Chief Information & Analytics Officer (since 2019). CHCIO, CDH-E. Leads digital/IT for the Southeast; strong secondary exec contact. |

## Outreach Messages

_From Eddy Mkwambe personally (Charlotte founder, @realitydb/cli). Framing: HIPAA blocks production patient data from dev/test. Relevant pack: us-healthcare (ICD-10-CM, MS-DRG, HIPAA-safe, 99/100 quality). Their analysts need realistic patient-encounter data for dashboard prototyping and pipeline testing — mapping to Epic Cogito → Snowflake → Power BI._

### Tina Esposito — SVP & Chief Data Officer, Advocate Health (PRIMARY)

**LinkedIn connection request (<300 chars)**
> Tina — you own cloud data engineering, governance and data science at Advocate, and you've spoken about the pragmatic work of integrating post-merger data on a modern platform. Every integration cycle needs realistic test data that isn't real PHI. I built RealityDB for exactly that. Would love to connect.

**LinkedIn DM follow-up (<150 words)**
> Tina — integrating Atrium + Advocate Aurora data (and soon WakeMed/OrthoCarolina) means constant pipeline validation, and HIPAA means you can't use real PHI to do it.
>
> RealityDB (@realitydb/cli) generates HIPAA-safe synthetic patient data — ICD-10-CM diagnoses, MS-DRG groupings, realistic encounters and demographics — in one command, 99/100 quality, deterministically seeded so pipeline and BI tests reproduce exactly. It maps cleanly onto Epic Cogito → Snowflake → Power BI.
>
> Teams build and validate on production-shaped data while real PHI never leaves production — the governed posture your TRAIN membership points at.
>
> Could I send your team a free Atrium-relevant sample to try in a lower environment?
> — Eddy (Charlotte)

### Rasu B. Shrestha — Enterprise EVP, Chief Strategy & Transformation Officer (EXEC AIR COVER)

**LinkedIn connection request (<300 chars)**
> Rasu — as executive sponsor for Advocate's enterprise data and analytics, you own the tension between moving fast on AI and keeping real PHI out of dev/test. I built RealityDB, a CLI for HIPAA-safe synthetic patient data. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Rasu — the transformation agenda you lead hits a recurring friction: analytics and AI teams need realistic data to move fast, but HIPAA keeps real PHI out of dev, test and vendor environments.
>
> RealityDB (@realitydb/cli) resolves that with HIPAA-safe synthetic patient data — ICD-10-CM, MS-DRG, realistic encounters — generated in one command at 99/100 quality. Teams prototype dashboards, test pipelines and run vendor demos on production-shaped data with zero PHI exposure.
>
> Given the Oracle/Cerner breach and the $1.8M web-tracker settlement, it's also a clean risk-reduction story for the board.
>
> Worth a 15-minute intro with you or Tina's team?
> — Eddy (Charlotte)

### Andy Crowder — SVP, Chief Digital Officer & CIO Southeast Region

**LinkedIn connection request (<300 chars)**
> Andy — leading digital/IT for Advocate's Southeast region from Charlotte, you see the test-data pain across every Epic-to-Snowflake analytics build. Real PHI can't go into dev/test. I built RealityDB, a CLI for HIPAA-safe synthetic patient data. Would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Andy — every analytics and BI build across the Southeast region hits the same wall: you need realistic patient data to develop against, but HIPAA keeps real PHI out of dev, test and QA.
>
> RealityDB (@realitydb/cli) generates HIPAA-safe synthetic patient data — ICD-10-CM, MS-DRG, realistic encounters and demographics — in one command, 99/100 quality, deterministically seeded so tests reproduce. It fits Epic Cogito → Snowflake → Power BI directly.
>
> Your teams get production-shaped data for dashboard prototyping and pipeline testing while PHI stays in production.
>
> Can I send a free Atrium-relevant sample for your team to try?
> — Eddy (Charlotte)

## Sources
- https://www.healthcareitnews.com/news/advocates-cdo-offers-tips-experience-integrating-post-acquisition-data-assets (Esposito, data org structure, modern data platform) — accessed via search snippet (page 403 on direct fetch)
- https://theorg.com/org/advocate-health-1/org-chart/tina-esposito
- https://www.truveta.com/blog/news/tina-esposito-advocate-health/
- https://www.beckershospitalreview.com/podcasts/podcasts-beckers-hospital-review/tina-esposito-senior-vice-president-and-chief-data-officer-at-advocate-health-131945477/
- https://www.linkedin.com/in/tina-esposito-19287412/
- https://www.linkedin.com/in/andycrowder
- https://atriumhealth.org/about-us/newsroom/news/2019/07/ah-ciao-announcement (Crowder Chief Information & Analytics Officer)
- https://atriumhealth.org/about-us/newsroom/news/2022/12/advocate-health-names-executive-leadership-team (Shrestha, enterprise data & analytics)
- https://atriumhealth.org/about-us/leadership/rasu-b-shrestha
- https://careers.atriumhealth.org/jobs/17193816-analytics-solution-architect (EOI, Epic Cogito, Snowflake, Power BI, RBAC, governance)
- https://careers.atriumhealth.org/jobs/16918632-business-intelligence-developer-epic-cogito-clarity-caboodle
- https://atriumhealth.org/about-us/newsroom/news/2020/02/atrium-health-selects-epic-for-implementation-of-electronic-health-records-across-three-states (Epic adoption)
- https://www.healthcareitnews.com/news/atrium-health-drop-cerner-move-epic-ehr-system
- https://www.hipaajournal.com/2-65-million-atrium-health-patients-impacted-by-business-associate-data-breach/ (Oracle/Cerner breach)
- https://www.thecybersignal.com/atrium-health-oracle-cerner-breach-16-health-systems-2026/
- https://www.hipaajournal.com/atrium-health-tracking-technologies-patient-portal/ (web tracker breach, ~586k)
- https://www.govinfosecurity.com/atrium-health-to-pay-18m-to-settle-web-tracker-lawsuit-a-32170 ($1.8M settlement)
- https://www.advocatehealth.org/news/advocate-health-deploys-ai-solution-to-redefine-diagnostic-excellence-through-agreement-with-aidoc (Aidoc, July 2025)
- https://atriumhealth.org/about-us/newsroom/news/2026/07/atrium-health-and-orthocarolina-join-forces-to-build-nationally-recognized-orthopedic-destination
- https://www.healthcaredive.com/news/atrium-health-wakemed-propose-to-merge-north-carolina/819246/ (WakeMed, May 2026)
- https://en.wikipedia.org/wiki/Advocate_Health (size, footprint, TRAIN founding member)
