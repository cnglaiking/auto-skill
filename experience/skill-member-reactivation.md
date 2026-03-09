# 💤 Skill: Dormant Member Reactivation — Win-Back Campaigns & Results
**Skill ID:** member-reactivation
**Owner:** Charlotte Ng, Sr. Manager, DCH Motors HK
**Last Updated:** 2026-03-09
**Target:** Reactivation rate ≥ 12% (at-risk), ≥ 6% (dormant) | Churn < 5% by Q4 2026

---

## Segmentation: Who Are Dormant Members?

### Definitions
| Segment | Definition | Size (Est. Q1 2026) | Priority |
|---|---|---|---|
| At-Risk | 60–89 days no activity | ~18,000 | HIGH |
| Dormant | 90–179 days no activity | ~28,000 | MEDIUM |
| Lapsed | 180+ days no activity | ~35,000 | LOW-MEDIUM |
| Churned | Unsubscribed or DNC | ~15,000 | LOW (comply only) |

**Total reactivation opportunity:** ~81,000 members (~37% of Q1 member base)

---

## Win-Back Campaign Architecture

### Campaign 1: "We Miss You" — At-Risk (60 days)
**Budget:** HK$15,000/quarter
**Channel Sequence:** Email (Day 1) → Push (Day 3) → WhatsApp (Day 5)

**Email Subject Options (A/B Test):**
- A: "Hi [Name], your MOTOGO points are lonely 😢"
- B: "[Name], you have [X] points waiting for you — don't let them expire!"
- Best performer: B (typically 38% open rate vs 28%)

**Email Body:**
```
Hi [Name],

It's been a while since we've seen you at MOTOGO — and we want to make it worth your while to come back.

As a [Tier] member, you have [X] points ready to use — and we've added 200 bonus points to your account as our 'we miss you' gift.

Here's what's waiting for you:
✅ [X] existing points + 200 bonus points
✅ [Relevant reward based on member history]
✅ Exclusive [Tier] member offer: [Personalised offer]

Your points expire on [date] — redeem them before they disappear!

[CTA: Explore Rewards] [CTA: Book a Service]
```

**WhatsApp Script:**
```
Hi [Name] 👋 It's MOTOGO! 

We haven't seen you for a bit and we've missed you! 

Good news: we've added 200 bonus points to your account 🎁 
Plus your [X] existing points are ready to use.

Tap here to see what you can redeem: [link]
Or reply OFFER and we'll send you our best deal this week 💪
```

**KPIs:** Open rate ≥ 35%, Click rate ≥ 12%, Reactivation (any action within 14 days) ≥ 12%

---

### Campaign 2: "Come Back Stronger" — Dormant (90–179 days)
**Budget:** HK$20,000/quarter (includes HK$50 e-voucher for high-value tier)
**Channel:** WhatsApp primary + Email secondary + TM for Gold/Platinum

**High-Value Trigger (Gold/Platinum dormant):**
- WhatsApp: "Hi [Name], your dedicated MOTOGO concierge here. As a [Gold/Platinum] member, we have a special comeback offer reserved just for you. Reply YES to unlock it."
- If YES: send HK$100 e-voucher + 500 bonus points + personal call from MOTOGO team within 48h

**Standard Trigger (Bronze/Silver dormant):**
- Email: "Your [X] points expire in 30 days — here's your exclusive comeback offer"
- Offer: Double points on next service + HK$30 e-voucher on redemption of 500+ points

**KPIs:** Reactivation rate ≥ 6%, ROI on voucher cost ≥ 3x (vs. acquiring new member at HK$80 CAC)

---

### Campaign 3: "Last Chance Rescue" — Lapsed (180+ days)
**Budget:** HK$8,000/quarter
**Approach:** Single high-impact message, no sequence (avoid spam risk)

**WhatsApp:**
```
Hi [Name], MOTOGO here — one last message before your [X] points expire for good on [date].

We know life gets busy, but we'd love to see you back!

Use code COMEBACK to get: 
• 3x points on your next visit
• Free car health check (HK$280 value)

Book by [date]: [link]

If you'd prefer not to receive messages from us, reply STOP 🙏
```

**Note:** If no response after this message — move to churned list, comply with PDPO, remove from CRM sequences. Do not re-contact without new consent.

---

## Predictive Churn Model (AI-Powered)

### Model Design
- **Platform:** SAP Emarsys AI + Dynamics 365 data
- **Inputs:** Last activity date, transaction history, points balance, tier, age of membership, email open rate (last 90 days), service appointment history
- **Output:** Churn probability score 0–100 (100 = certain churn)
- **Trigger:** Score ≥ 60 → auto-enrol in at-risk journey
- **Accuracy target:** ≥ 70% precision at 60-day prediction horizon

### Churn Probability Scoring Rules
```
+20 points: No activity in 30 days
+15 points: No email open in 60 days
+25 points: No points earned in 90 days
+10 points: Tier drop (Gold → Silver, etc.)
+15 points: 3+ failed WhatsApp deliveries
-10 points: Recent website/app visit
-15 points: Points redemption in last 30 days
-20 points: Service booking in last 60 days
```

---

## ROI Calculation — Why Reactivation > Acquisition

### Cost Comparison
| Action | Cost | Conversion | Revenue per Converted |
|---|---|---|---|
| Acquire new member | HK$80 CAC | 100% (new) | Low CLV initially |
| Reactivate at-risk | HK$12/member | 12% | Full CLV member |
| Reactivate dormant | HK$25/member | 6% | Full CLV member |
| Reactivate lapsed | HK$5/member | 2% | Full CLV member |

### ROI Calculation (Q1 2026)
```
At-risk campaign: 18,000 × HK$12 cost = HK$216,000 spend
Reactivation: 18,000 × 12% = 2,160 members
Revenue per reactivated member (annual): HK$180 avg (purchasing member)
Total revenue recovered: 2,160 × HK$180 = HK$388,800
ROI: (388,800 - 216,000) / 216,000 = 80% ROI
```
→ Even at 6% reactivation, win-back campaigns are 3–5× more efficient than new member acquisition.

---

## Charlotte's Proven Playbooks
1. **"Birthday Comeback Offer"** — dormant members with upcoming birthdays: 2.4× reactivation rate vs. standard campaign
2. **"Points Expiry Countdown"** — 30/14/7 day sequence → urgency drives 19% reactivation on lapsed segment
3. **"New Feature Announcement"** — re-engage dormant by announcing app upgrade / new reward → 8% reactivation with no discount cost
4. **"VIP Personal Touch"** — Gold/Platinum dormant: personal call from MOTOGO team → 31% reactivation rate (vs 6% email-only)
