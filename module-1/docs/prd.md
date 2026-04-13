# PRD: PostedIn — Real Estate Edition

_Updated April 11, 2026_

---

**Version:** 2.0
**Author:** Product Management
**Status:** Draft — Pending PM Review

---

## 1. Problem Statement

**Who we're solving for:** Real estate professionals — operators, developers, investors, advisors, and service providers — who need to stay on top of a fast-moving, fragmented market across multiple asset classes and geographies.

**The pain:** Real estate is a relationship-driven, information-driven industry. The people who move fastest on deals are the ones who see the right signals first. Yet today's information landscape is broken:

1. **Signal-to-noise failure.** Industry news is scattered across dozens of publications, data providers, and deal wires. Relevant signals are buried in generic business news.
2. **No personalization.** A commercial developer in the UK doesn't need US residential mortgage rate news. A PE investor focused on data centres doesn't need hotel RevPAR updates. Existing tools don't know who you are.
3. **Deal awareness gap.** Relevant transactions are announced daily, but most professionals hear about them too late — after pricing is set, counterparties are locked, or the narrative has already formed.
4. **Sharing friction.** When a professional wants to comment on a deal publicly (LinkedIn, client calls, investor updates), they start from scratch with no context scaffold.

**What PostedIn does:** PostedIn delivers a daily, personalized briefing — curated news headlines and deal summaries — filtered by asset class, geography, and professional role. For those who want to extend their reach, the platform offers one-tap deal sharing with AI-assisted commentary, ready for LinkedIn.

---

## 2. Goals

| # | Goal | Metric | Target | Timeframe |
|---|------|--------|--------|-----------|
| G1 | Deliver a genuinely useful daily briefing | % of users who open the briefing each day | ≥ 60% daily open rate | Within 30 days of launch |
| G2 | Surface relevant deals and news (not generic) | In-app relevance rating per item (thumbs up/down) | ≥ 75% positive ratings | Within 60 days of launch |
| G3 | Drive habitual use | 30-day retention rate | ≥ 50% | Within 60 days of launch |
| G4 | Build active user base across target segments | Registered and active users | 300 active users | Within 6 months of launch |
| G5 | Validate LinkedIn sharing add-on | % of DAU who use the share-with-commentary feature at least once per week | ≥ 20% | Within 90 days of launch |

---

## 3. Non-Goals

| ID | Non-Goal | Rationale |
|----|----------|-----------|
| NG1 | **Coverage outside real estate.** PostedIn will NOT cover general business, tech, or macro news beyond its direct real estate relevance. | Vertical focus is the core value. Diluting it undermines relevance. |
| NG2 | **Auto-publishing to LinkedIn.** PostedIn will NOT publish any post without the user explicitly reviewing and approving it. | Professional reputation risk is too high for automation without review. |
| NG3 | **Portfolio management or deal CRM.** PostedIn will NOT track a user's own portfolio, pipeline, or deal history. | That is a different product category. PostedIn is an intelligence and publishing tool, not a CRM. |
| NG4 | **Real-time market data or pricing.** PostedIn will NOT attempt to provide live pricing, valuations, or transaction-level financials. | Data licensing complexity and liability make this a v3+ consideration. |
| NG5 | **Content for platforms other than LinkedIn.** The sharing add-on targets LinkedIn only in v1. | LinkedIn is the dominant professional publishing platform for real estate. |
| NG6 | **Multi-user / team accounts.** v1 targets individual professionals only. | Delegated access and team workflows are a v1.1 consideration after validating the core loop. |

---

## 4. Users & Use Cases

### Asset Class Coverage

PostedIn covers the following real estate asset classes:

| Asset Class | Examples |
|---|---|
| **Commercial** | Office, retail, industrial, logistics |
| **Residential** | Build-to-rent, multifamily, single-family development |
| **Hotels & Hospitality** | Full-service, limited-service, branded residences |
| **Storage** | Self-storage, cold storage, last-mile logistics |
| **Data Centres** | Hyperscale, co-location, edge compute |

### Geographic Markets

| Market | Scope |
|---|---|
| **UK** | England, Scotland, Wales, Northern Ireland |
| **EMEA** | UK + Continental Europe, Middle East, Africa |
| **USA** | National US coverage |
| **APAC** | Asia-Pacific ex-China (Australia, Singapore, Japan, Korea, SE Asia) |

