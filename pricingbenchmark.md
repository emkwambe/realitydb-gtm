# Synthetic Data Pricing Benchmark & RealityDB Repricing Recommendation

_Compiled 2026-07-16. Sources are vendor pricing pages, data
marketplaces, and 2025–2026 pricing analyses (linked at end). Figures
are public list prices or published ranges; enterprise pricing is
mostly gated ("contact sales") and shown as ranges from third-party
analyses._

---

## TL;DR — the three things that matter

1. **RealityDB's headline self-serve prices ($49–$499 one-time) sit in
   "toy-data" territory**, right next to Mockaroo (generic random data,
   $50–$500 **per year**). For 100% referential integrity, temporally
   ordered, government-sourced statistical distributions (FDIC, CMS,
   FFIEC, NAIC), compliance-framed banking/healthcare data, that anchors
   the product as a cheap utility instead of a production-grade
   compliance asset. **The market prices compliant finance/healthcare
   synthetic data at enterprise levels** ($20K–$250K+ for high-fidelity
   custom).
2. **There is a canyon in the lineup**: nothing between the $499
   self-serve ceiling and the $25K consulting floor. That mid-market
   ($1.5K–$10K) is exactly where teams buy, and RealityDB has no product
   there.
3. **Selling by raw row count invites commoditization.** Competitors
   sell by *pack, seat, license, and compliance value* and hide
   enterprise pricing behind "contact sales." RealityDB should do the
   same — keep the row-count entry wedge, but reframe tiers around value.

---

## A. Market pricing landscape

| Vendor | What they sell | Pricing model | Concrete prices | Domain focus |
|--------|----------------|---------------|-----------------|--------------|
| **Mockaroo** | Generic mock/random datasets (self-serve) | Annual, by max rows/dataset | Free 1K rows · Silver **$50/yr** = 100K rows · Gold **$500/yr** = 10M rows | Generic (no compliance, no FK guarantees) |
| **YData** | Generation SDK/platform | Usage — data volume | **$1 per 1M data points** (cells); 1 credit = 10K tokens | Tabular/generic |
| **Tonic.ai** | Dev/test synthetic data platform | Subscription + usage (source DB size) | Free ($10/mo credits) · **~$199/mo** floor · Enterprise "contact sales" (signs BAA/DPA) | Dev/test, some regulated |
| **Gretel (now NVIDIA)** | Generation platform | Credits | Legacy: 15 free credits (~100K records) · **$2/credit** · Team **$295/mo**. Now folded into NVIDIA NeMo — **sales-gated** | Generic + regulated |
| **Mostly AI** | Generation platform | Credits (1 credit = 1M data points) | Free 5 credits/day · Team **$3/credit** · Enterprise **$5/credit (~$3,000/mo)** | Banking/insurance/health |
| **Hazy** | Enterprise synthetic data | Subscription | **~$500/mo** floor (enterprise deals higher) | Financial services |
| **Rendered.ai / Synthesis AI** | Image/CV synthetic data | Subscription | **$3,000–$15,000/mo** | Vision (infra-heavy) |
| **Syntegra** | Synthetic patient-level EHR data | License (quote) | Enterprise license; real patient-level data "hundreds of thousands+"; synthetic positioned as cheaper, still enterprise | Healthcare EHR |
| **MDClone** | Synthetic data engine (from real EHR) | Enterprise contract (quote) | Sales-gated, health-system scale | Healthcare |
| **AWS Data Exchange / marketplaces** | Third-party datasets | Subscription 1–36 mo | **Free → hundreds of thousands**; provider pays 3% listing fee | Finance, healthcare, all |
| **GenRocket** | Test-data generation | Enterprise subscription | Quote-based | Test data |

---

## B. Per-row / per-dataset benchmark

Two very different worlds — do not average them:

**Generic self-serve (the "toy" floor) — sets the *lower* bound only:**
- Mockaroo Gold: 10M rows / $500 per year ≈ **$0.00005/row/yr** (generic).
- YData metered: $1 / 1M data points ≈ **$0.0000001/cell** (pure compute).
- These are cheap because they carry **no compliance, no calibrated
  distributions, no referential-integrity guarantee**.

**Compliant / production-grade (the tier RealityDB actually competes in):**
- No public per-row price exists — it is sold as **platform
  subscription ($199–$3,000+/mo)** or **custom project ($10K–$250K+)**.
