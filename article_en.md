# Censorship as Recommendation: A Conjecture on the Advertising Revolution in the Age of AI Visual Understanding

> **Foreword**: I've been sitting on this question for a while — since AI image and text recognition is already so accurate, why haven't WeChat, ByteDance, Google, TikTok, and Meta — platforms sitting on oceans of content — implemented cross-verified precision ad targeting that matches platform content with advertiser products? The answer: **they absolutely can. They're choosing not to.** And when the cost of multimodal understanding drops far enough, the rules of the game will be rewritten entirely.


---


## 1. Historical Review: Three Advertising Revolutions


### The Print Era: Classified Ads → Paid Search


Early advertising was yellow-page-style information display — you searched by category, no filtering mechanism. Search gave us paid ranking, with keyword matching as the core logic. The defining feature of this era: **information asymmetry reigned, users were passive recipients**.


### The Social Media Era: Interest Tags → Feed Ads


Facebook and Google pioneered precision targeting based on user profiles: "male, 30-45, tier-1/2 cities, fitness enthusiast." This system was enormously successful from 2010-2020, but it planted a hidden flaw: **interest tags are lagging indicators**.


A user wants to buy a phone today. The system needs a week of behavioral data to infer that intent. By then, they've already ordered from a competitor.


### The Short-Video Era: The Skip Button Is Born


In 2015, YouTube launched TrueView, allowing users to skip ads after 5 seconds. This was the industry's first public admission of a problem: **users genuinely hate being interrupted**.


TikTok and Douyin followed suit. Skippable ads became standard. The irony: this only made advertisers more anxious — they started obsessing over "completion rates" instead of actually optimizing content value.


**Key insight**: The skip button isn't progress. It's a compromise. It signals that the traditional advertising model has run its course.


---


## 2. The Technical Truth: Why Giants Choose Conservatism


### Capability Reserves: They're Stronger Than You Think


Based on public patents and papers: ByteDance's object recognition patent (US2022037456A1) already supports video-level object detection and scene classification. Tencent's AI Lab has published multiple image understanding papers at CVPR and ICCV, with OCR and sentiment analysis capabilities for WeChat Official Account content. Google Cloud Video Intelligence API is already using AI to identify video content. Meta is experimenting with similar detection in Reels.


In other words: **technically, all of this is feasible** — they can scan every uploaded video frame in real time, detecting dumbbells, motorcycle helmets, strollers, pet food.


Yet their actual product capabilities remain at coarse-grained tags:
```
Fitness video → sports_equipment (vague)
Parenting video → baby_products (still vague)
```


Why not go granular: "detected Brand X dumbbells → serve Brand X protein powder ads"?


### Path Dependency: Legacy System Inertia Outweighs Technology


The current mainstream ad buying model looks like this:

```
$1M budget → target "male 30-45" + "tier-1/2 cities" → serve → KPI report
```

This system's strength: **quantifiable, attributable, backed by historical data**. Sales teams can show clients 3 years of case studies: "We delivered 1:8 ROI last year, guaranteed 1:10 this year."

But if we switch to content-understanding-based precision targeting:

```
$1M budget → target "videos containing fitness equipment" → serve → ??? how do we calculate KPI?
```

New problems emerge:
- **Historical data becomes useless**: years of accumulated "audience packages" go to waste
- **Sales team resistance**: they've spent careers selling "gender-age targeting," now they have to pitch "in-frame object recognition"
- **Client education cost**: brands don't know how to buy traffic for "a specific object in a video"

It's analogous to why Baidu didn't pivot to AI — not because of technical inability, but because **search generated tens of billions in annual revenue**. Too risky to disrupt.


ByteDance, Tencent, Google, and Meta face the same dilemma: their existing ad systems, while imperfect, generate hundreds of billions annually. Pivoting means rebuilding the underlying architecture, retraining sales teams, redefining KPIs — the cost is enormous.


### Profit Distribution: Ecosystem Game Theory


This is the deepest layer. If a giant truly achieves hyper-precise content-ad matching, what happens?


Imagine a fitness creator uploads a dumbbell training video. The system detects the dumbbell and automatically inserts a protein powder ad link. How is the profit split?

