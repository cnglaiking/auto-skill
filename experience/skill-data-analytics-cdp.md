# 📊 Skill: Data Analytics, CDP & Predictive Intelligence
**Skill ID:** data-analytics-cdp
**Owner:** Charlotte Ng, Sr. Manager, DCH Motors HK
**Last Updated:** 2026-03-09
**Initiative:** CDP Integration — Unified 11-BU Customer Intelligence Platform

---

## Charlotte's Data Vision (2026)

> "Every marketing decision at DCH Motors should be traceable to a data insight. Every member interaction should be personalised based on real behaviour. And every business unit should be able to see, in real time, how MOTOGO members are contributing to their revenue."

This is Charlotte's operating philosophy — and the basis of the CDP project that will define her legacy at DCH Motors.

---

## Current Data Architecture (Pre-CDP)

### Challenges
- 11 BUs each maintain separate customer records — no unified member view
- Emarsys (email/CRM), Dynamics 365 (CRM/leads), and MOTOGO App are partially integrated but not unified
- Member identity resolution: same person may exist as 3+ records across systems
- Attribution: impossible to track which campaign influenced a vehicle sale across BUs
- Reporting: manual data pulls, Excel-heavy, monthly lag

### Data Sources Available
| Source | Data Type | Volume | Integration Status |
|---|---|---|---|
| MOTOGO App | Member profile, points, transactions | 344K profiles | ✅ Live |
| SAP Emarsys | Email behaviour, campaign data | 344K | ✅ Integrated |
| Dynamics 365 | CRM leads, vehicle sales, TM logs | ~200K | ⚠️ Partial |
| E-Shop | Purchase data, SKU, basket | ~50K transactions/yr | ⚠️ Partial |
| SD (Service Dept) | Service history, vehicle service records | ~150K records/yr | ❌ Not integrated |
| Esso / Fuel Card | Fuel transaction data | ~30K active users | ⚠️ Partial |
| Insurance Partner | Policy data (new 2026) | 0 (new) | ❌ TBD |
| BU Sales Systems | Vehicle purchase records (11 BUs) | ~15K transactions/yr | ❌ Not integrated |

---

## CDP Integration Roadmap (2026)

### Phase 1: Foundation (Q1 2026)
**Goal:** Define golden record, connect core systems
- [ ] Select CDP vendor (shortlist: Salesforce CDP, Segment, mParticle, Adobe Real-Time CDP)
- [ ] Data audit: map all 11 BU data sources, data formats, and field definitions
- [ ] Identity resolution logic: define matching rules (phone > email > name+car reg)
- [ ] PDPO compliance review: data usage consent framework for unified profile
- [ ] Connect MOTOGO App + Emarsys + Dynamics 365 as Phase 1 sources
- **Deliverable:** Unified profile for 200K+ members with 5+ data attributes

### Phase 2: Intelligence (Q2–Q3 2026)
**Goal:** Build analytics and prediction capabilities
- [ ] Member 360 view: single screen showing all touchpoints per member
- [ ] Predictive churn model: deploy AI model (accuracy ≥ 70%)
- [ ] Member Lifetime Value (MLV) scoring: tier all members by projected 12-month value
- [ ] Campaign attribution model: multi-touch attribution for MOTOGO revenue streams
- [ ] Real-time KPI dashboard: live view for Charlotte + BU leaders
- **Deliverable:** Churn model live, MLV scores for 100% of active members

### Phase 3: Activation (Q4 2026)
**Goal:** Use data to drive autonomous personalisation
- [ ] Real-time triggers: behaviour → automated message within 15 minutes
- [ ] Next-best-action engine: AI recommends next offer/message for each member
- [ ] BU data sharing: each BU accesses MOTOGO member data relevant to their business
- [ ] GBA readiness: data structure supports Mainland China member expansion
- **Deliverable:** CDP fully operational, 11 BUs reporting from unified platform

---

## Predictive Churn Model — Technical Specification

### Model Architecture
```
Type: Binary classification (churn / no-churn)
Prediction horizon: 60 days
Training data: 18 months historical member behaviour
Features: 
  - Days since last activity
  - Points balance (earned vs redeemed ratio)
  - Transaction frequency trend (3-month vs 6-month)
  - Email engagement (open rate 30/60/90 days)
  - Tier (Bronze = higher churn risk)
  - WhatsApp delivery rate (failed = potential number change)
  - Service history gap (vehicle age vs service frequency)
  - Referral activity (referrers churn 40% less)
  
Output: Churn probability score 0–100 + segment tag
```

### Model Accuracy Targets
| Metric | Target |
|---|---|
| Accuracy | ≥ 70% |
| Precision | ≥ 65% |
| Recall | ≥ 75% |
| F1 Score | ≥ 0.70 |
| False positive rate | < 20% |

### Business Impact Calculation
```
Members scored ≥ 60 (at-risk): ~18,000/quarter
Reactivation rate with intervention: 12%
Revenue per reactivated member: HK$180/year
Annual revenue saved: 18,000 × 12% × HK$180 = HK$388,800
Model development cost: HK$150,000 (one-time)
Annual ROI: HK$238,800 (year 1), HK$388,800 (year 2+)
```

---

## KPI Dashboard Design — Charlotte's Executive View

### Dashboard 1: Board-Level (Monthly)
```
┌─────────────────────────────────────────────────────────────┐
│  MOTOGO LIVE KPI DASHBOARD — [Month Year]                   │
├──────────────┬──────────────┬──────────────┬───────────────┤
│ Revenue      │ Members      │ Active Rate  │ NPS Score     │
│ HK$X.XXM     │ XXX,XXX      │ X.XX%        │ +XX           │
│ vs plan [+/-]│ vs plan [+/-]│ vs plan [+/-]│ vs plan [+/-] │
├──────────────┴──────────────┴──────────────┴───────────────┤
│ REVENUE STREAMS          │ MEMBER FUNNEL                   │
│ SD Coupon: HK$XXX,XXX    │ Total: XXX,XXX                  │
│ MCL: HK$XXX,XXX          │ Active: XX,XXX (X.XX%)          │
│ E-Shop: HK$XXX,XXX       │ Purchasing: XX,XXX              │
│ Insurance: HK$XX,XXX     │ At-Risk: XX,XXX                 │
│ Ext Fee: HK$XX,XXX       │ Churned: XX,XXX                 │
├──────────────────────────┴─────────────────────────────────┤
│ ALERTS: [Any KPI > 10% off plan highlighted in red]        │
└─────────────────────────────────────────────────────────────┘
```

### Dashboard 2: BU Coordinator View (Weekly)
- MCL pipeline by BU
- TM contact/conversion rates
- New members from BU referral
- Service bookings via MOTOGO

---

## Charlotte's Data Leadership Narrative (Promotion-Ready)

> "I'm not just running a loyalty programme — I'm building DCH Motors' customer intelligence infrastructure. The CDP project, predictive churn model, and 11-BU unified reporting platform represent HK$1–2M in future cost avoidance and HK$388K+ in annual reactivation revenue. More importantly, they position DCH Motors as a data-driven organisation — a competitive differentiator in HK's automotive market."

This framing elevates Charlotte from "Sr. Manager" to "transformation leader" — essential for the GM/Director promotion case.
