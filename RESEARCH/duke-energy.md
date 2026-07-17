# Duke Energy

## Overview
Duke Energy Corporation (NYSE: DUK) is one of the largest regulated electric
and gas utilities in the US. HQ: 525 South Tryon Street, Charlotte, NC 28202.
Serves ~8.4M electric customers across six states (NC, SC, FL, IN, OH, KY)
plus natural gas customers. Operates ~55 GW of generation and 11 nuclear
reactors. ~28,000 employees.

The company is in the middle of a massive capital program: a stated
$190–$200B investment over the next decade, with ~$95–$105B slated for
2026–2030, much of it driven by grid modernization and unprecedented load
growth from Southeast population increases and hyperscale AI data centers
(drawing up to ~1 GW per facility). This makes Duke a strong-timing target:
grid modernization + AI investment are top corporate priorities right now.

Data science and enterprise analytics are centralized at Duke's innovation
hub, Optimist Hall, in Charlotte — the same city as the RealityDB founder.

## Data Team Signals
- **Ben Zhang** leads Duke's company-wide data science program as VP of
  Enterprise Data Analytics. PhD in finance/econometrics; started at Cinergy
  (became Duke 2006). Built models spanning financial markets, meteorology,
  electric demand, and power plants. His team operates out of Optimist Hall,
  Charlotte.