```
Old model:
Creator adds shopping cart → user buys → platform takes 10%


New model:
AI auto-inserts ad → user buys → platform takes 30% + creator share?
```


**The implications are massive:**
- R&D labs need to coordinate revenue splits with ad sales departments
- Third-party e-commerce affiliates get bypassed
- MCN agencies lose bargaining power
- Content platforms undergo fundamental identity shifts


So this isn't a technology problem — it's a **profit distribution problem**. Decision-makers at these giants see "a few billion more from existing business" vs. "uncertainty from new tech." The former clearly wins.


---


## 3. Big Tech Divergence: Google, TikTok, and Meta's Choices


### Google: The Search Shadow Is Too Large


Google's core formula:
```
User enters keyword → match ad → charge per click
                      ↓
CPC: $2-50 (high-value verticals like finance, healthcare, legal can reach $100+)
Annual profit: ~$70B
```


By comparison, video ad value density is much lower:
```
User watches video → display ad → charge per thousand impressions
                      ↓
CPM: $2-10 (typically halved again for creator revenue share)
Annual profit: ~$10B
```


**Key insight**: Search ad per-conversion value is 5-10× that of video. YouTube, despite its scale, is merely "icing on the cake" compared to search. Investing R&D resources in technology that improves search ad conversion by 1% yields far higher returns than video understanding.


Google Video Intelligence API already identifies video content with AI, but the ultimate goal isn't ad precision — it's **content moderation and recommendation ranking**. Because:
1. Content moderation carries higher risk costs
2. Recommendation ranking directly impacts watch time (KPI)
3. Ad serving stays with the traditional interest-tag system


### TikTok: Closest to a Disruptor, Yet Chose Conservatism


| Metric | 2021 | 2022 | 2023 | 2024E |
|--------|------|------|------|-------|
| Ad Revenue | $10B | $20B | $30B | $45B+ |
| YoY Growth | 100% | 100% | 50% | 50% |


TikTok is growing far faster than other platforms, yet it still hasn't fully opened content-ad precision matching. Three reasons:


#### 1. User Mindset Is Still Forming
Surveys show 72% of users see "TikTok as entertainment," and only 18% are willing to watch shopping ads on TikTok. Launching aggressive content-matched commerce features now could undermine the user experience foundation.


#### 2. E-commerce Infrastructure Is Incomplete
TikTok Shop's US coverage is far below China's. Many countries lack complete logistics and payment systems, brand onboarding willingness is low, and creators can't settle commissions directly. Pushing content-understanding ads aggressively would expose a broken backend (supply chain, payments, customer support — all weak).


#### 3. Founder Preference for "Light Touch"
ByteDance's culture leans "algorithm-driven, human-restrained" — automate where possible, intervene minimally, hire few salespeople. This makes response to complex profit distribution slow, lacking frontline sales feedback loops.


### Meta: Distracted by WhatsApp and Threads


| Metric | 2020 | 2023 | Change |
|--------|------|------|--------|
| Facebook DAU | 2B+ | 2B+ | Flat |
| Instagram DAU | 1.5B | 1.7B | +13% |
| TikTok DAU | 900M | 1.6B | **+78%** |
| Gen Z MAU Share | 35% | 22% | **-13pp** |


Gen Z has already migrated en masse from Facebook to TikTok — an existential threat for Meta. Reels is fundamentally a response to the TikTok threat, not a core growth engine. Priority ranking: WhatsApp Business API > Instagram Shops > Facebook Core > Reels.


Reels sits at fourth place, showing it's not being cultivated internally as a "next-generation traffic gateway." Meta's ad backend is 15 years old, with deeply accumulated advertiser habits, API specifications, and third-party tool integrations. Changing the distribution logic is equivalent to rebuilding the ad system from scratch — more costly than for TikTok. Add post-Cambridge Analytica privacy policy pressure, and any data-collection attempts get amplified through public scrutiny.


---


## 4. Interactive Design: The Key to KPI Tracking


How do you track KPIs? How do advertisers know their money is well-spent? This question is critical — and there are already attempts underway, just progressing slowly.


### Existing Practice Cases