- Ultra-high-fidelity **healthcare/finance custom "may exceed $250,000"**.
- The per-row number is deliberately hidden; buyers pay for **fidelity,
  privacy guarantee, and compliance**, not rows.

**RealityDB's current self-serve per-row (for reference):**
| Tier | Price | Rows | $/row |
|------|-------|------|-------|
| Starter | $49 | 50K | $0.00098 |
| 100K | $79 | 100K | $0.00079 |
| 500K | $299 | 500K | $0.000598 |
| 1M | $499 | 1M | $0.000499 |

→ RealityDB's finished, compliant dataset is priced **~10–20× above
generic Mockaroo per row** (good — quality premium is real) but **1–2
orders of magnitude BELOW the compliant-platform world** it actually
belongs in.

---

## C. Domain premium — finance & healthcare (evidence)

- **Compliant finance/healthcare is the top pricing tier, everywhere.**
  Ultra-high-fidelity synthetic data in these domains "may exceed
  $250,000" per project; high-fidelity generally $20K–$100K+.
- **Privacy/compliance guarantees add a documented 30–50% premium** over
  basic generation.
- **Real patient/claims data costs "hundreds of thousands of dollars";**
  synthetic is sold as the cheaper-but-still-enterprise alternative
  (Syntegra, MDClone) — i.e., the anchor is a six-figure real-data cost,
  not a $50 mock dataset.
- Regulated-domain vendors **sign BAAs/DPAs** and gate pricing behind
  sales — both are signals that say "production-grade, not a utility."

**Implication for RealityDB:** us-banking and us-healthcare packs are
the premium SKUs. They should be priced and framed *up*, against the
six-figure real-data / custom-project anchor — not against Mockaroo.

---

## D. Off-the-shelf vs custom vs generation-access

| Motion | Market pricing pattern |
|--------|------------------------|
| **Off-the-shelf dataset** | Marketplace one-off or cheap annual (generic: $50–$500/yr). Compliant ready-made is rare — RealityDB's actual white space. |
| **Generation access (platform)** | Subscription floor ($199–$500/mo entry; $3K–$15K/mo enterprise) + usage meter (credits/compute/volume) + annual on-prem license ($80K–$250K/yr). |
| **Custom / bespoke** | Project-based: PoC $10K–$30K · tabular build $10K–$40K · high-fidelity $20K–$100K+ · enterprise implementation $175K–$350K. Priced by **complexity/fidelity**, not rows. Privacy premium +30–50%. |

Annual billing conventionally saves **15–25%**. "Cost per data point
cannot explain actual market pricing" — the market is **value-based**.

---

## E. Assessment of RealityDB's current pricing

**Where it under-prices (money left on the table):**
- **Self-serve ceiling far too low.** $499 for 1M rows of 99/100
  compliant banking data competes on headline with a $500/yr generic
  toy. The compliant tier supports **10–50× more**.
- **Team plan undercuts every entry competitor.** $99/mo (or $990/yr =
  $82.50/mo) is below Tonic ($199), Gretel ($295), Hazy ($500).
- **Custom per-row is low.** $0.001–$0.007/row with a $95 minimum. Market
  custom tabular starts at $10K projects; compliant work carries a
  30–50% privacy premium. The $95 floor signals "hobby."

**Inconsistencies / confusion risks:**
- **Per-row overlap.** Self-serve tops out at ~$0.0005/row (1M tier),
  which is **cheaper per row than the custom "Simple" $0.001/row**. A
  buyer comparing the store to the custom quote sees the bespoke option
  costing *more per row than the finished one* at low volumes but the
  finished 1M dataset costing *less per row than the custom minimum* —
  confusing math either way.
- **Selling by rows commoditizes.** It invites a direct
  apples-to-oranges comparison with Mockaroo's row counts and erases the
  compliance story.
- **The $499 → $25K canyon.** No mid-market offer for a team that wants
  more than a dataset but isn't buying a $25K–$85K engagement.

---

## F. Repricing recommendation

Principle: **keep a cheap entry wedge for adoption, reframe tiers around
value not rows, raise the ceiling, and add an "Enterprise: contact us"
anchor** (the universal production-grade signal). Keep the *visible*
menu to ~3 tiers + Enterprise so buyers aren't confused.