- Named data science team members (from Duke's own "illumination" article):
  Masoud Sobhani, Charlotte Wang, Matthew Wiseman, Martin Cardenas.
- **iGrid** — a suite of forecasting/analytics products the team built to
  forecast and analyze electric demand, energy efficiency, rooftop solar, and
  EV adoption. Directly relevant to demand-forecasting synthetic data.
- **Revenue protection program** — uses data science on **smart meter data**
  to identify faulty meters and energy theft; saved $60M+ (2016–2018). This is
  literally smart-meter-reading analytics — RealityDB's proposed us-utility pack.
- Energy-efficiency program optimization saves ~$10M/yr via analytics.
- **Justin Brown** — Director, Grid Data & GIS (grid node / geospatial data
  ownership). **Aaron Smith** — Analytics Manager. **Todd Beaver** — Manager,
  DET (Data, Engineering & Technology) Analytics. All Charlotte-based.
- An enterprise-wide **Analytics Leadership Team** council exists to promote
  analytics in business decision-making.

## Technology Stack Signals
- **Cloud/data warehouse:** Snowflake and AWS Redshift referenced as Duke's
  cloud-native data warehousing stack; strategic gen-AI partnership with **AWS**
  (using generative AI to cut grid interconnection study times from weeks to
  minutes). Also partners with **GE Vernova**.
- ~1,400 business applications enterprise-wide; only 10–15% built in-house
  (heavy vendor/integration environment). Mix of on-prem and cloud data centers.
- **Smart meter data** is a core data asset — interview-prep material for Duke
  data roles centers on smart-meter reading tables with irregular timestamps
  and per-user hourly consumption calculations (confirms the data shape
  RealityDB's us-utility pack would synthesize).
- 50+ generative AI use cases in production across field ops, customer service,
  and internal IT. AI predictive modeling for meter anomaly detection since 2017.
- Data science languages/tools not fully public, but the program is
  model-heavy (forecasting, ML) — typical Python/SQL + Snowflake/Redshift.

## Pain Signals
- **Cannot freely use real customer energy-consumption data in development.**
  State laws and utility-commission rules require customer usage information be
  protected from disclosure (CPNI-adjacent privacy). Development/test teams
  need realistic smart-meter, outage, and customer-account data that is NOT
  real customer data. This is the exact gap RealityDB's custom us-utility pack
  fills.
- Massive grid-modernization build-out (2026–2030) means many new analytics
  and grid-software projects spinning up simultaneously — each needs test data.
- Smart-meter analytics (revenue protection, iGrid demand forecasting) depend
  on large, realistic meter-reading datasets that are privacy-encumbered in
  production.
- Heavy vendor/integration environment (85–90% of apps not in-house) = lots of
  integration/QA work where synthetic data de-risks handing data to vendors.
- CIO's stated principle "**Data before dazzle**" (quality data infrastructure
  must precede AI) — a direct hook: safe, high-quality synthetic data is a
  prerequisite for the AI programs they are funding.

## Recent News
- Oct 2025 (Forbes): CIO profile emphasizes AI/digital transformation; 50+
  gen-AI use cases; guardrails "Reliability first," "Data before dazzle,"
  "Human in the loop." Formalized gen-AI governance guardrails in 2024.
- 2025: Developed a standardized, repeatable data-center delivery design to
  meet AI-driven capacity demand.
- AWS generative-AI collaboration to slash grid interconnection study times.
- ~$9.88B invested in first nine months of 2025; $190–200B decade plan.
- DTECH 2026 conference session: "Revolutionizing our Grid Modernization
  Journey: Duke Energy's Journey Integrating AI."

## Compliance Context
- **NERC CIP** — Duke's bulk electric system is subject to NERC Critical
  Infrastructure Protection audits. Duke was fined $10M by NERC for 127
  security violations (2015–2018), so data-governance rigor is a live,
  board-level concern. Enterprise Cybersecurity Oversight Group (ECOG) now
  oversees AI governance.
- **Customer data privacy** — state laws and state utility commissions require
  certain customer information (including energy-usage data) be protected from
  disclosure. This is the CPNI-adjacent constraint that blocks use of real
  consumption data in dev/test/training.
- Framing: synthetic smart-meter/customer data lets Duke build and test
  analytics and AI without exposing regulated customer usage data or expanding
  the CIP/audit footprint of dev environments.

## Entry Point Recommendation
Primary target: **Ben Zhang, VP Enterprise Data Analytics** — he owns the
company-wide data science program (iGrid demand forecasting, smart-meter
revenue protection) that maps 1:1 to a custom us-utility pack (smart meter
readings, outage records, customer accounts, grid nodes, demand forecasting).
He is a model builder by background and will immediately grasp the value of
realistic-but-safe distributions.

Secondary: **Justin Brown, Director Grid Data & GIS** (grid-node/geospatial
data owner) and **Todd Beaver / Aaron Smith** (hands-on analytics managers who
feel the test-data pain day to day and can champion a $10–25K engagement).

Pitch the custom **us-utility pack consulting engagement** ($10,000–$25,000):
smart meter readings, outage records, customer accounts, grid nodes, and
demand-forecasting series — generated synthetically so no real customer usage
data touches development, testing, or AI training. Anchor on "Data before
dazzle" and NERC CIP / customer-privacy governance.

## Personalization Angles

### Ben Zhang (VP Enterprise Data Analytics)
- His revenue-protection program uses smart-meter data to catch faulty meters
  and theft — a RealityDB us-utility pack could generate labeled synthetic
  meter-anomaly/theft data for model development without touching real usage.
- iGrid forecasts demand, EE, rooftop solar, EV adoption — offer synthetic
  demand-forecasting datasets with realistic seasonality/weather correlation
  for pipeline and model testing.
- He is a quant/model builder — speak in distributions and data quality, not
  marketing.

### Justin Brown (Director, Grid Data & GIS)
- Owns grid data and GIS — the "grid nodes" component of the pack. Hook:
  synthetic grid-node/topology + outage records for testing grid analytics and
  GIS pipelines safely.

### Todd Beaver / Aaron Smith (Analytics Managers)
- Hands-on owners of analytics delivery who hit the "can't use real customer
  data in dev" wall. Hook: a fast, low-cost ($10–25K) synthetic dataset that
  unblocks their teams' development and QA immediately.

### Governance/CIO angle (Richard Donaldson / Bonnie Titone)
- Tie to "Data before dazzle" and the $10M NERC fine history: synthetic data
  shrinks the regulated-data footprint in dev/test and de-risks vendor handoffs
  across their 1,400-app, 85–90%-vendor environment.

## Contacts Found

| Name | Title | LinkedIn | Notes |
|------|-------|----------|-------|
| Ben Zhang | VP, Enterprise Data Analytics | VERIFY MANUALLY — multiple "Ben Zhang" profiles returned (linkedin.com/in/zhangben/ shows "Synergy Analytics Partners" which may be an outside/after role; also linkedin.com/in/ben-zhang-a8a2b2b4). Confirm the Duke Charlotte profile before outreach. | PRIMARY target. Owns company-wide data science (iGrid, smart-meter revenue protection). Optimist Hall, Charlotte. |
| Justin Brown | Director, Grid Data & GIS | https://www.linkedin.com/in/justin-brown-89890b28/ | Owns grid/GIS data = "grid nodes" pack component. Charlotte. Strong secondary. |
| Aaron Smith | Analytics Manager | https://www.linkedin.com/in/aaron-smith-5aa62090/ | Common name — VERIFY the Duke Charlotte profile. Hands-on champion. |
| Todd Beaver | Manager, DET Analytics | https://www.linkedin.com/in/todd-beaver-38222910/ | Charlotte Metro. Hands-on analytics delivery owner. |
| Bonnie Titone | SVP & CIO / EVP & Chief Administrative Officer | https://www.linkedin.com/in/bonnie-titone-ab26541 | Exec sponsor. Leads digital transformation + data optimization. Joined 2019 from PG&E. (Title may overlap/have shifted vs Donaldson — see note.) |
| Richard Donaldson | SVP & Chief Information Officer | VERIFY MANUALLY — no LinkedIn URL confirmed in search. | ~25 yrs at Duke; profiled Oct 2025 as CIO ~9 months in. Owns AI/digital strategy ("Data before dazzle"). Titone and Donaldson both surface as "CIO" — org structure likely shifted; confirm current titles. |
| Norv Clontz | VP, Data Strategy & Innovation (Duke); Analytics Leadership Team | VERIFY MANUALLY — https://www.linkedin.com/in/norvclontz/ ; one source indicates he may now be at E Source, not Duke. Confirm current employer. | Historically on Duke's Analytics Leadership Team council. |

Note: No single formal "Chief Data Officer" title found at Duke — data
leadership is split between Ben Zhang (analytics/data science) and the CIO org
(Donaldson/Titone). Ben Zhang is the functional data leader to target.

## Outreach Messages
To be drafted by message-drafter agent.

## Sources
- https://www.duke-energy.com/our-company/about-us/leadership
- https://illumination.duke-energy.com/articles/ben-zhang-and-team-use-data-science-for-a-cleaner-resilient-electric-grid
- https://www.forbes.com/sites/peterhigh/2025/10/22/duke-energys-cio-on-powering-digital-and-ai-transformation/
- https://www.linkedin.com/in/justin-brown-89890b28/
- https://www.linkedin.com/in/aaron-smith-5aa62090/
- https://www.linkedin.com/in/todd-beaver-38222910/
- https://www.linkedin.com/in/bonnie-titone-ab26541
- https://www.linkedin.com/in/norvclontz/
- https://www.duke-energy.com/our-company/about-us/leadership/bonnie-titone
- https://www.ainvest.com/news/duke-energy-grid-unsung-infrastructure-ai-curve-2602/
- https://www.distributech.com/2026-event-schedule/revolutionizing-our-grid-modernization-journey-duke-energys-journey-integrating-ai
- https://dataford.io/interview-guides/duke-energy/data-scientist
- https://www.utilitydive.com/news/duke-fined-10m-for-cybersecurity-lapses-since-2015/547528/
- https://www.duke-energy.com/legal/privacy-policy
- https://www.sec.gov/Archives/edgar/data/1326160/000110465926032452/tm2528215d2_ars.pdf