| Platform | Product Form | Interaction | Coverage |
|----------|-------------|-------------|----------|
| **YouTube** | Shoppable Video | Tap product → overlay popup | ~10% of channels |
| **TikTok** | TikTok Shop Tags | Bottom tag + cart redirect | ~5% countries/categories |
| **Instagram** | Shopping Posts | Tap product in image/Reels | ~30% brand accounts |
| **Xiaohongshu** | Notes with product links | Comment or body link | ~40% commerce notes |
| **Taobao Live** | Real-time popup product cards | Auto-popup + countdown | ~90% livestream rooms |


**Key finding**: These features all exist, but coverage is very low.


### Core Obstacle: User Experience vs. Commercialization Balance


**Obstacle 1: "Annoyance Threshold" Is Hard to Quantify**


Experimental data shows interactive lightweight ads outperform forced pre-rolls by 10-20×, but even best practices cause completion rates to drop 0.5-2%. A 1% completion drop leads to a 5% recommendation weight reduction, which then causes a 15% creator traffic decline — reducing quality content. It's a chain reaction platforms are afraid to trigger.


**Obstacle 2: KPI Calculation Complexity Is High**


The new approach raises three problems:
1. **Inventory uncertainty**: AI scanning takes time (seconds to minutes), making it impossible to predict tomorrow's eligible video volume
2. **Multi-advertiser competition**: one video may contain multiple products — how to allocate ad slots?
3. **Missing real-time bidding system**: traditional Ad Exchanges are designed for "predefined audiences," not "dynamic content libraries"


**Obstacle 3: Creator Willingness Varies**


Top creators reject AI auto-inserted ads (revenue too low, persona risk), while mid-to-small creators might accept — creating an ecosystem gap.


### Possible Solutions


**Solution 1: Creator Toggle (Gradual Adoption)**
Let creators decide whether to enable AI ad placement — opt-in gives creators control, platform data accumulates more authentically.


**Solution 2: KPI Redefinition**
Since traditional CPM/CPC don't map directly, design new metric systems: VCPM (Video Content Per Mille), Object-CPC, Scene-Relevance Score, Conversion-Lookback Window. e.g. `ad_impression_value = base_cpm * object_relevance * engagement`.


**Solution 3: Hybrid Transition Period**
Run both systems simultaneously, giving brands choice: audience-package targeting (traditional, mature, stable) or content-package targeting (new, precise, requires AI scan wait).


---


## 5. Auction Mechanism Design: The Monetization Model Platforms Love Most


On the question of multiple advertisers competing for the same video inventory — the answer is clear: **bidding**.


### Core Insight: Why Do Platforms Love Bidding?


Bidding = profit maximization + risk minimization. For a new business like AI content-understanding ads, what platforms want most isn't "rapid adoption" but "profit validation." Bidding satisfies both.


### Design A: Creator Tiered Auction Pools


```python
ad_inventory_pool = {
    'tier_1_top_creators': {  # followers > 1M
        'video_count': 1000,
        'avg_views_per_video': 500000,
        'base_bid_floor': $50 per thousand impressions,
        'priority': 'brand_campaigns'
    },
    'tier_2_mid_creators': {  # followers 100K-1M
        'video_count': 10000,
        'avg_views_per_video': 50000,
        'base_bid_floor': $20 per thousand impressions,
        'priority': 'mid_brand_campaigns'
    },
    'tier_3_small_creators': {  # followers < 100K
        'video_count': 100000,
        'avg_views_per_video': 5000,
        'base_bid_floor': $5 per thousand impressions,
        'priority': 'performance_campaigns'
    }
}
```


Bidding flow:
1. Brand submits budget + target audience
2. AI scans video library → outputs eligible video list
3. Layer by creator tier, enter corresponding auction pool
4. Real-time bidding (RTB), highest bidder wins
5. Auto-insert clickable product link → data feedback → billing


### Design B: Cross-Tier Hybrid Auction


Beyond tiering, build a dynamic pool with hybrid weighted auction rules: consider not just bid price but also video quality, preventing traffic from going entirely to ad-farms. Brands can specify "prioritize Tier 1" or "full coverage," with base price floating based on daily inventory.


### Why Haven't Giants Done This Yet?