### User Roles

| Role | Description |
|---|---|
| **Operator** | Asset manager or property manager running day-to-day operations |
| **Developer** | Residential or commercial developer, planning through delivery |
| **PE Investor** | Private equity / institutional investor |
| **Private Investor** | Family office, HNWI, private capital |
| **Advisor** | Broker, consultant, lawyer, agent |
| **Service Provider** | Lender, valuer, architect, contractor, PropTech vendor |

---

### Primary Persona

**Name:** The Deal-Aware Real Estate Professional
**Role:** Varies by segment (see roles above)
**Behaviour today:** Scans CoStar, EG, CoStar, Bloomberg, Twitter/LinkedIn, and email newsletters sporadically. Misses deals. Catches news too late. Has opinions but rarely publishes them.
**Key motivations:** Stay ahead of the market, spot deal flow early, build a reputation as a knowledgeable voice.
**Key frustrations:** Too much noise, not enough signal; irrelevant content wastes time; when they want to comment on a deal publicly, it takes too long to draft something worth posting.

---

### Use Case Scenarios

**Scenario 1 — The PE Investor in London**

Amir is a Principal at a real estate PE fund focused on UK logistics and data centres. Every morning he opens PostedIn and sees a briefing filtered to his exact focus: three news items on UK industrial/logistics demand, two data centre investment stories (one cross-border, one domestic), and a summary of two deals that closed in the last 24 hours in his asset classes. He skims the deal summaries. One — a £120M sale-leaseback on a last-mile logistics portfolio — is directly relevant to a transaction he's working on. He taps "Share this deal" and types two sentences about why the pricing signals something about cap rate compression in the sector. PostedIn drafts a 150-word LinkedIn post with his take framed. He edits one sentence, approves it, and schedules it. Total time: four minutes.

**Scenario 2 — The Commercial Developer in Dubai**

Fatima is a development director at a UAE-based developer with projects across EMEA. She selects Commercial and Hotels as her asset classes and EMEA as her market. Each morning her briefing surfaces relevant planning approvals, major leasing announcements, and hotel transaction news from the Gulf, London, and Paris. She doesn't post to LinkedIn often, but when a major hotel brand announces a new EMEA pipeline deal, she uses the "Share with commentary" feature to quickly capture her perspective before her 9 AM call. The draft is done in two minutes — she wouldn't have done it without the scaffold.

**Scenario 3 — The Advisor Wanting to Build a Profile**

Tom is a commercial property advisor in Sydney. He focuses on retail and industrial across Australia and Singapore. He signs up for PostedIn, selects Advisor as his role, APAC as his market, and Commercial and Storage as his asset classes. Each morning he gets a curated briefing. He starts using the "Share with commentary" feature once a week, building a consistent LinkedIn presence focused on APAC real estate trends. Within 60 days, two inbound enquiries from LinkedIn cite his posts.

---

## 5. Onboarding Flow

Onboarding must capture enough context to personalise the daily briefing from day one. It should take under 3 minutes.

### Step 1 — Role & Title

| Question | Input Type | Options |
|----------|-----------|---------|
| What is your role in real estate? | Single select | Operator, Developer, PE Investor, Private Investor, Advisor, Service Provider |
| What is your job title? | Free text | — |
| Who do you work for? (company name) | Free text | Optional |

### Step 2 — Market Focus

| Question | Input Type | Options |
|----------|-----------|---------|
| Which markets do you focus on? | Multi-select | UK, EMEA, USA, APAC exc China |

### Step 3 — Asset Class Focus

| Question | Input Type | Options |
|----------|-----------|---------|
| Which asset classes are relevant to you? | Multi-select | Commercial, Residential, Hotels & Hospitality, Storage, Data Centres |

### Step 4 — Professional Context (for personalization)

| Question | Input Type | Notes |
|----------|-----------|-------|
| What does your current work focus on? (2-3 sentences) | Free text | Used to personalise tone and deal relevance |
| What topics or trends are you most interested in right now? | Free text | Used to refine news curation |

### Step 5 — LinkedIn Connection (optional at onboarding, required for sharing add-on)

- Connect LinkedIn account to enable the share-with-commentary feature
- Users who skip this can still access the daily briefing; they are prompted again the first time they tap "Share"

---

## 6. Core Feature: Daily Briefing

### What the briefing contains

