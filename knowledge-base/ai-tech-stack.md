# 🤖 DCH Motors AI & Tech Stack — CRM Platforms, CDP & Tools
**Last Updated:** 2026-03-09
**Owner:** Charlotte Ng (Technology oversight for CRM/Loyalty/Data)

---

## Current Technology Stack

### 1. SAP Emarsys — Marketing Automation
- **Role:** Email lifecycle automation, triggered campaigns, A/B testing, audience segmentation
- **Key capability:** Smart personalisation, send-time optimisation, revenue attribution
- **Charlotte's use:** 6-stage lifecycle journeys, monthly campaign blasts, retention flows
- **Integration status:** Connected to Dynamics 365; partial app data
- **Limitation:** Not yet connected to CDP (in progress); limited offline data ingestion
- **Contract:** Existing — annual renewal, key vendor relationship to maintain

### 2. Microsoft Dynamics 365 — CRM & Sales Pipeline
- **Role:** Master member records, referral tracking, service history, BU sales data
- **Key capability:** 360-degree member view (when data is complete), pipeline management
- **Charlotte's use:** MCL referral pipeline, member profile management, BU reporting
- **Integration status:** Connected to Emarsys; limited real-time sync with POS
- **Limitation:** Data silos across 11 BUs; manual data entry in some BUs
- **Action needed:** Standardise BU data input protocols (Q1 2026)

### 3. WhatsApp CRM (OmniChat)
- **Role:** Conversational CRM, 1:1 member engagement, broadcast campaigns
- **Key capability:** Chatbot flows, rich media messages, two-way conversation
- **Charlotte's use:** Re-engagement, insurance chatbot, VIP comms, win-back
- **Engagement stats:** ≥45% open rate target (vs email 22%)
- **Compliance:** PDPO consent required for all broadcast; opt-out honoured immediately
- **Best practice:** Max 2 broadcasts/month per member; personalise every message

### 4. MOTOGO App
- **Role:** Member portal — points balance, offer wallet, service booking, event RSVP
- **Key capability:** Push notifications, gamification framework, loyalty card display
- **Charlotte's use:** Activation campaigns, event management, tier progression tracking
- **Current gap:** App UX refresh needed (Q2 2026 priority); gamification module to launch
- **DAU/MAU target:** ≥18% by Q4 2026

### 5. CDP — Customer Data Platform (New Initiative 2026)
- **Role:** Unify all data sources into single customer view
- **Status:** Vendor assessment Q1 → Implementation Q2–Q3 → Live Q3 2026
- **Data sources to unify (minimum 6):**
  1. POS transaction data (all 11 BUs)
  2. CRM (Dynamics 365) member records
  3. App behaviour data
  4. E-Shop purchase data
  5. Telemarketing contact logs
  6. WhatsApp interaction data
  7. Partner data (Esso, insurance)
- **Charlotte's KPI:** ≥6 sources unified by Q3; ≥75% member profile completeness
- **Business case:** "DCH Motors Data Transformation 2026-2027" — board-level initiative
- **Benefit:** Real-time personalisation, better attribution, predictive models

### 6. Predictive Churn Model (AI — New 2026)
- **Role:** Identify members at risk of churning 60 days in advance
- **Target accuracy:** ≥70%
- **Trigger:** Auto-launch re-engagement journey when churn risk score exceeds threshold
- **Timeline:** Scoping Q1 → Build Q2 → Test Q2 → Launch Q3
- **Data inputs:** Transaction recency, frequency, channel engagement, NPS responses

### 7. AutoSkill AI (This System)
- **Role:** Charlotte's AI second brain — institutional knowledge system
- **Function:** Auto-loads DCH Motors context for every AI session
- **Contents:** Programme strategy, member personas, KPIs, campaign rules, brand voice, promotion playbook
- **How to update:** After successful sessions, write learnings to `experience/` folder
- **GitHub:** https://github.com/cnglaiking/auto-skill

---

## Data Privacy & Compliance (PDPO HK)

### Key Rules
- All member data collected must have explicit consent at point of enrolment
- Marketing communications require opt-in (not opt-out) — especially WhatsApp
- Data retention policy: active member data retained; inactive members (3yr+) reviewed annually
- Data access: role-based; BU staff see only their BU member data
- Analytics: anonymised / aggregated data for reporting; no personal data in dashboards
- Third-party data sharing (insurance, Esso): Data Processing Agreement required
- Breach protocol: Charlotte notified within 24 hours; escalation to legal within 48 hours

### Campaign Compliance Checklist
- [ ] Consent verified for all target segments
- [ ] Opt-out mechanism in every communication
- [ ] T&C for all prize promotions
- [ ] Financial promotions reviewed by legal (insurance, SD coupons)
- [ ] Data subject access request process documented

---

## Tech Roadmap 2026

| Quarter | Initiative | Owner | Impact |
|---|---|---|---|
| Q1 | BU data reporting standardisation | Charlotte + Data team | 11/11 BUs reporting |
| Q1 | CDP vendor selection | Charlotte + IT | Foundation for Q2 build |
| Q2 | Insurance chatbot (WhatsApp) | CRM team | VAS revenue unlock |
| Q2 | CDP Phase 1 implementation | IT + Charlotte | First 3 data sources |
| Q2 | App gamification launch | App team | Engagement boost |
| Q3 | CDP Phase 2 (all 6+ sources) | IT + Charlotte | Full unified view |
| Q3 | Predictive churn model live | Data analyst | Proactive retention |
| Q3 | Real-time KPI dashboard | Analytics | Weekly BU reviews |
| Q4 | Loyalty tier algorithm upgrade | Charlotte + Tech | Better personalisation |
| Q4 | 2027 overseas tech scoping | Charlotte | GBA expansion |

---

## AI Tools Charlotte Uses (2026 Stack)
- **AutoSkill** — Knowledge base and session memory
- **Genspark AI** — Strategic planning, document creation, deep research
- **SAP Emarsys AI** — Send-time optimisation, subject line suggestions
- **Microsoft Copilot** — Dynamics 365 data queries, report generation
- **ChatGPT / Claude** — Campaign copy drafting, analysis assistance
- **Power BI (via Dynamics)** — BU performance dashboards