Two core reasons:
1. **Existing ad systems are built on "audience packages"** — switching costs are enormous
2. **Top creators' relationship networks are too strong** — exclusive partnerships lock in top creators; an auction model would strip MCNs of bargaining power


---


## 6. Top Creator Privileges: Balancing Creative Control and Auction Mechanisms


This is the through-line connecting all the obstacles above — if top creators won't buy in, the entire model can't move. Creator control must be at the center of the design.


### Core Tension: Persona Protection vs. Commercialization Revenue


| Concern | Real Reason | Impact |
|---------|------------|--------|
| **Brand mismatch** | "My fans see me as a hardcore reviewer — suddenly inserting a beauty product destroys my persona" | Fan loss |
| **Ad overload** | "Three product links in one video will turn viewers off" | Completion drop |
| **Passive pricing** | "I wanted $50K, the system only offers me $7.5" | Revenue loss |
| **Data black box** | "How many sold, how many clicked, is the math right?" | Trust deficit |


### Solution: Tiered Authorization System


```python
creator_privilege_level = {
    'tier_1_premium': {  # top creators
        'ad_selection_mode': 'whitelist_approve',
        'max_ads_per_video': 3,
        'revenue_share': '80% to creator, 20% platform',
        'opt_out_any_time': True
    },
    'tier_2_standard': {  # mid-tier creators
        'ad_selection_mode': 'category_filter',
        'max_ads_per_video': 2,
        'revenue_share': '70% to creator, 30% platform',
        'opt_out_any_time': False
    },
    'tier_3_auto': {  # small creators
        'ad_selection_mode': 'full_auto',
        'max_ads_per_video': 1,
        'revenue_share': '60% to creator, 40% platform',
        'opt_out_any_time': False
    }
}
```


### Operational Flow


**Step 1: Creator Sets Preferences**

```json
{
  "creator_id": "top_fitness_blogger",
  "ad_preferences": {
    "approved_brands": ["Nike", "GymShark", "MyProtein"],
    "blocked_categories": ["diet_pills", "cosmetics", "alcohol"],
    "max_ad_density": 0.3,
    "preferred_placement": "end_screen_only"
  },
  "bid_fallback": {
    "auto_accept_brands_if_bid_exceeds": "$50 CPM"
  }
}
```


Key point: not fully passive AI allocation — whitelist mechanism protects persona, final veto retained.


**Step 2: Ad Auction + Creator Filtering**

```
Ad request arrives → AI identifies object (dumbbell) → candidate ad list (5 brands)
                    ↓
Filter by creator preferences
├─ Brand A (not on whitelist) → skip
├─ Brand B (on whitelist, $40 CPM) → enter auction pool
├─ Brand C (not on whitelist, $60 CPM) → trigger manual approval request
└─ Brand D (not on whitelist, $30 CPM) → reject

Winner → insert ad slot → creator receives revenue report
```


**Step 3: Real-time Feedback Loop**


Adjust ad strategy in real time based on CTR and conversion rates. Underperforming ads auto-replaced, ensuring optimal overall ROI.


---


## 7. The Ultimate Scenario: Cut Out the Middlemen, Creators Take Commission Directly


This is the boldest conjecture I want to explore in this entire piece.


### Status Quo: A Tangled Profit Chain


The current e-commerce influencer model looks like this:

```
Brand → Agency → MCN → Creator → Platform → User
         ↓    ↓      ↓       ↓     ↓
      20%   15%    10%      5%    10%

Total extraction: ~60%
```


In other words, when a brand spends ¥100 on promotion, only about ¥40 reaches the creator. This is why many quality content creators avoid ads — the ROI is terrible for them.


### New Vision: Platform Direct-to-Creator


If AI can truly achieve real-time content understanding and ad placement, what business model emerges?

```
Creator uploads video → AI auto-matches relevant product → generates tracked ad slot → user purchases → platform settles commission directly to creator
```


In this model:
- **Brands** pay once per sale (CPS)
- **Platform** takes 10-20% service fee (replacing all intermediate layers)
- **Creators** receive 70-80% direct share


Key shifts: high automation — no need for creators to manually select products; high transparency — every transaction traceable; incentive alignment — creators more willing to share genuine experiences.


### Why Hasn't This Emerged Yet?


