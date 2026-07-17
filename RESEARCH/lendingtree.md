# LendingTree

## Overview
LendingTree, Inc. (NASDAQ: TREE) is an online financial-services marketplace that connects consumers with lenders and insurers across mortgage, personal/auto/business loans, credit cards, and insurance. It is headquartered in Charlotte, NC (with a state-incented headquarters expansion in Mecklenburg County) and employs on the order of ~1,000+ people. The business is currently being driven by an insurance marketplace boom — Q1 2026 consolidated revenue hit a record $327.3M (+37% YoY), with Insurance revenue of $221.9M (+51% YoY) — which is generating enormous volumes of consumer and partner data flowing through their platform.

## Data Team Signals
- **Centralized analytics/strategy at the top.** Sarah Bacha (formerly Sarah Guidry) is SVP, Head of Analytics & Corporate Strategy (she has led the Analytics function since ~2021 and now owns Strategy, Analytics & AI, including a new "AI lab"). She sits on North Carolina's AI Advisory Council and is the company's public face on responsible AI.
- **Dedicated Data Engineering org.** Per The Org, the Data Engineering department lists ~17 members, led by **Darshit Parekh, Senior Director, Data Engineering** (at LendingTree since 2012; owns the company-wide data strategy, platform modernization, and a unified enterprise customer-intelligence / "single source of truth" integrating Marketing, Product, Sales, and Contact Center data).
- **Separate Data Science function.** **Samira Shaikh, Director, Data Science** (PhD, NLP/AI background, formerly UNC Charlotte faculty) leads data science; the team is actively hiring (Senior Data Scientist, Manager Data Science).
- **Structure looks hub + embedded partners.** Data teams "work with partners across Marketing, Product, Data Science, Analytics, Contact Center and Technology" — i.e., a central data-engineering/platform group serving embedded analytics consumers. This is exactly the topology where test/synthetic data and environment provisioning become a shared pain.

## Technology Stack Signals
- Job postings and Charlotte-market signals point to a **modern cloud data stack**: AWS, Snowflake, streaming pipelines, ETL/ELT, Python/SQL; Charlotte-area data-engineer roles broadly cite Airflow, Spark, dbt, Databricks, Docker/Kubernetes, Terraform. LendingTree is named among Charlotte companies hiring for Snowflake data engineers.
- Data Engineering roles emphasize **streaming data pipelines and cloud ETL** to feed analytics and data science.
- Heavy **MarTech / Customer Data Platform (CDP)** investment — Parekh's mandate centers on unifying customer data across channels for personalization and predictive decisioning.
- Emerging **AI/ML + GenAI** footprint (AI lab under Bacha; Director-level GenAI experience on the DS team).

## Pain Signals
- **Hiring = pain.** Multiple open Charlotte data roles right now — Senior Data Scientist ($130–170K), Manager Data Science, Data Engineer (streaming/ETL), Sr. Data Product Manager ($140–170K). Active build-out of data pipelines and ML means constant need for realistic, non-production test data.
- **Single-source-of-truth / CDP integration program.** Merging Marketing, Product, Sales, and Contact Center data into one customer-intelligence platform is a classic scenario where dev/test/QA environments need production-shaped-but-safe data — you can't seed a CDP or personalization model with real PII in lower environments.
- **AI/ML model development at scale.** Building and validating credit/insurance-matching and personalization models raises data-quality and model-risk exposure; regulated-lending model validation depends on well-formed, edge-case-rich data (rare/high-risk scenarios) that production data rarely supplies safely.
- **Consumer-financial PII everywhere.** As a marketplace, LendingTree ingests sensitive applicant data (income, SSNs, credit, insurance details). Using that in test/analytics environments is a privacy/compliance liability — a direct fit for synthetic banking/insurance data.

## Recent News
- **2026-07-06:** LendingTree publicly applauded Governor Josh Stein's North Carolina AI Strategic Roadmap and highlighted its own leadership in "responsible AI," via SVP Sarah Bacha's service on the state AI Advisory Council (focus on innovation + consumer protection). Strong signal they are actively branding around AI governance and responsible AI.
- **Q1 2026 (reported ~Apr 30, 2026):** Record quarterly revenue $327.3M (+37%); GAAP net income $17.3M ($1.22/diluted share); Adjusted EBITDA $42.0M (+71%). Insurance revenue $221.9M (+51%). Full-year guidance raised to $1.30–1.35B revenue and $152–162M adjusted EBITDA.
- **Ongoing:** State-incented headquarters expansion in Mecklenburg County (Charlotte).
- **Trade coverage** framed an "AI-driven transformation" thesis, citing real-time AML/KYC tooling and embedded compliance engines as part of LendingTree's AI governance posture.

