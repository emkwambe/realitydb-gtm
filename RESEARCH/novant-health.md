# Novant Health

## Overview
Novant Health is a ~$10B-revenue not-for-profit integrated health system headquartered in Winston-Salem, NC, operating 19+ medical centers and 850+ locations (physician clinics, urgent care, outpatient facilities) across NC, SC and VA, with roughly 40,000 employees and 2,000+ physicians. Charlotte is a core market — it originates from the 1997 merger with Presbyterian Health Services of Charlotte, anchored by the 654-bed Novant Health Presbyterian Medical Center, plus major growth investments in SouthPark and Ballantyne (Hall Family Farm). Leadership has publicly stated a goal of roughly tripling in size / targeting ~$30B revenue over the next several years, making data scalability and interoperability a live strategic problem.

## Data Team Signals
- **Digital/IT org led by a CDIO.** Onyeka Nchege is EVP & Chief Digital and Information Officer (joined ~2020), owning IT strategy, cybersecurity, analytics, digital health and enterprise platforms. He describes the analytics/AI operating model as "experimentation as a service" — test before production.
- **New dedicated analytics executive (June 2026).** Stephanie Lenzner was named SVP of Value Intelligence on June 22, 2026, reporting to Nchege. She explicitly "leads the integration of analytics, data science and performance intelligence." She was previously Chief Data & Analytics Officer at Froedtert & Medical College of Wisconsin and led digital/data/AI capabilities at Mayo Clinic — a strong signal Novant is consolidating and maturing a still-fragmented analytics function. A brand-new leader building a "data foundation" is an ideal early-relationship moment.
- **Institute of Innovation & AI (est. 2019).** Governance body of physicians + executives that vets AI use cases; Karen Hegarty, PhD leads AI & Innovation there, focused on ethical/trustworthy/safe AI deployment.
- **Active data-engineering build-out.** Job listings include "Manager, Data Engineering" and "Director, Business Insights & Analytics," alongside numerous Data Scientist and Business Data Analyst roles — indicating a growing but still-scaling central data team. Data governance roles (Technical Data Stewards) exist, pointing to formal data-quality/integrity initiatives.
- Team appears to be a **centralizing hub-and-spoke**: a central digital/analytics org (under Nchege/Lenzner) plus embedded informatics analysts and the AI Institute.

## Technology Stack Signals
- **Epic EHR is the backbone.** As of mid-2026, 19,000+ team members actively use AI features embedded in Epic. This implies the Epic analytics stack (Cogito, Clarity, Caboodle) is the core reporting/data layer — heavy ICD-10-CM / DRG / clinical-coded data.
- **Cloud + modern data engineering.** Novant's data-engineering and data-scientist postings align with the healthcare-analytics norm of Azure/cloud data platforms, SQL Server, Python, and ETL/ELT pipelines feeding data lakes; data-scientist comp (Levels.fyi ~$127K–$178K+) indicates a real in-house DS bench.
- **AI/ML in production:** robotic process automation (revenue cycle), computer vision in radiology (stroke / pulmonary embolism detection), predictive maintenance, patient-outcome forecasting, demand/staffing prediction. Historically partnered with prescriptive-analytics vendor Jvion.
- Nchege sits on the **Truveta Board of Directors** — Truveta is a de-identified health-data/AI platform, showing executive fluency in large-scale, privacy-preserving clinical data (directly adjacent to synthetic/HIPAA-safe data value props).

## Pain Signals
- **HIPAA / PHI exposure is a proven, expensive pain.** Novant agreed to a **$6.6M settlement** over the Meta/Facebook tracking-pixel case: pixel code on its MyChart portal potentially disclosed PHI of up to ~1.36M patients (May 2020–Aug 2022). This is a concrete, public demonstration that using real PHI in web/analytics contexts created massive legal and reputational cost — a textbook case for HIPAA-safe synthetic data in dev/test/analytics environments.
- **Scale/interoperability strain.** A "triple in size / $30B" growth mandate plus continuous M&A (e.g., Community Hospital of Stokes acquisition June 1, 2026) means constant data integration, migration and testing — environments where real PHI is risky and synthetic data accelerates safe dev/QA.
- **New analytics leadership building foundations** = active reassessment of tooling, data quality, and test-data practices right now.
- Ongoing hiring across data engineering, analytics and governance = capacity is stretched (classic pain signal).