Each daily briefing is composed of two sections:

**Section A — News Headlines**
- 3–7 curated news items per day, filtered by the user's selected asset classes and markets
- Each item: headline, source, 2–3 sentence summary, relevance tag (asset class + market)
- Sourced from: real estate trade publications, RSS feeds, press releases, CoStar/EG data feeds (where available)
- Refreshed every 24 hours, delivered by 7 AM in the user's local timezone

**Section B — Deal Summaries**
- 2–5 notable transactions closed or announced in the last 24–48 hours
- Each deal: asset class, geography, deal type (acquisition, development, JV, refinancing), headline price/size where available, buyer/seller names where public, 2–3 sentence context summary
- Ranked by relevance to the user's profile

### Personalization logic

| Signal | How it's used |
|--------|--------------|
| Role | Adjusts framing of summaries (e.g. PE Investor sees cap rate and returns framing; Developer sees planning/delivery framing) |
| Asset class selection | Filters all content to selected classes; deprioritises others |
| Market selection | Filters geographically; EMEA users see European and Middle East content, not US regional news |
| Free text context (onboarding) | Used as context window for relevance ranking via Claude API |
| Engagement history (post-launch) | Thumbs up/down on items trains future relevance ranking |

---

## 7. Add-On Feature: Share a Deal with Commentary

This is an optional feature layered on top of the daily briefing. It is not required to access the core product.

### Flow

1. User taps "Share this deal" on any deal summary in their briefing
2. PostedIn shows the deal summary with a text input prompt: *"What's your take on this deal? Why does it matter?"*
3. User types 1–3 sentences (text or voice input, minimum 10 characters)
4. PostedIn generates a 100–250 word LinkedIn post that:
   - Leads with the user's perspective
   - Provides deal context from the summary
   - Closes with a question or call to action to drive engagement
   - Matches tone appropriate to the user's role (e.g., investor tone vs. advisor tone)
5. User reviews, edits inline if needed, and either:
   - **Approves & Schedules** — picks a date/time for LinkedIn publishing
   - **Copies to clipboard** — pastes manually into LinkedIn
   - **Discards** — nothing is saved or posted

### Content rules

- PostedIn will NOT generate posts about deals without the user's personal take as input
- Generated posts will NOT include specific financial projections, legal opinions, or claims about deal terms not in the public source
- All generated posts pass a content moderation check before being shown to the user

---

## 8. User Stories

### Must-Have

| ID | User Story |
|----|-----------|
| US-M1 | As a **real estate professional**, I want to **complete a 5-step onboarding that captures my role, market focus, and asset class preferences** so that **my daily briefing is relevant from day one.** |
| US-M2 | As a **real estate professional**, I want to **see a daily briefing of curated news headlines filtered to my selected markets and asset classes** so that **I stay informed without scanning multiple publications.** |
| US-M3 | As a **real estate professional**, I want to **see 2–5 deal summaries per day relevant to my profile** so that **I'm aware of notable transactions in my space as they happen.** |
| US-M4 | As a **real estate professional**, I want to **tap on any deal summary and add my commentary** so that **PostedIn can draft a LinkedIn post with my take, ready to review and share.** |
| US-M5 | As a **real estate professional**, I want to **review and edit the generated LinkedIn post before it goes anywhere** so that **I stay in control of what's published under my name.** |
| US-M6 | As a **real estate professional**, I want to **schedule approved posts to LinkedIn or copy them to clipboard** so that **I have flexibility in how I publish.** |

### Should-Have

| ID | User Story |
|----|-----------|
| US-S1 | As a **real estate professional**, I want to **update my market focus and asset class preferences after onboarding** so that **my briefing evolves as my work focus changes.** |
| US-S2 | As a **real estate professional**, I want to **rate each news item and deal summary as relevant or not relevant** so that **my briefing improves over time.** |
| US-S3 | As a **real estate professional**, I want to **receive the briefing as a daily digest email or push notification** so that **I don't have to remember to open the app.** |
| US-S4 | As a **real estate professional**, I want to **see engagement data for posts I've shared via PostedIn** so that **I can understand what content resonates with my audience.** |

### Nice-to-Have

