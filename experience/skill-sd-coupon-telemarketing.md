# 📞 Skill: SD Coupon Telemarketing — Scripts, Optimisation & Revenue Management
**Skill ID:** sd-coupon-telemarketing
**Owner:** Charlotte Ng, Sr. Manager, DCH Motors HK
**Last Updated:** 2026-03-09
**Revenue Line:** HK$840,660/quarter → FY HK$3,362,640 (34.5% of total revenue)
**Risk Level:** CRITICAL — Largest single revenue stream. Contract renewal required Q1 2026.

---

## Programme Overview

### What Is SD Coupon Telemarketing?
- MOTOGO operates an outsourced telemarketing service for SD (Service Department) coupons
- Members receive inbound/outbound calls promoting service bookings, accessory deals, and seasonal campaigns
- Revenue = commission per booking/coupon redemption from SD business unit
- Volume: consistent HK$840,660/quarter (HK$3.36M FY2026)

### Revenue Formula
```
Revenue = Calls Made × Contact Rate × Conversion Rate × Avg Commission Value
= ~50,000 calls × 22% contact × 18% conversion × HK$420 commission
= HK$840,660
```

---

## Telemarketing Scripts — Best Performing Versions

### Script A: Service Booking (Standard Member)
```
"Hi, am I speaking with [Name]? 

I'm calling from MOTOGO Loyalty Programme at DCH Motors. 
We noticed your [Car Model] is due for its [service type] — and as a valued member, 
we'd love to help you book it today with a special [Tier] member discount.

You'll also earn [X] MOTOGO points on this visit — taking you closer to [next tier reward].

Can I check your availability — morning or afternoon works better for you?"
```
**Conversion rate:** 18–22%
**Best time:** Tue–Thu, 10am–12pm, 2pm–5pm HKT

---

### Script B: Dormant Member Re-engagement Call
```
"Hi [Name], this is [Agent] from MOTOGO at DCH Motors.

We haven't seen you for a while and wanted to personally reach out — 
your [X] MOTOGO points are due to expire on [date], 
and we have a special offer reserved just for you.

If you book a service this month, we'll double your points AND 
give you a HK$[X] service credit as our 'welcome back' gift.

Shall I check what's available at your nearest DCH service centre?"
```
**Conversion rate:** 14–16% (dormant segment)
**Best outcome:** Combine with WhatsApp pre-send 2 days before call

---

### Script C: Referral Warm Lead Call (MCL Pipeline)
```
"Hi [Name], congratulations — your friend [Referrer Name] has recommended you 
as someone who might be interested in [vehicle model / service].

As a MOTOGO referral guest, you're entitled to [special offer] 
with no obligation — just a complimentary test drive / consultation.

Can I arrange a time for our specialist to call you back, 
or would you prefer to visit our showroom at [location]?"
```
**Conversion rate:** 26–32% (warm referral)
**Handoff:** Log in Dynamics 365 as MCL lead, flag for BU follow-up within 24h

---

## Contract Renewal Strategy (Q1 2026 — CRITICAL)

### Current Contract Status
- Renewal deadline: **January 31, 2026**
- Revenue at risk if not renewed: HK$3,362,640
- Fallback plan: In-house TM pilot (30% capacity, 60-day setup time)

### Renewal Negotiation Points
1. Volume guarantee: commit to 45,000+ calls/quarter in exchange for better commission split
2. Quality metrics: add conversion rate minimum 16% to SLA (current 18% — room to negotiate)
3. Exclusivity: push for HK automotive segment exclusivity with TM vendor
4. Data ownership: all call outcomes, contact data, recordings owned by DCH Motors/MOTOGO
5. Tech integration: vendor must support Dynamics 365 API for real-time lead sync

### Escalation Plan
- If renewal delayed past Jan 31: Charlotte to escalate to GM with business case deck
- Business case: SD Coupon TM = 34.5% of MOTOGO revenue, direct service department revenue driver
- Board-level number: ~HK$3.36M programme revenue at risk + indirect SD department revenue HK$8–12M

---

## Performance Optimisation Framework

### Monthly Review Checklist
- [ ] Total calls made vs target (50,000/quarter = 16,667/month)
- [ ] Contact rate (target ≥ 22%)
- [ ] Conversion rate (target ≥ 18%)
- [ ] Average commission per conversion (target ≥ HK$420)
- [ ] Compliance: no-call list checks, PDPO adherence
- [ ] Script A/B test results (rotate scripts quarterly)
- [ ] Best-performing time slots (update call schedule accordingly)

### Segment Prioritisation (Highest ROI First)
1. **Gold/Platinum members** — highest CLV, personalised scripts, priority call slots
2. **At-risk (90 days no activity)** — re-engagement + service combo offer
3. **Birthday month members** — bonus points + service offer (emotional trigger)
4. **Vehicle age ≥ 3 years** — service reminder (maintenance need + loyalty offer)
5. **New members (30–90 days)** — first service booking habit formation

---

## Integration with CRM

### Dynamics 365 Call Log Fields
```
Contact_Type: TM_SD_Coupon
Call_Outcome: [Booked / Interested / Not_Interested / No_Answer / DNC]
Script_Version: [A / B / C]
Commission_Value: [HK$ amount]
Points_Promised: [number]
Follow_Up_Date: [date if applicable]
Agent_ID: [agent code]
Booking_Ref: [SD booking reference number]
```

### Emarsys Suppression Sync
- DNC (Do Not Call) → auto-suppress from all TM lists in Emarsys within 24h
- Converted members → remove from TM queue, add to "Active Purchaser" segment
- No Answer ×3 → move to "Low Contact" segment, attempt WhatsApp follow-up instead

---

## Charlotte's Proven Wins
- **"Pre-call WhatsApp + TM Call" sequence** → 23% conversion uplift vs cold call alone
- **Tier personalisation in Script A** → mentioning member tier by name → +8% conversion
- **Time slot optimisation** → shifting calls from 5–7pm to 10am–12pm → contact rate +5%
- **Birthday month overlay** → adding birthday offer to TM script in member's birth month → 34% conversion