## Recent News
- **Jun 22, 2026** — Stephanie Lenzner named SVP of Value Intelligence to integrate analytics, data science and performance intelligence (reports to CDIO Onyeka Nchege).
- **Jul 1, 2026** — Reported milestone: 19,000+ team members actively using AI features embedded in the Epic EHR, framed around reducing clinician administrative burden/burnout.
- **Jun 1, 2026** — Acquisition of Community Hospital of Stokes (continued M&A-driven growth).
- **2025–2026** — Ongoing coverage (Forbes/CIO/HealthTech/Technology Magazine) of Novant's data + AI strategy under Nchege; goal of tripling in size / ~$30B revenue.

## Compliance Context
- **HIPAA / HITECH** govern all PHI — ICD-10-CM diagnoses, MS-DRG, encounters, demographics. The $6.6M pixel settlement shows Novant is a live target for privacy litigation and regulatory scrutiny around PHI handling.
- **Meta-pixel / web-tracking enforcement wave** (OCR guidance + class actions) makes any use of real patient data outside strict clinical need a liability.
- **De-identification (Safe Harbor / Expert Determination)** and synthetic data are the accepted paths to use realistic data in analytics, dev, testing and vendor demos without PHI exposure — directly matching RealityDB's us-healthcare pack (ICD-10-CM, MS-DRG, HIPAA-safe).
- As a multi-state NC/SC/VA system, also subject to state privacy/breach-notification regimes.

## Entry Point Recommendation
**Primary target: Stephanie Lenzner, SVP of Value Intelligence.** She is brand-new (June 2026), explicitly owns the integration of analytics + data science + "data foundation," and comes from a Chief Data & Analytics Officer background — she is actively shaping tooling and test-data practices and is the natural economic buyer for HIPAA-safe synthetic data. First-90-days leaders are unusually open to new vendors.

**Secondary / technical champion: the Manager or Director of Data Engineering** (see open reqs under Business Insights & Analytics) — the people who feel the pain of provisioning safe, realistic data for pipelines, QA and Epic/Cogito development.

**Executive sponsor / air-cover: Onyeka Nchege (EVP, CDIO)** — sets the "experimentation as a service" mandate and sits on the Truveta board, so he already believes in privacy-preserving data platforms.

**AI angle: Karen Hegarty (Head of AI & Innovation)** — for use cases needing safe training/eval data for AI models.

## Personalization Angles
1. **The $6.6M pixel settlement.** Frame RealityDB as the way to give analytics, dev and AI teams realistic ICD-10-CM / MS-DRG data with zero PHI — so the next "real data in the wrong environment" incident never happens. Concrete, board-level pain they already paid for.
2. **Lenzner's first-90-days "data foundation."** Congratulate her appointment and connect synthetic test data to the exact mandate she was hired for — integrating analytics/data science on a trustworthy foundation, while tripling in size and absorbing M&A (Stokes) without dragging PHI through every migration/QA cycle.
3. **Nchege's Truveta board seat + "experimentation as a service."** He already champions privacy-preserving clinical data at scale; RealityDB's HIPAA-safe synthetic data is the sandbox that lets teams experiment fast (Epic/Cogito, AI models) without waiting on de-identified data access or risking PHI.

## Contacts Found
| Name | Title | LinkedIn | Notes |
| --- | --- | --- | --- |
| Stephanie Lenzner | SVP, Value Intelligence (analytics, data science, performance intelligence) | https://www.linkedin.com/in/stephanie-lenzner-9031553/ | LIKELY MATCH — RocketReach + her posts tie this profile to "Mayo Clinic, Chair Digital/Data/AI Value," matching the Novant press release. Confirm the employer flip to Novant on view. PRIMARY / economic buyer. |
| Onyeka Nchege | EVP, Chief Digital & Information Officer | https://www.linkedin.com/in/onyeka-nchege/ | Executive sponsor. Owns analytics/AI/cyber. On Truveta board. 2024 Carolina ORBIE CIO of the Year. |
| Karen Hegarty, PhD | Head of AI & Innovation (Institute of Innovation & AI) | https://www.linkedin.com/in/karen-hegarty/ | AI use-case champion; ethical/safe AI focus. Good for AI training-data angle. |
| Keith Murphy, PhD | Data Scientist II | https://www.linkedin.com/in/keith-murphymph/ | Charlotte-based IC; potential technical validator. |
| Stephanie Fontanella | Director of Informatics Solutions | https://www.linkedin.com/in/stephanie-fontanella-66b37766/ | Informatics leadership (Greensboro area). |
| Sandip Ray | Senior Program Manager, Novant Health (Charlotte) | https://www.linkedin.com/in/sr72/ | VERIFIED profile (Novant, Charlotte, Auburn Univ). TITLE CORRECTED — Senior Program Manager (program/project mgmt, IT & change), NOT a data/analytics IC. Outreach framing likely no longer fits — re-target or drop. |