## Compliance Context
- **Consumer financial data / privacy:** GLBA (Gramm-Leach-Bliley) safeguards on nonpublic personal financial information; FCRA (credit data); state privacy laws. Strong argument against using real applicant PII in non-production environments.
- **Fair lending / model governance:** ECOA and fair-lending scrutiny of any model influencing credit outcomes; regulators increasingly focus on AI/ML model risk, bias in training data, and lineage/documentation — where clean, controllable synthetic data with rare/edge cases improves validation.
- **Insurance regulation:** Insurance marketplace (now the revenue engine) adds state insurance-department data-handling and marketing-compliance requirements.
- **AML/KYC:** Public framing references AML/KYC tooling — a domain where synthetic scenario data is used to stress-test detection without exposing customer records.
- **State AI policy:** LendingTree is explicitly aligning with NC's AI Roadmap and "responsible AI," making privacy-preserving/synthetic data a narrative fit.

## Entry Point Recommendation
**Primary: Darshit Parekh, Senior Director, Data Engineering.** He owns the enterprise data platform, the CDP/single-source-of-truth program, and platform modernization — he is the budget-adjacent technical owner who feels test-data and environment-provisioning pain directly. Best first touch for a hands-on @realitydb/cli conversation.

**Secondary / air-cover: Sarah Bacha, SVP, Head of Analytics & Corporate Strategy (+ AI).** Executive sponsor for AI/analytics and the public voice on responsible AI — the right person for the privacy-preserving / responsible-AI framing and for top-down pull.

**Also worth a thread: Samira Shaikh, Director, Data Science** — she and her hiring team need realistic, edge-case-rich data for model development and validation.

## Personalization Angles
1. **Responsible-AI / NC AI Roadmap hook (for Bacha):** "Saw LendingTree championing NC's AI Strategic Roadmap and consumer-protection-first AI — synthetic banking/insurance data lets your teams build and validate models without ever putting real applicant PII into dev/test, which is exactly the 'responsible by design' posture you're advocating publicly."
2. **CDP / single-source-of-truth build (for Parekh):** "As you unify Marketing, Product, Sales, and Contact Center data into one customer-intelligence platform, lower environments need production-shaped data without the GLBA/FCRA exposure. @realitydb/cli generates realistic synthetic banking + insurance records so your pipelines and CDP integrations can be tested at volume, safely."
3. **Insurance-surge scale + hiring (for Parekh/Shaikh):** "With insurance revenue up 51% and a wave of new data-engineering/DS hires, the bottleneck is usually realistic test data to onboard people and validate models fast. We spin up synthetic insurance/lending datasets (including rare, high-risk edge cases for model validation) in one CLI command."

## Contacts Found
| Name | Title | LinkedIn | Notes |
|------|-------|----------|-------|
| Darshit Parekh | Senior Director, Data Engineering | https://www.linkedin.com/in/darshit-mukesh-parekh/ | PRIMARY entry point. At LendingTree since 2012; owns enterprise data strategy, CDP/single-source-of-truth, platform modernization. (Alt profile also seen: linkedin.com/in/darshit-parekh-8659a411/) |
| Sarah Bacha (née Guidry) | SVP, Head of Analytics & Corporate Strategy (Strategy, Analytics & AI) | https://www.linkedin.com/in/sarah-bacha-guidry-bb3a9b19/ | Executive sponsor / air-cover. Leads Analytics + AI lab; on NC AI Advisory Council; public voice on responsible AI. Charlotte-based. |
| Samira Shaikh | Director, Data Science | https://www.linkedin.com/in/drsamirashaikh/ | PhD, NLP/GenAI background, ex-UNC Charlotte faculty. Leads DS; team actively hiring. Good technical champion for model-validation angle. |
| Brian Holbrook | Senior Manager, Revenue Analytics (listed under Data Engineering org) | VERIFY MANUALLY | Role confirmed (The Org, ZoomInfo), but the two "Brian Holbrook" LinkedIn profiles found are different people — no LendingTree match. |
| Owais Ahmed | Principal / Lead Data Engineer | VERIFY MANUALLY | Role confirmed on The Org, but no LinkedIn profile disambiguates to LendingTree/Charlotte. |
| Luis Lema | Staff Data Engineer | https://www.linkedin.com/in/llema/ | VERIFIED — profile shows LendingTree; corroborated by AeroLeads (Staff Data Engineer) and The Org. |