| ID | User Story |
|----|-----------|
| US-N1 | As a **real estate professional**, I want to **choose from multiple draft framings (e.g. contrarian take, market analysis, personal story)** so that **I can pick the style that fits my audience that day.** |
| US-N2 | As a **real estate professional**, I want to **save a deal or news item to revisit later** so that **I can come back to it when I have more time to post.** |
| US-N3 | As a **real estate professional**, I want to **search past deals and news items in PostedIn** so that **I can find context when I need it for a client conversation or presentation.** |

---

## 9. Acceptance Criteria

### US-M1: Onboarding

```
GIVEN a new user signs up
WHEN they enter the app for the first time
THEN they are walked through 5 steps: role/title, market focus, asset class focus, professional context, and LinkedIn connection (optional)

GIVEN the user completes steps 1–4
WHEN they arrive at the home screen
THEN their daily briefing is already filtered to their selections

GIVEN the user skips LinkedIn connection at onboarding
WHEN they tap "Share this deal" for the first time
THEN PostedIn prompts them to connect their LinkedIn account before proceeding
```

### US-M2 & US-M3: Daily Briefing

```
GIVEN the user has completed onboarding and selected at least one asset class and one market
WHEN they open the app each morning
THEN they see a briefing containing:
  - At minimum 3 news headlines with 2–3 sentence summaries
  - At minimum 2 deal summaries with asset class, geography, deal type, and context
  - All items tagged by asset class and market

GIVEN a news or deal item is displayed
WHEN the user taps on it
THEN they see an expanded view with full summary and source attribution

GIVEN no fresh news or deals are available for a user's selected filters [edge case]
WHEN the briefing loads
THEN the user sees a message explaining this and is shown the most recent available items from their asset classes, clearly dated
```

### US-M4 & US-M5: Share a Deal with Commentary

```
GIVEN a deal summary is displayed in the user's briefing
WHEN the user taps "Share this deal"
THEN they see the deal summary and a text input field prompting them for their take

GIVEN the user submits fewer than 10 characters
WHEN they tap "Generate"
THEN the system shows: "Please share a bit more — even a sentence gives us enough to work with."

GIVEN the user submits a valid take (≥ 10 characters)
WHEN they tap "Generate"
THEN PostedIn returns a LinkedIn draft of 100–250 words within 15 seconds
AND the draft has passed a content moderation check before being shown

GIVEN a draft is displayed
WHEN the user reviews it
THEN they can: edit inline, approve and schedule, copy to clipboard, or discard
```

### US-M6: Scheduling

```
GIVEN the user taps "Approve & Schedule"
WHEN the scheduling screen opens
THEN they can select a date and time, with 2–3 recommended slots highlighted

GIVEN the user confirms a scheduled time
WHEN the scheduled time arrives
THEN the post is published to LinkedIn and marked as published in PostedIn

GIVEN the LinkedIn connection is not set up
WHEN the user attempts to schedule
THEN PostedIn prompts them to connect their LinkedIn account
```

---

## 10. Risks & Assumptions

| Risk | Assumption | Mitigation |
|------|-----------|-----------|
| Real estate deal news sources are fragmented and inconsistent | Sufficient RSS + structured data sources exist for each asset class and market | Seed a curated list of 15–20 high-quality per-market sources; evaluate CoStar API for deal data |
| News relevance scoring requires significant tuning per role | Role-based framing can be approximated via prompt engineering at v1 | Start with rule-based filters (market + asset class tags); layer in ML ranking post-launch |
| Deal summaries may contain inaccurate or incomplete information from public sources | Users understand summaries are drawn from public announcements, not verified financial data | Add a clear source attribution and disclaimer on all deal summaries |
| LinkedIn API access for scheduling may require approval | LinkedIn's API is accessible under standard developer terms for publishing | Begin API application immediately; fall back to clipboard copy at launch if approval is delayed |
| Users in APAC and EMEA have very different deal markets — one curation engine may not serve both well | Regional filtering by market tag is sufficient for v1 | Build modular source lists per market; validate with a small cohort in each region before scaling |
| Content moderation may over-flag legitimate deal commentary | Bold, contrarian views on deals are not inherently harmful | Tune moderation prompts to allow market opinion; flag only genuinely harmful or misleading content |

---

## 11. Monetization

**Model:** Monthly subscription, individual tier only in v1. 7-day free trial. No free plan.