## Outreach Messages

_From Eddy Mkwambe personally (Charlotte founder, @realitydb/cli). Framing: HIPAA blocks production patient data. Relevant pack: us-healthcare (ICD-10-CM, MS-DRG, HIPAA-safe, 99/100 quality). Pain anchor for exec-level messages = the $6.6M Meta-pixel HIPAA settlement (~1.36M patients). Karen Hegarty framed around safe AI development data._

### Stephanie Lenzner — SVP, Value Intelligence (PRIMARY / economic buyer)

**LinkedIn connection request (<300 chars)**
> Stephanie — congrats on the Value Intelligence role. As you build Novant's data foundation, the $6.6M Meta-pixel settlement is the cautionary tale: real PHI in the wrong environment is expensive. I built RealityDB, a CLI for HIPAA-safe synthetic patient data. Would love to connect.

**LinkedIn DM follow-up (<150 words)**
> Stephanie — congratulations on the SVP, Value Intelligence appointment. You're building the data foundation for analytics and data science exactly as Novant triples in size and absorbs acquisitions like Stokes.
>
> The $6.6M Meta-pixel settlement already showed what real PHI in the wrong environment costs. RealityDB (@realitydb/cli) gives your teams realistic ICD-10-CM / MS-DRG patient data — 99/100 quality, deterministically seeded — so every migration, dashboard and QA cycle runs on production-shaped data with zero PHI.
>
> For a first-90-days leader setting tooling, it's a clean way to make "no real PHI in dev/test" the default from day one.
>
> Could I send a free Novant-relevant sample to try?
> — Eddy (Charlotte)

### Onyeka Nchege — EVP, Chief Digital & Information Officer (EXEC SPONSOR)

**LinkedIn connection request (<300 chars)**
> Onyeka — your "experimentation as a service" mandate and Truveta board seat say you already believe in privacy-preserving data at scale. After the $6.6M pixel settlement, synthetic data is the sandbox that keeps real PHI out of experiments. I built RealityDB for exactly that. Would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Onyeka — "experimentation as a service" only works if teams can experiment without dragging real PHI through every sandbox — and the $6.6M Meta-pixel settlement is the expensive proof of what happens when they do.
>
> RealityDB (@realitydb/cli) is that sandbox's data layer: HIPAA-safe synthetic patient data — ICD-10-CM, MS-DRG, realistic encounters — generated in one command at 99/100 quality. Your Truveta board seat already reflects the thesis; this is the same privacy-preserving idea for internal dev, QA and AI experimentation.
>
> Teams move fast on Epic/Cogito and AI models without waiting on de-identified-data access.
>
> Worth a 15-minute look with you or Stephanie's team?
> — Eddy (Charlotte)

### Karen Hegarty, PhD — Head of AI & Innovation (safe AI development data)

**LinkedIn connection request (<300 chars)**
> Karen — leading AI & Innovation with an ethical/safe-AI focus, you need training and eval data that never exposes real PHI. I built RealityDB, a CLI for HIPAA-safe synthetic patient data — ICD-10-CM, MS-DRG — built for exactly that. Charlotte founder — would love to connect.

**LinkedIn DM follow-up (<150 words)**
> Karen — safe, trustworthy AI starts with the data you develop and evaluate on, and real PHI in model-building environments is exactly the exposure the Institute exists to govern.
>
> RealityDB (@realitydb/cli) generates HIPAA-safe synthetic patient data — ICD-10-CM diagnoses, MS-DRG groupings, realistic encounters — deterministically seeded so AI experiments and evaluations are reproducible, at 99/100 quality. Teams prototype and validate models on production-shaped data with zero PHI, then move to governed real data only when truly needed.
>
> It's a clean fit for the ethical-AI posture the Institute vets use cases against.
>
> Could I send a free sample for an AI use case your team is exploring?
> — Eddy (Charlotte)

### Keith Murphy, PhD — Data Scientist II (technical validator)

