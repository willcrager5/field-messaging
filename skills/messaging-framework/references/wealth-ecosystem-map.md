# Wealth Ecosystem Map — Field's Position in the Terrain

**Author:** Will (strawman for Bill's review)
**Status:** Working draft. Nothing is locked. Reacts welcome.
**Purpose:** A terrain map, not a battlecard. For the Field Brand Strategist to reason against the full wealth stack — not just Field's internal story — whenever positioning, competitive, or segment work comes up.

---

## How to read this

Each layer of the wealth stack has its own players, its own job, and its own relationship to Field. Field is not a player inside any single layer. Field's strategic claim is the *intelligence layer* that sits above data-producing systems and cross-cuts to the demand side. So every relationship below is framed from that vantage: Field as connective tissue, not as a competitor inside a vertical.

**Relationship vocabulary** (used in the table and narrative):
- **Consumer** — Field ingests data from this layer
- **Enricher** — Field makes this layer's data more useful in context
- **Neutral coexist** — Field operates alongside, different job
- **Partner** — Field integrates; both benefit from the relationship
- **Demand-side customer** — this layer pays Field for something (the network side)
- **Builder / infrastructure customer** — this layer builds products on Field/Bridge infrastructure
- **Adjacent** — overlaps sometimes, different primary job
- **Competitive** — direct overlap in claim (rare for Field)
- **Substitutable** — customers may perceive as an alternative to Field (address in positioning)

---

## Quick reference — the layers

| # | Layer | Representative players | Field's relationship | One-line positioning rule |
|---|---|---|---|---|
| 1 | Custody | Schwab, Fidelity, Pershing, BNY | Consumer (via BridgeFT) | "Field connects to where your accounts actually live — not a replacement, a layer above." |
| 2 | Portfolio accounting / performance | Orion, Black Diamond, Tamarac, Addepar | Consumer + neutral coexist | "Field sits above your performance reporting and makes it firm-level intelligence." |
| 3 | CRM | Salesforce FSC, Wealthbox, Redtail, Practifi | Consumer + enricher | "Your CRM captures activity. Field turns activity and accounts into business intelligence." |
| 4 | Financial planning | eMoney, MoneyGuide Pro, RightCapital | Consumer + enricher | "Field pulls goal and plan data into the same view as portfolio and client signal." |
| 5 | Research / content / market data | Morningstar, FactSet, YCharts | Neutral coexist | "Different job — those tools tell the market story; Field tells the firm story." |
| 6 | Risk analytics | Nitrogen (fka Riskalyze), HiddenLevers | Neutral coexist / adjacent | "Field reads risk signals across the book; risk tools quantify per portfolio." |
| 7 | Compliance / archiving | Smarsh, Hearsay, MyRepChat | Neutral coexist | "Field provides the audit trail across client and account data; compliance tools cover comms." |
| 8 | Data aggregation / plumbing | Plaid, Yodlee, ByAllAccounts, MX | Adjacent (advisor-side, not consumer-side) | "Field is advisor-owned intelligence, not consumer-permissioned pipes." |
| 9 | Asset managers (mega / alts) | **BlackRock, Blackstone, Nuveen, PIMCO, Apollo** | **Demand-side customer** | "The distribution intelligence layer for the modern asset manager." |
| 10 | TAMPs | Envestnet, SEI, AssetMark | Partner or adjacent (segment-dependent) | "Different economic model. Field gives RIAs intelligence regardless of investment platform." |
| 11 | Broker-dealers / aggregators | LPL, Commonwealth, Raymond James | Adjacent (segment-dependent) | "Field serves RIAs; where BDs own the advisor relationship, Field is a platform decision they make." |
| 12 | Wealthtech / fintech builders | Income Lab, ZOE Financial, ALLINDEX, new builders | **Builder / infrastructure customer** (BridgeFT's ICP) | "The infrastructure layer for the next generation of wealth products." |
| 13 | Robo / digital advice | Betterment, Wealthfront, SigFig | Adjacent / not ICP | "Different end customer. Field is for advisor-led firms." |

---

## Layer-by-layer narrative

### 1. Custody — Schwab, Fidelity, Pershing, BNY

The system of record for advisor-held assets. Custodians own account, position, and transaction data. They are the trusted backbone of the industry. Field is a **consumer** of custodial data via BridgeFT's multi-custodial API — the most mature and trusted consumer, thanks to the acquisition. Field is not a custodian, does not aspire to be, and should never position as one.

*Positioning rule:* Field connects to where your accounts actually live. We don't replace the custodian — we make their data legible at the firm level.

### 2. Portfolio accounting / performance — Orion, Black Diamond, Tamarac, Addepar

The firms that turn custodial feeds into performance reporting, billing, and reconciled books. Large RIAs live inside these systems for day-to-day operations. Field **consumes** their output where firms already run them, or ingests custodial data directly where firms don't. Field **neutrally coexists** — different job. Portfolio accounting is about account-level truth; Field is about firm-level intelligence.

Addepar is the closest analog in ambition but solves for UHNW reporting depth, not firm-level business intelligence or distribution network economics. Respect them publicly; position differently.

*Positioning rule:* Your performance reporting tells you what happened in an account. Field tells you what's happening in your firm.

### 3. CRM — Salesforce FSC, Wealthbox, Redtail, Practifi

The system of record for client relationships and activity. Field **consumes and enriches** — CRM captures activity; Field combines activity with account, plan, and portfolio data to produce something CRM alone can't: business intelligence about the firm's book. Tight integration is table stakes.

*Positioning rule:* Your CRM captures activity. Field turns activity and accounts into business intelligence.

### 4. Financial planning — eMoney, MoneyGuide Pro, RightCapital

Goal data and plan data lives here. Field **consumes and enriches** — pulling plan data into the firm-level view so goals, plans, and portfolio action can be seen together. Not a competitor.

*Positioning rule:* Field pulls plan data into the same view as portfolio and client signal. One picture, not four tabs.

### 5. Research / content / market data — Morningstar, FactSet, YCharts

Outbound market content used to tell investment stories. **Neutral coexist** — completely different job. Research tools tell the *market* story (how is this fund performing, what's the fixed income outlook); Field tells the *firm* story (what's happening in your book, your clients, your growth).

Don't anchor competitive positioning on this layer. Advisors use both. The two don't overlap enough to fight about.

*Positioning rule:* Those tools tell the market story. Field tells the firm story.

### 6. Risk analytics — Nitrogen (formerly Riskalyze), HiddenLevers

Risk scoring at the portfolio level. **Neutral coexist** with an adjacent edge — Field reads risk signals across the book and over time; risk tools quantify per-portfolio at a moment. If anything, integration is value-additive.

*Positioning rule:* Field reads risk signals across the book. Risk tools quantify per portfolio. Both are useful.

### 7. Compliance / archiving — Smarsh, Hearsay, MyRepChat

Communications archiving, supervision, regulatory compliance. **Neutral coexist** — Field provides audit trails across client and account data; these tools cover the comms layer. Can integrate, doesn't compete.

*Positioning rule:* Field provides the audit trail across client and account data. Compliance tools cover the conversations.

### 8. Data aggregation / plumbing — Plaid, Yodlee, ByAllAccounts, MX

Consumer-side or institutional plumbing for account aggregation. **Adjacent, not comparable.** Plaid and Yodlee are consumer-permissioned — the end customer connects their accounts. Field is advisor-owned and governed by the RIA relationship. Different permission model, different data economics, different governance story.

This distinction matters when the data-rights conversation comes up. *We are not Plaid.*

*Positioning rule:* Field is advisor-owned intelligence, not consumer-permissioned pipes.

### 9. Asset managers (mega / alts) — **BlackRock, Blackstone, Nuveen, PIMCO, Apollo**

The **demand-side customer** of the Field network. These firms have massive wholesaling operations trying to reach the RIA channel with the right product at the right moment — and the current motion (cold calls, conferences, generic content campaigns) is expensive and low-signal. Field's network side is the distribution intelligence layer: anonymized, opted-in, governed signal from the RIA base that lets AMs target the right firms at the right time. The "Digital Wholesaler" idea was already in BridgeFT's product — Field extends and scales it.

At this stage Field is pursuing mega asset managers and alts, not boutique AMs. That's the tier with the wholesaling budgets, the need for channel intelligence, and the willingness to pay for scaled data access. Messaging for this audience is enterprise-grade, data-serious, and governance-forward — not "get in front of advisors." It's "replace a random motion with an intelligent one."

*Positioning rule for AM audience:* The distribution intelligence layer for the modern asset manager. Replace the random motion with a signal-driven one.

### 10. TAMPs — Envestnet, SEI, AssetMark

Investment platform + back-office for RIAs who outsource operations. **Partner or adjacent**, depending on the RIA segment. Larger, self-sufficient RIAs don't use a TAMP for operations and are clearly Field ICP. Smaller or lifestyle RIAs may live inside a TAMP. Field should be platform-neutral — if your firm is on a TAMP, Field works alongside; if you're not, Field is the firm intelligence layer you'd otherwise lack.

Envestnet is the biggest and most complicated — part TAMP, part data/insights platform (Tamarac, Yodlee, Wheelhouse). There's surface-area overlap on "insights," but Envestnet's insights are platform-gated (for accounts custodied or sub-advised through them). Field's claim is portable: firm intelligence regardless of investment platform.

*Positioning rule:* Field gives RIAs intelligence regardless of investment platform. Works with your TAMP, doesn't require one.

### 11. Broker-dealers / aggregators — LPL, Commonwealth, Raymond James

Own the advisor affiliation for the BD / hybrid channel. **Adjacent**, potentially addressable at the enterprise level (the BD buys Field for its advisors), but the primary RIA ICP is independent. BDs are a segment conversation, not a competitor.

Note: advisors at BDs sometimes hear "network" and think LPL/Commonwealth. This is why the register discipline matters — Field is not a BD network.

*Positioning rule:* Field serves RIAs. Where BDs want a firm intelligence layer for their advisor base, Field is a platform-level conversation.

### 12. Wealthtech / fintech builders — Income Lab, ZOE Financial, ALLINDEX, new builders

**Builder / infrastructure customer** of BridgeFT — these are the firms building new wealth products on top of multi-custodial infrastructure. This audience is developer-first, API-native, and was BridgeFT's existing ICP pre-acquisition. The Phase 1 endorser line ("BridgeFT, part of the Field Network") preserves the brand they chose; the audience doesn't need the Field brand in its face on day one. Field's role: the trusted infrastructure layer they keep building on.

*Positioning rule:* The infrastructure layer for the next generation of wealth products. Trusted, multi-custodial, developer-first.

### 13. Robo / digital advice — Betterment, Wealthfront, SigFig

Direct-to-consumer digital advice. **Adjacent / not ICP.** Different end customer. Mention only to clarify Field is advisor-led, not consumer-facing.

*Positioning rule:* Different end customer. Field is for advisor-led firms.

---

## Cross-cutting observations

**Field is the connective tissue, not a vertical player.** The single most important message embedded in this map: Field is not competing inside any single layer. Field sits above the data-producing layers (1–8) and monetizes both the RIA relationship (platform) and the demand-side cross-section (layer 9, AMs) plus the builder side (layer 12). Anyone who positions Field as a tool inside a single layer is underselling it.

**Two layers need the most language discipline.** Custody (1) and aggregation (8) both get confused with Field by people who haven't heard the full story. The governance conversation lives here — "you own the data, network participation is opt-in, AMs fund the network" — because the comparisons people reach for (custodians, Plaid) would otherwise shape their assumptions.

**One layer is where the flywheel economically closes.** Asset managers (9) are the demand-side revenue that subsidizes the RIA product. Without AM willingness to pay for distribution intelligence, the subsidy model is just marketing. With it, the flywheel is real. This makes AM positioning and early AM wins strategically upstream of everything else — including the May 5 RIA launch narrative.

**TAMP/BD layers (10, 11) require segment-level care, not a single line.** The RIA universe is not homogenous — large independent RIAs, TAMP-reliant smaller RIAs, BD-affiliated hybrid advisors all have different primary platforms. Segment messaging (Section 5 of the framework) should address the "where do you live today" question honestly rather than pretend Field is equally positioned across all of them.

**Substitutability risk is lowest in layer 9, highest in layer 2.** Nobody in layer 9 currently sells what Field's network sells — the distribution intelligence category is essentially new. In layer 2, larger RIAs may perceive Addepar or Envestnet Wheelhouse as "already doing that." The competitive-positioning work for Section 7 of the framework should focus on layer 2 substitutes, not layer 5 (content tools).

---

## Open questions for Bill

1. Is the AM tier list right (BLK, BX, Nuveen, PIMCO, Apollo)? Anyone missing, anyone out of scope at this stage?
2. How do we want to position against Addepar specifically? It's the only player with enough overlap to warrant a specific stance, and the answer shapes Section 7.
3. TAMP/BD — are these addressable at the enterprise level (partnership/platform sales) or explicitly out of scope for the May 5 launch?
4. Where does Precept fit in this map? I've treated its capabilities as absorbed into Field's three-layer architecture, but if Precept had unique ecosystem relationships pre-acquisition, we should surface them.