### 1. Self-serve store — reframe by pack, not raw rows
| Tier | Suggested price | What it is |
|------|-----------------|-----------|
| **Sample** | **Free** | 5–10K-row sample of any pack (the wedge — keep generous) |
| **Single Dataset** | **$99** (from $49) | One pack, up to 100K rows, one project |
| **Pack License** | **$1,500–$2,500 / yr** | One domain pack, unlimited internal use + regen, 1 seat-team |
| **Multi-Pack / Team** | **$6,000–$9,000 / yr** | All US packs, up to ~5 seats, annual regeneration |
| **Enterprise** | **Contact us** | SSO, BAA/DPA, custom volumes, watermark attestation |

Rationale: the **Pack License** and **Multi-Pack** tiers fill the $499→$25K
canyon and match entry/mid platform subscriptions ($199–$500/mo ≈
$2.4K–$6K/yr) — but as a *finished compliant asset*, which nobody else
sells off-the-shelf. Row caps stay as fair-use guardrails, not the
headline metric.

### 2. Custom datasets — raise floor, add a regulated tier
- Keep per-row for small jobs but **raise the minimum from $95 → $500**.
- Tiers: Simple **$0.002/row**, Moderate **$0.005/row**, Complex
  **$0.010/row** (up from 0.001/0.003/0.007).
- Add **Regulated/Compliant tier: +40% premium** (market supports
  30–50% for privacy/compliance guarantees) — applies to banking,
  healthcare, insurance builds.
- Reframe larger custom work as **project-based**, not per-row: a
  "Compliant Dataset Build" starting at **$5,000** (aligns with market
  $10K–$40K tabular projects while staying founder-accessible).
- Keep Express +50% / Rush +150% — consistent with market urgency
  premiums.

### 3. Subscription
- Raise team monthly to **$199/mo** (market entry floor) with **annual
  at ~$1,990/yr** (≈16% off — within the 15–25% norm).

### 4. Consulting anchors (already well-placed — make them visible)
- AI Readiness Audit **$25K–$35K** and Synthetic Sandbox MVP **$45K–$85K**
  are on-market vs custom-implementation ranges ($15K–$100K; enterprise
  $175K–$350K). **Show these publicly as the top anchor** — they make the
  $1.5K–$9K licenses look like the easy, obvious buy (price anchoring).

### 5. Positioning rules (avoid devaluing / confusing)
- **Lead with the anchor, not the floor.** Reference the six-figure cost
  of real/regulated data and $250K+ custom builds; position RealityDB as
  the compliant shortcut.
- **Sell the guarantee, not the rows** — 100% referential integrity,
  temporally ordered, deterministic seeding, Ed25519 watermarking,
  government-sourced statistical distributions (FDIC, CMS, FFIEC, NAIC).
  These are the "production-grade"
  signals that separate you from toy generators.
- **Gate enterprise behind "contact us"** — every premium/compliant
  vendor does; a public $499 ceiling actively signals "not enterprise."
- **One clean menu.** 3 visible tiers + Enterprise. Move the full per-row
  matrix to the consulting page so the store stays simple.
- **Annual-first** with the 15–25% discount to lift LTV and match norms.

---

## Sources
- Mockaroo pricing — https://www.mockaroo.com/pricing
- Tonic.ai pricing — https://www.tonic.ai/pricing
- Mostly AI pricing tiers — https://opentools.ai/news/mostly-ais-new-pricing-tiers-what-you-need-to-know
- Gretel/NVIDIA pricing history — https://www.g2.com/products/gretel-ai/pricing ; https://aichief.com/ai-development-tools/gretel-ai/
- 2025 Global Synthetic Data Pricing Strategy Analysis (Pebblous) — https://blog.pebblous.ai/project/SyntheticData/synthetic-data-pricing/en/
- Synthetic data generation pricing (Monetizely) — https://www.getmonetizely.com/articles/what-is-synthetic-data-generation-pricing-for-privacy-compliant-analytics
- Syntegra synthetic EHR (Datarade) — https://datarade.ai/data-products/syntegra-synthetic-ehr-data-structured-healthcare-electroni-syntegra
- MDClone synthetic data — https://www.mdclone.com/synthetic-data
- AWS Data Exchange pricing — https://aws.amazon.com/data-exchange/pricing/
- Synthetic data in healthcare market — https://dataintelo.com/report/synthetic-data-in-healthcare-market

_Note: Gretel (NVIDIA), Tonic enterprise, Mostly AI enterprise, MDClone,
and Syntegra all gate real numbers behind "contact sales" — public
figures above are entry tiers or third-party estimates and should be
treated as directional, not exact quotes._