By all logic, this should be a win-win-win. The answer remains: **no one wants to be the first to stand up as a target**. Brands are accustomed to negotiating via MCNs. MCNs don't want to surrender their middleman cut. Platforms worry "direct collaboration" will disrupt existing channel management. Creators fear income instability "post-abandonment." It requires a sufficiently powerful external forcing function — like AI costs dropping enough that automation feasibility surpasses manual negotiation value.


---


## 8. Rational Analysis: Can Three-Way Win-Win Be Achieved?


If this scenario actually materializes, can platforms, creators, and users all win?


My assessment: **theoretically yes, practically challenging**. Let's analyze each stakeholder:


### Platforms: The Biggest Beneficiaries


| Dimension | Current | New Model | Change |
|-----------|---------|-----------|--------|
| **Revenue** | CPM $5-10 | CPM $15-30 | **+200-300%** |
| **User stickiness** | Ad-driven churn | Precision ads reduce churn | Improved |
| **Ecosystem control** | Dependent on MCNs | Direct creator relationship | Strengthened |
| **Tech moat** | Undifferentiated | AI understanding capability | Moat built |


**Risks**:
- Misidentification causing user backlash
- Data leaks triggering compliance issues
- Over-commercialization destroying community atmosphere


### Creators: Deeply Divided


| Type | Expected Revenue | Risk | Attitude |
|------|-----------------|------|----------|
| **Top creators** | High (bargaining power) | Persona risk | ⚠️ Cautious |
| **Mid-tier creators** | Medium-high | Medium | ✅ Open |
| **Small creators** | Low (fierce competition) | High (auto low-price competition) | ❌ Resistant |


**Core issues**:
- Top creators fear "passive pricing" eroding bargaining power
- Mid-tier creators welcome monetization but fear tonal impact
- Small creators fear becoming "ad laborers"


**My recommendation**: Top creators must be given sufficient control (whitelist, veto), or there will be collective resistance.


### Users: Short-Term Pain, Long-Term Gain


| Dimension | Current | New Model | Change |
|-----------|---------|-----------|--------|
| **Ad intrusion** | Skippable forced pre-roll | Lightweight interactive ads | Improved |
| **Ad relevance** | Generic targeting | Content-matched | Major improvement |
| **Decision support** | None | Genuine usage feedback | Valuable |
| **Privacy concerns** | Medium | High (deep profiling) | Worse |


**Key conclusions**:
- If ads are well-designed (lightweight, closable, valuable), users won't strongly resist
- But excessive data collection for ads will trigger privacy backlash


### Synthesis: Prerequisites for Win-Win


For genuine three-way win-win, these conditions must be met:

1. **Transparency**: clearly inform users of ad sourcing, provide opt-out
2. **Control**: creators have the right to select/reject specific ads
3. **Fair revenue split**: platform and intermediary cuts must not be excessive
4. **Content quality first**: never sacrifice content for ad revenue
5. **Privacy boundaries**: clearly define which data can and cannot be used


**Without the above, "win-win" is a false promise.**


---


## 9. Who Would Buy an Independent SaaS?


This is the most critical practical question — if you build an independent SaaS, who pays?


### Potential Client Type Analysis


#### Type A: Vertical Community Apps (Ideal)


| Feature | Example | Pain Point | Willingness to Pay |
|---------|---------|------------|-------------------|
| User scale | 500K-10M DAU | Low ad conversion | ✅ High |
| Industry | Fitness, auto DIY, pets | Generic platforms not precise enough | ✅ High |
| Tech capability | Limited in-house AI | Need external service | ✅ High |
| Revenue share constraints | Don't want 30% to giants | Cost reduction | ✅ High |


**Examples**: Keep (fitness app), Autohome forums, Boqii (pet community).


#### Type B: Regional Livestream Platforms


| Feature | Example | Pain Point | Willingness to Pay |
|---------|---------|------------|-------------------|
| Market scale | Regional/national | Can't compete with global platforms | ✅ Medium |
| Localization advantage | Language/culture fit | Giants don't understand local | ✅ Medium |
| Revenue share sensitivity | Don't want 30% cut | Cost reduction | ✅ High |