**LinkedIn connection request (<300 chars)**
> Keith — as a data scientist at Novant, you're the one who needs realistic patient data to build and test models, and real PHI isn't an option in dev. I built RealityDB, a CLI that generates HIPAA-safe synthetic ICD-10-CM/MS-DRG data. Charlotte-based founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Keith — model work needs realistic, edge-case-rich patient data, and HIPAA keeps real PHI out of the environments where you actually build and test.
>
> RealityDB (@realitydb/cli) generates HIPAA-safe synthetic patient data in one command — ICD-10-CM, MS-DRG, realistic encounters and demographics — deterministically seeded so a model run or a failing test reproduces exactly. 99/100 quality, 303 passing tests.
>
> It's meant to drop straight into a notebook or pipeline so you can start day one without a PHI-access request.
>
> Happy to send you a free sample to try locally — want me to?
> — Eddy (Charlotte)

### Stephanie Fontanella — Director of Informatics Solutions

**LinkedIn connection request (<300 chars)**
> Stephanie — informatics solutions work constantly needs realistic patient data for build and test, and HIPAA keeps real PHI out of those environments. I built RealityDB, a CLI for HIPAA-safe synthetic ICD-10-CM/MS-DRG data. Would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Stephanie — informatics solutions live on realistic patient data, but HIPAA keeps real PHI out of the dev, test and demo environments where your team builds.
>
> RealityDB (@realitydb/cli) generates HIPAA-safe synthetic patient data — ICD-10-CM, MS-DRG, realistic encounters and demographics — in one command, 99/100 quality, deterministically seeded so builds and tests reproduce. It maps cleanly onto an Epic Cogito → warehouse → BI flow.
>
> Your team gets production-shaped data for prototyping and pipeline testing while PHI stays in production.
>
> Can I send a free Novant-relevant sample for your team to try?
> — Eddy (Charlotte)

### Sandip Ray — Healthcare Analytics, Charlotte

**LinkedIn connection request (<300 chars)**
> Sandip — healthcare analytics work needs realistic patient data to prototype dashboards and test pipelines, and real PHI can't go into those environments. I built RealityDB, a Charlotte-made CLI for HIPAA-safe synthetic ICD-10-CM/MS-DRG data. Would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Sandip — prototyping analytics and testing pipelines both need realistic patient data, and HIPAA keeps real PHI out of dev/test.
>
> RealityDB (@realitydb/cli) generates HIPAA-safe synthetic patient data — ICD-10-CM, MS-DRG, realistic encounters — in one command, 99/100 quality, deterministically seeded so dashboards and tests reproduce exactly.
>
> It gives you production-shaped data to build and demo against without waiting on PHI access or risking exposure.
>
> Both of us are Charlotte-based — happy to send a free sample tuned to a Novant use case. Want me to?
> — Eddy (Charlotte)

## Sources
- https://www.novanthealth.org/about/company/our-leadership/
- https://www.novanthealth.org/newsroom/novant-health-names-senior-vice-president-of-value-intelligence-to-strengthen-care-delivery
- https://www.beckershospitalreview.com/hospital-executive-moves/novant-health-appoints-value-intelligence-leader/
- https://www.forbes.com/sites/peterhigh/2025/05/30/using-data-and-ai-to-improve-outcomes-at-novant-health/
- https://www.cio.com/article/350281/novant-healths-angela-yochem-on-changing-the-cost-center-mindset.html
- https://www.novanthealth.org/about/our-commitment/institute-of-innovation--artificial-intelligence/
- https://www.hcinnovationgroup.com/analytics-ai/news/21084329/novant-health-launches-artificial-intelligence-institute
- https://distilinfo.com/2026/07/01/novant-health-deploys-ai-across-epic-ehr/
- https://www.hipaajournal.com/novant-health-pixel-privacy-breach-settlement/
- https://www.wral.com/story/nc-hospital-accused-of-sharing-private-data-settles-with-patients/21471784/
- https://www.novanthealth.org/newsroom/novant-health-reaches-preliminary-settlement-resolving-meta-pixel-class-action-claims
- https://en.wikipedia.org/wiki/Novant_Health
- https://www.levels.fyi/companies/novant-health/salaries/data-scientist
- https://www.linkedin.com/in/onyeka-nchege/
- https://www.linkedin.com/in/karen-hegarty/
- https://www.linkedin.com/in/keith-murphymph/
- https://www.linkedin.com/in/stephanie-fontanella-66b37766/
- https://www.linkedin.com/in/sr72/
