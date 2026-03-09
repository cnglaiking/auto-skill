# 📣 CRM Campaign Strategy, Channel Rules & Best Practices
**Last Updated:** 2026-03-09
**Platform:** SAP Emarsys + Microsoft Dynamics 365 + WhatsApp (OmniChat)
**Programme:** MOTOGO | DCH Motors HK

---

## CRM Platform Stack

| Platform | Role | Use Case |
|---|---|---|
| **SAP Emarsys** | Marketing automation engine | Email lifecycle, triggered campaigns, A/B testing, segmentation |
| **Microsoft Dynamics 365** | CRM & sales pipeline | Member records, referral tracking, BU sales data, service history |
| **WhatsApp (OmniChat)** | Conversational CRM | 1:1 re-engagement, insurance chatbot, win-back, VIP comms |
| **MOTOGO App** | Member portal + push | Points balance, offers, event booking, gamification |
| **CDP (in progress)** | Unified data layer | Merging POS, app, CRM, web, TM data into single customer view |

---

## 6-Stage Lifecycle CRM Journey

```
Stage 1: WELCOME (Day 0–7)
→ Trigger: New enrolment
→ Channel: Email + App push + WhatsApp (if opted in)
→ Content: Welcome + 200 bonus points + "How MOTOGO works" guide
→ KPI: Email open rate ≥35%, App activation ≥40%

Stage 2: ONBOARD (Day 7–30)
→ Trigger: No first transaction after Day 7
→ Channel: WhatsApp Day 7 + Email Day 14 + App push Day 21
→ Content: "Your first reward is waiting" + specific product offer
→ KPI: First Purchase Rate ≥30% within 30 days

Stage 3: FIRST EARN (Transaction 1)
→ Trigger: First points-earning transaction
→ Channel: Email + App push (real-time)
→ Content: Congratulations + points summary + "next milestone" preview
→ KPI: Repeat transaction within 60 days ≥50%

Stage 4: FIRST REDEEM (Points redemption milestone)
→ Trigger: Sufficient points accumulated (threshold set per tier)
→ Channel: App push + Email
→ Content: "You've earned enough to redeem!" + redemption options
→ KPI: Redemption rate ≥25% (target 35% by Q4)

Stage 5: TIER UPGRADE
→ Trigger: Member crosses tier threshold
→ Channel: WhatsApp (personal feel) + Email
→ Content: Congratulations + new tier benefits + what's unlocked
→ KPI: Post-upgrade purchase within 30 days ≥60%

Stage 6: RE-ENGAGEMENT
→ Trigger: 90 days no transaction
→ Channel: WhatsApp → Email → App push (3-touch sequence)
→ Content: Points expiry urgency + strong offer (min 2x points or HK$50 voucher)
→ KPI: Reactivation rate ≥12%
```

---

## Channel Strategy & Rules

### WhatsApp CRM (HIGHEST PRIORITY)
- **Engagement rate target:** ≥45%
- **Frequency rule:** Maximum 2 broadcast messages per member per month (respect attention)
- **Best for:** VIP comms, win-back, insurance chatbot, transactional updates
- **Tone:** Conversational, warm, human — never corporate-sounding
- **Format:** Keep under 160 characters + one clear CTA
- **Do NOT:** Mass blast with promotional content — high unsubscribe risk
- **Personalisation:** Always include member name + relevant data point

### Email (SAP Emarsys)
- **Open rate target:** ≥22% (industry benchmark automotive: 18%)
- **CTR target:** ≥3%
- **Best for:** Lifecycle journeys, campaign newsletters, monthly member digest, offer blasts
- **Send time:** Tuesday–Thursday, 10am–12pm HKT performs best
- **Subject line rules:** Personalise with name, use urgency/benefit, under 50 chars
- **Design:** Mobile-first, single column, strong hero image, one primary CTA
- **A/B test:** Subject line + CTA button text minimum per major campaign

### App Push Notification
- **DAU/MAU target:** ≥18%
- **Best for:** Time-sensitive flash offers, event reminders, points milestone alerts
- **Frequency:** Max 3 push notifications per week per member
- **Timing:** Evening 7–9pm performs best for consumer app
- **Do NOT:** Send generic push — kills opt-in rate

### Social Media (IG/FB)
- **IG:** Visual storytelling, member lifestyle, event highlights — younger demographic
- **FB:** Community, older demographic, event promotions, referral campaigns
- **Posting cadence:** 3 posts/week (1 product/offer, 1 lifestyle, 1 community/UGC)
- **Engagement rate target:** ≥4%
- **UGC programme:** Monthly #MOTOGOLife challenge — members share driving moments
- **Paid:** Meta ads for acquisition campaigns (new member target cost: <HK$12 CPA)

### Telemarketing (SD Coupons + Others)
- **Contact rate target:** ≥35%
- **SD Coupon conversion target:** ≥12%
- **Revenue:** HK$840,660/quarter (stable floor — protect this)
- **Script rule:** AI-assisted prompts; personalise opening with member vehicle/service history
- **Upsell protocol:** Always pair SD Coupon pitch with one secondary offer (E-Shop / Insurance)
- **Compliance:** All calls recorded; PDPO consent confirmed before data use

---

## Campaign Execution Rules

### Before Any Campaign Launch
- [ ] Audience segment defined (no generic "all members" blasts)
- [ ] A/B test variants prepared (subject line + CTA minimum)
- [ ] Suppression list applied (recent buyers, opted-out, VIPs on separate track)
- [ ] Legal review for promotions with financial incentives
- [ ] Mobile preview checked
- [ ] UTM tracking in place for all links

### After Every Campaign
- [ ] Open rate, CTR, conversion tracked within 48 hours
- [ ] Compare vs benchmark (see kpi-benchmarks-2026.md)
- [ ] Document learnings in experience/skill-crm-campaigns.md
- [ ] Share top-line results with relevant BUs within 1 week

---

## A/B Testing Framework
- **Minimum 2 tests per month** across all active campaigns
- Test ONE variable at a time: subject line OR send time OR CTA text OR image
- Minimum sample: 500 per variant for statistical significance
- Winner criteria: ≥10% lift in primary KPI
- Document all test results — wins AND losses — in experience log

---

## WhatsApp Insurance Chatbot Flow (Q2 2026 Launch)
```
Trigger: Member vehicle age ≥ 3 years (data from Dynamics 365)
→ WhatsApp: "Hi [Name], your [Vehicle Model] is coming up for insurance renewal. 
   As a MOTOGO member, you get exclusive rates. Want a quick quote?"
→ Yes response: "Great! Just confirm your vehicle registration [XXXX]?"
→ Confirmation: Instant quote returned via chatbot
→ Interested: Route to insurance partner for closing
→ Not now: "No problem! I'll check back in 30 days. Enjoy your drive 🚗"
```
KPI: 500+ quotes/month, 50+ policies/month (Q2 target)

---

## Campaign Budget Rules (A&P = HK$1,000,000 FY2026)
- Never exceed quarterly allocation without Charlotte approval
- All spend over HK$50,000 requires brief + sign-off
- Events budget ring-fenced: HK$300,000 (Spring Drive + VIP Night)
- Contingency HK$100,000 — for unplanned opportunities only; requires Charlotte approval
- Monthly spend tracking vs plan — report in monthly CRM review