**Examples**: Naver Live (Korea), ShareChat (India), Southeast Asian local livestream platforms.


#### Type C: Creator Alliances / MCNs (Potential but High Resistance)

MCNs introducing this SaaS effectively weaken their own bargaining power as middlemen. **Unless you can prove this earns more than the existing model.**


#### Type D: Small-to-Mid E-Commerce Platforms (Long Tail)


| Feature | Example | Pain Point | Willingness to Pay |
|---------|---------|------------|-------------------|
| E-commerce scale | < $100M GMV | Limited ad budget | ⚠️ Medium |
| Own content platform | Brand-owned video site | Need precise reach | ✅ Medium |
| Tech resources | Minimal | External dependency | ✅ High |


### Recommended Target Client Sequence


| Priority | Client Type | Rationale |
|----------|------------|-----------|
| **1** | Vertical community apps | High willingness + clear pain points + low competition |
| **2** | Regional livestream platforms | Anti-giant + needs localized solution |
| **3** | Small-mid e-commerce platforms | Limited budget but real demand |
| **4** | MCN agencies | Highest resistance but biggest upside if cracked |


### Pricing Strategy


```json
{
  "tier_1_basic": {
    "price": "$500/month",
    "quota": "100 hours video processing",
    "features": ["video object detection", "category matching"]
  },
  "tier_2_pro": {
    "price": "$2000/month",
    "quota": "500 hours",
    "features": ["add clickable links", "conversion tracking API", "basic bidding system"]
  },
  "tier_3_enterprise": {
    "price": "$10000+/month",
    "quota": "unlimited",
    "features": ["on-premise deployment", "custom model training", "white-label solution"]
  }
}
```


**Comparative advantage**:
- 5-10× cheaper than Google Cloud Video Intelligence API ($1000+/month)
- 10-50× cheaper than an in-house team ($100K+/year)
- Lower take rate (15-20%) than giant platform cuts (30%)


---


## 10. Future Outlook: Three Possible Time Windows


### 2025-2026: Edge Computing Proliferation


Lightweight models become common on mobile and edge devices. Video understanding costs drop to 1/10 of today. Small-to-mid platforms can experiment with content-ad precision matching.


**Key metrics**: per-hour processing cost ≤ $0.10, accuracy ≥ 90%, latency ≤ 100ms.


### 2027-2028: Vertical Scenario Explosion


Dedicated AI ad platforms emerge in verticals like fitness, auto DIY, and pet supplies. Accuracy exceeds the industry average, beginning to squeeze general-platform share.


**Key signals**: first $10M+ funded vertical AI ad platform; top MCNs begin adopting AI placement tools; regulators issue AI ad transparency standards.


### 2029-2030: Full-Chain Automation Maturity


AI not only identifies video content but auto-generates ad creative adapted to different contexts (dynamic creative optimization) and adjusts strategy based on real-time feedback. The middleman role further weakens. Creator-to-brand direct connection becomes the norm.


**Key signals**: content-ad precision matching becomes mainstream (≥50% of video ads); MCN numbers significantly decline; platform take rates drop to 10-15%.


---


## Conclusion: Technology's Endgame Is Business Victory


Returning to the original question: **why haven't WeChat, ByteDance, Google, TikTok, and Meta done this?**


The answer may be disappointing — not because they can't, but because **the existing business structure is making them money**. Any technology that breaks the rules encounters resistance from vested interests, unless the gains from the new rules are large enough to cover transition costs.


My conjecture: **the cost curve will breach the threshold first**. When video understanding costs drop to a critical point (say, 1% of today's), edge computing solutions will become more attractive than centralized ones — and that's when disruption happens.


I personally believe the advertising of the future won't be "forced promotion" + "skip button." It will be **the natural fusion of content and commerce** — like water seeping into soil, invisible yet everywhere. When we look back at today's ad formats from that future, it will feel like how we now view newspaper classifieds: **inefficient and full of noise**.


As for who will realize this vision first? My assessment: **vertical independent SaaS players will land before the giants**, because their boats are small enough to turn, and they carry no historical baggage.


*This article is based on systematic analysis of the advertising industry and technical feasibility research. It does not represent any platform's position. Discussion, rebuttal, and additions are welcome.*
