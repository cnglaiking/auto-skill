# 🔄 Skill: CRM Lifecycle Journey Design & Automation
**Skill ID:** crm-lifecycle-journey
**Owner:** Charlotte Ng, Sr. Manager, DCH Motors HK
**Last Updated:** 2026-03-09
**Platform:** SAP Emarsys + Microsoft Dynamics 365 + WhatsApp (OmniChat)

---

## Purpose
This skill codifies best practices for designing, building, and optimising automated CRM lifecycle journeys for the MOTOGO loyalty programme. Use this when asked to: design a CRM journey, write automation logic, set up triggered messages, or improve lifecycle metrics.

---

## MOTOGO Lifecycle Architecture — 6 Stages

### Stage 1: Welcome (Day 0–7)
**Trigger:** Member registration confirmed
**Goal:** First impression, immediate value, activate first action
**Channels:** Email → Push Notification → WhatsApp (Day 3 if no open)
**Sequence:**
- Day 0: Welcome email — personalised (name, car model if known), points balance, app download CTA
- Day 1: Push: "Your MOTOGO journey starts now 🚗" — link to earn guide
- Day 3 (no open): WhatsApp: "Hi [Name], welcome to MOTOGO! Here's your first reward 🎁" — attach QR voucher
- Day 7: Email: Top 5 ways to earn points — education content

**KPIs:** Open rate ≥ 45%, App activation ≥ 30%, First action within 7 days ≥ 25%

---

### Stage 2: Onboarding (Day 8–30)
**Trigger:** Welcome stage completed, no first purchase yet
**Goal:** Drive first earning behaviour (service booking / e-shop / event)
**Channels:** Email + WhatsApp alternating (respect 48h gap)
**Sequence:**
- Day 8: Email — "Earn your first 500 points: Book a service today"
- Day 14: WhatsApp — "Don't let your welcome bonus expire! Redeem by [date]"
- Day 21: Push — Member milestone animation: "You're 500 points away from Silver tier 🥈"
- Day 28: Email — "Last chance: Your onboarding bonus expires in 3 days"

**KPIs:** First purchase conversion ≥ 30% within 30 days, Onboarding completion rate ≥ 60%

---

### Stage 3: Earn (Active Member Phase — Ongoing)
**Trigger:** Member has completed at least 1 earning action
**Goal:** Sustain engagement, increase purchase frequency, tier progression
**Channels:** Email (bi-weekly), WhatsApp (event-triggered), Push (real-time)
**Rules:**
- Points earned → instant Push confirmation
- Approaching tier threshold: trigger 3-touch sequence (Email → Push → WhatsApp)
- Birthday month: special 2x points offer email (personalised)
- Quarterly: Points summary + "You're [X] points from [next tier]"

**KPIs:** Active rate Q4 ≥ 10.27%, Avg transactions/active member ≥ 2.3/quarter, Points issuance ratio ≥ 70%

---

### Stage 4: Redeem (Reward Engagement)
**Trigger:** Member has >500 redeemable points OR has been active for 60+ days without redemption
**Goal:** Drive redemption, close the reward loop, reduce liability
**Channels:** Email + WhatsApp
**Sequence:**
- Trigger A (>500 pts): "You have [X] points! Here's what you can redeem 🎁" — personalised reward carousel
- Trigger B (60 days no redemption): "Your points are waiting — don't let them expire! [CTA: View Rewards]"
- Trigger C (expiry warning 30 days): Urgent WhatsApp — "⚠️ [X] points expiring on [date]! Redeem now"

**KPIs:** Redemption rate Q4 ≥ 35%, Reward claim rate ≥ 80% on triggered offers

---

### Stage 5: Tier Up (Loyalty Deepening)
**Trigger:** Member crosses tier threshold (Bronze → Silver → Gold → Platinum)
**Goal:** Celebrate milestone, communicate new benefits, reinforce status
**Channels:** Email (premium HTML) + Push + WhatsApp (personal touch for Gold/Platinum)
**Sequence:**
- Immediate: Tier upgrade congratulations email — personalised, animated, new benefits list
- +1 day: Push — "Welcome to [Tier] 🏆 Your new benefits are live"
- Gold/Platinum only: WhatsApp from "MOTOGO Concierge" — "Congratulations [Name], I'm your dedicated MOTOGO concierge. How can I help?"

**KPIs:** Tier progression rate ≥ 15% per quarter, VIP (Gold+Platinum) ≥ 5% of active members by Q4

---

### Stage 6: Re-engage (Win-Back)
**Trigger:** No activity for 90 days (at-risk), or 180 days (dormant)
**Goal:** Win back lapsed members before permanent churn
**Channels:** WhatsApp primary, Email secondary, Telemarketing for high-value segments
**Sequence (At-Risk — 90 days):**
- Day 90: Email — "We miss you! Here's 200 bonus points to come back 🙏"
- Day 97: WhatsApp — "Hi [Name], your MOTOGO points expire in 60 days. Don't lose them!"
- Day 105: Push — Limited offer: "Today only — double points on your next service"

**Sequence (Dormant — 180 days):**
- WhatsApp + HK$50 e-voucher (high-value tier only)
- Telemarketing call for members with past purchase history (via SD Coupon TM team)

**KPIs:** Reactivation rate ≥ 12% on at-risk, ≥ 6% on dormant, Churn Q4 < 5%

---

## Technical Setup — SAP Emarsys Configuration

### Program Settings
```
Journey Type: Multi-channel automated
Entry: Database filter → segment trigger
Re-entry: Allowed (after 90 days)
Frequency cap: Max 3 messages/week per member
Timezone: HKT (UTC+8)
Unsubscribe: Single click, auto-update Dynamics 365
```

### WhatsApp Template Naming (OmniChat)
```
motogo_welcome_d0
motogo_welcome_d3
motogo_onboard_d14
motogo_redeem_expiry_30d
motogo_tiereup_gold
motogo_winback_90d
motogo_winback_hv_180d
```

### A/B Test Rules
- Minimum 2 A/B tests per month across lifecycle stages
- Test duration: 7 days minimum, 10,000 recipients minimum per variant
- Test variables: Subject line, CTA text, Send time (10am vs 7pm), Channel order (Email first vs WhatsApp first)

---

## Performance Benchmarks (2026 Targets)

| Stage | KPI | Target |
|---|---|---|
| Welcome | Open rate | ≥ 45% |
| Welcome | App activation | ≥ 30% |
| Onboarding | First purchase in 30d | ≥ 30% |
| Earn | Active rate | ≥ 10.27% Q4 |
| Redeem | Redemption rate | ≥ 35% Q4 |
| Tier Up | Tier progression | ≥ 15%/quarter |
| Re-engage | At-risk reactivation | ≥ 12% |
| Re-engage | Churn rate | < 5% Q4 |

---

## Charlotte's Proven Playbooks
1. **"Points Expiry Urgency"** — 3-touch WhatsApp sequence 30/14/7 days before expiry → 23% redemption lift
2. **"Tier Teaser"** — Send progress bar email "You're 200 pts from Silver" → 31% click-through
3. **"Birthday 2x Points"** — Personalised birthday month campaign → 2.8x average revenue vs baseline
4. **"Service Reminder + Points"** — Combine service booking reminder with points reminder → 42% booking rate
