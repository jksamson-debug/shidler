# FX Receivable Exposure & Hedging Strategy — EUR 4,500,000 Due July 31, 2026

**Created by:** Jersey Kianne Samson
**Updated by:** Jersey Kianne Samson
**Date Created:** April 4, 2026
**Date Updated:** April 4, 2026
**Version:** 1.0
**LLM Used:** Claude Sonnet 4.6

---

## Executive Summary (≤150 words)

Our firm expects to receive **EUR 4,500,000** from a European customer on **July 31, 2026**. At the current spot rate of 1.0820 USD/EUR, this receivable carries a USD equivalent of approximately **$4,869,000** — but that figure is unprotected. EUR/USD volatility over the next 119 days could reduce proceeds by $145,000 or more without any operational misstep on our part. This memo frames the exposure, quantifies the downside risk, and introduces three hedging families — forward contracts, FX put options, and zero-cost collars — as candidate strategies. We recommend authorizing a four-stage analysis (Stages 2–4) to model outcomes across rate scenarios, document the methodology, and deliver a formal hedge recommendation to this office before May 15, 2026.

---

## Background & Objectives

**Exposure Context**

The firm entered a euro-denominated sales contract with a European counterparty. Settlement of EUR 4,500,000 is due in a single payment on July 31, 2026. Because our functional currency is USD, the final dollar value of this receivable will be determined by the EUR/USD spot rate on the settlement date — a rate we cannot control.

**Why This Matters**

EUR/USD has exhibited annualized volatility of approximately 7–9% in recent years. Over a four-month horizon, a one-standard-deviation adverse move (~3–4%) implies a dollar shortfall of **$145,000–$195,000** relative to today's equivalent. A more pronounced euro depreciation — driven by ECB rate policy, U.S. dollar strengthening, or geopolitical disruption — could push that loss materially higher. Left unhedged, this exposure introduces budget variance, earnings risk, and cash flow uncertainty that management cannot absorb passively.

**Objectives**

1. Quantify the FX risk in dollar terms across bear, base, and bull rate scenarios.
2. Evaluate three hedging families on cost, certainty, and upside retention.
3. Select and implement a hedge strategy before the exposure window widens further.

---

## Methods

**Phase 1 — Exposure Identification (Complete)**

Confirmed notional (EUR 4,500,000), settlement date (July 31, 2026), and current spot reference (1.0820 USD/EUR). Established USD equivalent and volatility baseline using trailing 12-month EUR/USD data.

**Phase 2 — Excel Model (Stage 2)**

Build a working `.xlsx` prototype that computes and compares hedge outcomes across a scenario matrix. The model will include forward contract locked-rate analysis vs. spot at maturity, an FX put option payoff diagram across spot scenarios net of premium, zero-cost collar bounded outcome ranges with break-even analysis, and a scenario matrix spanning bear (−5%), base (0%), and bull (+5%) EUR/USD moves.

**Three Hedge Families Under Evaluation**

| Strategy | Mechanism | Pros | Cons |
|---|---|---|---|
| **Forward Contract** | Lock today's rate for July 31 delivery | Full certainty; no premium; simple to execute | Forgoes upside if EUR strengthens; requires bank credit line |
| **FX Put Option** | Right (not obligation) to sell EUR at a strike price | Downside protected; full upside preserved | Option premium (~1–2% of notional, est. $49K–$97K) |
| **Zero-Cost Collar** | Buy put, sell call to offset premium cost | Near-zero net cost; bounded downside | Caps upside gain; more complex to structure |

**Phase 3 — Technical Specification (Stage 3)**

Document model inputs, formulas, assumptions, and design decisions in a structured spec — precise enough for an AI or junior analyst to reconstruct or extend the tool independently.

**Phase 4 — Final Recommendation (Stage 4)**

Use model output to select the optimal strategy. Construct a structured AI prompt to stress-test the recommendation. Deliver a one-page executive summary with implementation instructions and counterparty execution steps.

---

## Limitations & Next Steps

**Known Constraints & Assumptions**

- The spot rate of 1.0820 USD/EUR is a reference point only; actual execution rate will differ at time of hedge placement.
- Option premium estimates (1–2% of notional) are indicative and subject to prevailing implied volatility at execution.
- Analysis assumes the EUR 4,500,000 receivable is certain; any counterparty credit risk or contract amendment would require hedge resizing.
- Forward availability and collar structures are contingent on existing bank credit facilities and ISDA agreement status.

**Immediate Next Steps**

| Action | Owner | Target Date |
|---|---|---|
| CFO approval to proceed with Stage 2–4 analysis | CFO | April 11, 2026 |
| Obtain indicative forward & option quotes from counterparties | Treasury | April 14, 2026 |
| Complete Excel hedge model (Stage 2) | Treasury / Finance | April 25, 2026 |
| Deliver technical specification (Stage 3) | Treasury / Finance | May 2, 2026 |
| Final recommendation memo to CFO (Stage 4) | Treasury | May 15, 2026 |

---

## References

- European Central Bank. (2026). *EUR/USD historical exchange rates*. Retrieved from https://www.ecb.europa.eu/stats/exchange/eurofxref
- CME Group. (2026). *EUR/USD futures and options product specifications*. Retrieved from https://www.cmegroup.com
- Garman, M. B., & Kohlhagen, S. W. (1983). Foreign currency option values. *Journal of International Money and Finance, 2*(3), 231–237.
- Hull, J. C. (2022). *Options, futures, and other derivatives* (11th ed.). Pearson.