| Tier | Price | What's included |
|------|-------|----------------|
| **Briefing** | £49/month | Daily personalized news + deal summaries, unlimited saves, thumbs up/down feedback |
| **Pro** | £99/month | Everything in Briefing + share-with-commentary (LinkedIn draft generation), scheduling, engagement analytics |

**Unit economics (estimated):**
- Estimated cost (Claude API + data feeds + infra): ~£6–9/user/month
- Gross margin: ~82% at Briefing, ~91% at Pro
- Target: maintain ≥ 80% gross margin as usage scales

---

## 12. Open Questions

| # | Question | Owner |
|---|----------|-------|
| 1 | Which data sources will cover each asset class and market with sufficient deal volume? Which require paid API access (e.g. CoStar, EG)? | Founder |
| 2 | Should users be able to add custom RSS sources or news feeds to supplement the curated briefing? | Founder |
| 3 | How do we handle deals that are rumoured but not publicly confirmed — include with a caveat, or exclude? | Founder |
| 4 | Should the "Share with commentary" feature be gated to Pro from day one, or offered in a limited way on Briefing to drive upgrade? | Founder |
| 5 | For APAC exc China — are we covering China-adjacent deals (e.g. Hong Kong, Singapore cross-border)? | Founder |

---

## 13. Success Metrics

### Leading Indicators

- Daily briefing open rate (target: ≥ 60%)
- Relevance rating on news and deal items (target: ≥ 75% thumbs up)
- % of Pro users who use "Share with commentary" at least once per week (target: ≥ 20%)
- Onboarding completion rate (target: ≥ 85%)

### Lagging Indicators

- 30-day retention rate (target: ≥ 50%)
- Upgrade rate from Briefing to Pro (target: ≥ 30% within 60 days)
- Net Promoter Score at 60 days
- LinkedIn post engagement on PostedIn-generated content vs. user baseline (target: +20% within 90 days)

---

## Sprint 1 — Scope

**Goal:** Ship the core briefing loop. A user can sign up, complete onboarding, and receive a personalized daily briefing of real estate news and deal summaries filtered to their role, markets, and asset classes.

**Sharing add-on:** Included in Sprint 1 as a basic flow (generate draft → edit → copy to clipboard). LinkedIn scheduling deferred to Sprint 2 pending API access.

**Market scope:** UK + EMEA for Sprint 1. USA and APAC in Sprint 2.

**Asset class scope:** All five (Commercial, Residential, Hotels, Storage, Data Centres) — but coverage quality will vary by market at launch.

### Stories in Scope

| Priority | Story | Effort |
|----------|-------|--------|
| 1 | **Onboarding** — 5-step flow capturing role, market, asset class, context, and optional LinkedIn connection | Medium (2–3 days) |
| 2 | **Data ingestion** — RSS and structured feed ingestion for UK/EMEA real estate news and deals, tagged by asset class and market | Large (1 week+) |
| 3 | **Briefing generation** — Claude-powered summarisation and relevance ranking; daily briefing rendered in-app by 7 AM | Large (1 week+) |
| 4 | **Deal sharing (basic)** — User taps "Share", enters take, receives LinkedIn draft, can edit + copy to clipboard | Medium (2–3 days) |
| 5 | **Content moderation** — All generated posts pass moderation check before display | Small (< 1 day) |
| 6 | **Relevance feedback** — Thumbs up/down on each briefing item; stored for future ranking improvements | Small (< 1 day) |

### Sprint 1 Definition of Done

- [ ] A new user can complete 5-step onboarding in under 3 minutes
- [ ] The daily briefing shows ≥ 3 news items and ≥ 2 deal summaries filtered to user's profile
- [ ] All items are tagged by asset class and market
- [ ] If no fresh content is available, a fallback message is shown and recent items are surfaced
- [ ] A user can tap "Share this deal", enter their take, and receive a LinkedIn draft within 15 seconds
- [ ] The draft passes content moderation before being shown
- [ ] A user can edit the draft inline and copy it to clipboard
- [ ] Thumbs up/down feedback is captured per briefing item

### Sprint 2 (Planned)

| Feature | Reason deferred |
|---------|----------------|
| LinkedIn OAuth + scheduling | API access approval timeline uncertain |
| USA market coverage | Validate with UK/EMEA first |
| APAC market coverage | Validate with UK/EMEA first |
| Push notification / email digest | Core in-app loop first |
| Engagement analytics | Requires LinkedIn API post-publish access |