## Outreach Messages

_From Eddy Mkwambe personally (Charlotte founder, @realitydb/cli). Framing: LendingTree is a fintech/lending marketplace — pain is mortgage lead data, credit-scoring pipelines, and conversion analytics, not wires/SEPA. Relevant packs: us-banking (loan data, credit scores, FICO distributions) + fintech._

### Darshit Parekh — Senior Director, Data Engineering (PRIMARY)

**LinkedIn connection request (265 chars)**
> Darshit — you own LendingTree's data platform and the CDP/single-source-of-truth build. Seeding lower environments with real applicant PII is a GLBA/FCRA headache. RealityDB, my CLI for synthetic lending data, fixes that. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Darshit — unifying four channels into one customer-intelligence platform means your dev/test/QA environments need production-shaped data, and real applicant records (income, SSNs, credit) can't safely go there.
>
> RealityDB (@realitydb/cli) generates synthetic lending/credit datasets — MOD-10-valid ABA routing, realistic FICO and income/DTI distributions, plus rare high-risk edge cases production data rarely surfaces — in one command. 99/100 quality, deterministic seeding so tests reproduce exactly.
>
> Happy to generate a free sample shaped to a LendingTree pipeline you're building — mortgage or personal-loan applications, your call — so you can drop it straight into a lower environment.
>
> Worth 15 minutes to see if it fits?
> — Eddy (Charlotte)

### Sarah Bacha — SVP, Head of Analytics & Corporate Strategy (+ AI) (AIR COVER)

**LinkedIn connection request (294 chars)**
> Sarah — saw LendingTree championing NC's AI Strategic Roadmap and consumer-protection-first AI via your Advisory Council seat. Synthetic data lets teams build and validate models without real applicant PII in dev/test — responsible by design. RealityDB does exactly this. Would love to connect.

**LinkedIn DM follow-up (<150 words)**
> Sarah — your public stance on responsible, consumer-protection-first AI (and the NC AI Roadmap work) is the exact posture I built RealityDB around.
>
> Every model your AI lab and DS team build gets safer if real applicant PII never touches dev/test. RealityDB (@realitydb/cli) generates synthetic banking/insurance data — realistic FICO, income, credit and insurance distributions, with rare high-risk edge cases that make model validation and fair-lending testing stronger — all GLBA-safe and reproducible.
>
> It's the "responsible by design" data layer underneath the AI governance you're already advocating.
>
> Could I send your team a free LendingTree-relevant sample to try in a lower environment?
> — Eddy (Charlotte)

### Samira Shaikh — Director, Data Science

**LinkedIn connection request (300 chars)**
> Samira — as your DS team scales and validates credit/insurance-matching models, the bottleneck is realistic, edge-case-rich data you can't pull from production. RealityDB, my CLI for synthetic lending/insurance data with controllable rare cases, solves it. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Samira — building and validating credit- and insurance-matching models is only as good as the edge cases in your data, and production rarely surfaces the rare/high-risk scenarios safely.
>
> RealityDB (@realitydb/cli) generates synthetic lending/insurance datasets with deliberately controllable distributions — FICO, income/DTI, fraud and high-risk edge cases — deterministically seeded so model tests reproduce, and free of the GLBA/FCRA exposure of real applicant PII.
>
> For a team that's actively hiring, it also means new data scientists start on realistic data day one, no prod-data wait.
>
> I'd love to generate a free sample tuned to one of your model-validation use cases. Open to a quick look?
> — Eddy (Charlotte)

### Brian Holbrook — Senior Manager, Revenue Analytics

**LinkedIn connection request (293 chars)**
> Brian — revenue analytics at LendingTree runs on conversion and lead-quality data that's hard to prototype against without touching real applicant records. RealityDB, a CLI that generates realistic synthetic lending/conversion data for exactly that. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Brian — prototyping revenue and conversion analytics usually means either waiting on prod-data access or risking real applicant PII in a dashboard sandbox.
>
> RealityDB (@realitydb/cli) generates production-shaped synthetic lending data — applications, FICO/income distributions, conversion-relevant fields — in one CLI command, deterministically seeded so your dashboards and tests reproduce. No GLBA/FCRA exposure.
>
> It's a fast way to build and demo revenue-analytics views before real data is wired in.
>
> Can I send you a free sample shaped to a LendingTree conversion funnel to try?
> — Eddy (Charlotte)

### Owais Ahmed — Principal / Lead Data Engineer

**LinkedIn connection request (<300 chars)**
> Owais — as a hands-on owner of LendingTree's pipelines, you feel the test-data problem daily: you can't seed lower environments with real applicant PII. I built RealityDB, a CLI that generates realistic synthetic lending data at volume. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Owais — pipeline work lives or dies on test data, and real applicant records (income, SSNs, credit) can't go into dev/test/QA without GLBA/FCRA headaches.
>
> RealityDB (@realitydb/cli) generates synthetic lending/credit datasets at volume from one command — MOD-10-valid ABA routing, realistic FICO/income/DTI, rare high-risk edge cases — deterministically seeded so pipeline tests reproduce. 99/100 quality, 303 passing tests.
>
> It drops straight into Snowflake/streaming ETL, no prod-data request needed.
>
> Happy to generate a free sample matched to one of your pipelines. Worth a look?
> — Eddy (Charlotte)

### Luis Lema — Staff Data Engineer

**LinkedIn connection request (<300 chars)**
> Luis — staff-level pipeline work means constantly needing realistic data for dev/test that can't be real applicant PII. I built RealityDB, a CLI that generates synthetic lending/credit data at volume, deterministically seeded. Charlotte founder — would value connecting.

**LinkedIn DM follow-up (<150 words)**
> Luis — as a staff engineer you're the one who ends up needing production-shaped data for pipeline dev, QA and reproducing bugs — and real applicant PII isn't an option in lower environments.
>
> RealityDB (@realitydb/cli) generates synthetic lending/credit datasets in one command — valid ABA routing, realistic FICO/income distributions, rare edge cases — deterministically seeded so a failing test reproduces exactly. 99/100 quality score.
>
> It loads straight into Snowflake or your streaming ETL, no prod-data request.
>
> Can I send you a free sample shaped to a LendingTree pipeline to try locally?
> — Eddy (Charlotte)

## Sources
- LendingTree Investor Relations — https://investors.lendingtree.com/
- NC Commerce, HQ expansion in Mecklenburg County — https://www.commerce.nc.gov/news/press-releases/lendingtree-expands-headquarters-operations-mecklenburg-county
- LendingTree applauds NC AI Strategic Roadmap (2026-07-06) — https://www.sahmcapital.com/news/content/lendingtree-applauds-north-carolinas-ai-strategic-roadmap-highlights-companys-leadership-in-shaping-responsible-ai-policy-2026-07-06
- StockTitan — LendingTree / NC AI roadmap — https://www.stocktitan.net/news/TREE/lending-tree-applauds-north-carolina-s-ai-strategic-roadmap-b3a40empmpe5.html
- Sarah Bacha executive bio — https://press.lendingtree.com/about/our-executives/bio/sarahbacha
- Sarah Bacha (Guidry) LinkedIn — https://www.linkedin.com/in/sarah-bacha-guidry-bb3a9b19/
- The Org — LendingTree Data Engineering team roster — https://theorg.com/org/lendingtree/teams/data-engineering
- The Org — Darshit Parekh — https://theorg.com/org/lendingtree/org-chart/darshit-parekh
- Darshit Parekh LinkedIn — https://www.linkedin.com/in/darshit-mukesh-parekh/
- Samira Shaikh LinkedIn — https://www.linkedin.com/in/drsamirashaikh/
- Samira Shaikh — UNC Charlotte School of Data Science — https://sds.charlotte.edu/directory/samira-shaikh/
- LendingTree Careers (jobs) — https://www.lendingtree.com/careers/jobs/
- LendingTree Careers — Charlotte — https://www.lendingtree.com/careers/locations/charlotte/
- Greenhouse job board (LendingTree) — https://job-boards.greenhouse.io/lendingtree/jobs/6161624
- LendingTree Q1 2026 results (PRNewswire) — https://www.prnewswire.com/news-releases/lendingtree-reports-first-quarter-2026-results-302759400.html
- LendingTree Q1 2026 8-K (SEC) — https://www.sec.gov/Archives/edgar/data/0001434621/000162828026028909/tree-33126xer.htm
- ChartMill — TREE Q1 2026 earnings — https://www.chartmill.com/news/TREE/Chartmill-46618-LendingTree-Inc-NASDAQTREE-Q1-2026-Earnings-Meet-Revenue-Estimates-Beat-EPS-But-Stock-Falls-52
- AInvest — LendingTree AI-driven transformation (AML/KYC, compliance engines) — https://www.ainvest.com/news/lendingtree-ai-driven-transformation-catalyst-sustained-double-digit-growth-financial-services-2508/
