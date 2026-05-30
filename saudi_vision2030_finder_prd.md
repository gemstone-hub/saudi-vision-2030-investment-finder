# Product Requirements Document
## Saudi Arabia Vision 2030 Investment Finder

**Product Name:** Saudi Vision 2030 Investment Finder
**Version:** 1.0
**Author:** Christian
**Platform:** Antigravity
**Last Updated:** May 2026

---

## 1. Overview

### 1.1 Purpose
A free, standalone web tool that asks a Saudi Arabia property investor five questions about their investment profile and recommends the best matching Vision 2030 Giga Project for their specific situation. The tool serves as a lead magnet — investors get a personalised, genuinely useful recommendation, and Christian gets qualified conversations with people who are actively thinking about Saudi real estate investment.

### 1.2 Problem Statement
Saudi Arabia's Vision 2030 Giga Projects represent over $700 billion in planned investment across five major developments — NEOM, Red Sea Global, Diriyah Gate, Qiddiya, and ROSHN. An investor, developer, or proptech founder trying to understand which project fits their profile has no fast, personalised way to find out. The gap between curiosity and conviction costs platforms, advisors, and developers qualified leads every day. This tool closes that gap in under two minutes.

### 1.3 Target Users
- Saudi Arabia property investors evaluating Vision 2030 opportunities
- International investors researching GCC real estate entry points
- Proptech founders and platform builders in Saudi Arabia
- Real estate developers and advisors working within the Giga Project ecosystem
- Saudi Premium Residency applicants evaluating qualifying investments

### 1.4 Unique Value
No tool like this exists publicly. Every investor researching Vision 2030 Giga Projects currently reads long reports, browses multiple websites, and still arrives at conversations with advisors without a clear sense of which project fits their situation. This tool does that work in five questions.

### 1.5 Success Metrics
- Time to result: under 90 seconds from first question to recommendation
- CTA click rate: target 10%+ of users who complete the quiz
- Session engagement: average user completes all five questions
- Mobile usability: fully functional on screens 375px and above
- Zero errors: no JavaScript errors in any supported browser

---

## 2. The Five Questions

Questions are displayed one at a time. Never all at once. Each question shows its number out of five.

### Question 1 — Investment Horizon
**Text:** What is your investment horizon?

| Option value | Display label |
|---|---|
| short | 1 to 3 years — I want returns quickly |
| medium | 3 to 7 years — balanced approach |
| long | 7 to 15 years — I am building long-term wealth |
| very_long | 15+ years — generational investment |

### Question 2 — Investment Budget
**Text:** What is your investment budget?

| Option value | Display label |
|---|---|
| small | Under SAR 500,000 |
| mid | SAR 500,000 to SAR 2 million |
| large | SAR 2 million to SAR 10 million |
| xlarge | Over SAR 10 million |

### Question 3 — Type of Return
**Text:** What type of return matters most to you?

| Option value | Display label |
|---|---|
| yield | Rental income — I want steady cash flow |
| capital | Capital appreciation — I want the asset to grow |
| both | Both yield and capital growth |
| vision | Strategic positioning in Vision 2030 |

### Question 4 — Risk Appetite
**Text:** How do you think about risk?

| Option value | Display label |
|---|---|
| low | Conservative — I want proven stable investments |
| medium | Moderate — balanced risk and reward |
| high | Growth-oriented — I can accept volatility for higher returns |
| vhigh | Visionary — I want to be part of something historic |

### Question 5 — Sector Preference
**Text:** Which sector excites you most?

| Option value | Display label |
|---|---|
| residential | Residential communities and housing |
| tourism | Luxury tourism and hospitality |
| entertainment | Entertainment, sports and culture |
| future | Futuristic cities and deep technology |

---

## 3. The Five Giga Projects

All project data must be stored as JavaScript objects. Never hardcoded into HTML.

### 3.1 NEOM

```
name: NEOM
sub: The Line, Trojena, Oxagon, Sindalah
total_value: $500 billion
risk: High to visionary
ideal_horizon: 7 to 20+ years
min_investment: SAR 500K+
pipeline: $500B total project value
description: A $500 billion futuristic megacity on the Red Sea coast
with a special tax and regulatory framework for foreign investors.
NEOM is designed for those who want to be part of the most ambitious
development project in modern history. Sub-projects include The Line,
Trojena (mountain ski resort), Oxagon (floating industrial city), and
Sindalah (luxury island, operational since late 2024).
best_for: Futuristic sector, visionary risk, long to very long horizon,
large to xlarge budget, capital appreciation or Vision 2030 positioning.
```

### 3.2 Red Sea Global

```
name: Red Sea Global
sub: Luxury tourism, 28,000 km coastline, 50+ hotels
total_awarded: $14B+
risk: Moderate
ideal_horizon: 3 to 10 years
min_investment: SAR 2M+
pipeline: $14B+ awarded, Phase 1 operational
description: The world's most ambitious luxury tourism destination
spanning 28,000 km of pristine Red Sea coastline. Phase 1 resorts
are already open and welcoming guests. Investors benefit from a proven
hospitality model, strong international brand partnerships, and Saudi
Arabia's rapidly growing inbound tourism market targeting 150 million
visits annually by 2030.
best_for: Tourism sector, moderate risk, medium to long horizon,
large to xlarge budget, both yield and capital growth.
```

### 3.3 Diriyah Gate

```
name: Diriyah Gate
sub: Historic Riyadh, culture, heritage and F&B
commissioned: $14.5B
pipeline: $45.6B
risk: Low to moderate
ideal_horizon: 3 to 10 years
min_investment: SAR 500K to SAR 10M+
pipeline_display: $45.6B pipeline
description: Saudi Arabia's first capital reimagined as a world-class
cultural and heritage destination on the edge of Riyadh. With $14.5
billion commissioned and $45.6 billion in pipeline, Diriyah is one of
the most advanced Giga Projects in delivery progress. The Bujairi
Terrace district has been operational since 2022. Combining Najdi
architectural heritage with international hospitality brands across
F&B, culture, and accommodation.
best_for: Tourism or culture sector, low to moderate risk, medium
horizon, mid to large budget, both yield and capital.
```

### 3.4 Qiddiya

```
name: Qiddiya
sub: Entertainment city near Riyadh, sports and culture
gdp_contribution: $4.53B by 2030
residential_units: 4,000 by 2025, 11,000 by 2030
jobs: 57,000 new jobs
risk: Moderate
ideal_horizon: 3 to 8 years
min_investment: SAR 300K to SAR 5M
pipeline_display: $4.53B GDP contribution by 2030
description: The entertainment capital of Saudi Arabia, located near
Riyadh. Qiddiya is building 4,000 residential units by 2025 and 11,000
by 2030, expected to contribute $4.53 billion to Saudi GDP and create
57,000 new jobs. Home to the world's first Dragon Ball theme park and
a major Formula 1 racing circuit. The project for investors who believe
in the lifestyle transformation of the Kingdom.
best_for: Entertainment sector, moderate risk, short to medium horizon,
small to mid budget, rental yield focus.
```

### 3.5 ROSHN

```
name: ROSHN
sub: 400,000+ homes by 2030, nationwide communities
homes_target: 400,000+ by 2030
ownership_target: 70% Saudi home ownership
communities: Sedra, Alarous, and expanding
risk: Low to moderate
ideal_horizon: 1 to 7 years
min_investment: SAR 200K to SAR 3M
pipeline_display: 400,000+ homes by 2030
description: Saudi Arabia's national residential developer and the most
accessible entry point into Vision 2030 real estate. ROSHN is targeting
70% home ownership across the Kingdom, already delivering communities
at scale including Sedra and Alarous. Foreign developers are actively
invited to participate. The lowest-risk Giga Project with the clearest
residential return model and the shortest path to delivered product.
best_for: Residential sector, low to moderate risk, short to medium
horizon, small to mid budget, rental yield focus.
```

---

## 4. Scoring Algorithm

The scoring function runs entirely in JavaScript on the client side. It must produce a score for each of the five Giga Projects based on the five answers. Higher score equals better match.

### 4.1 Scoring Table

**Horizon (answers.horizon):**

| Answer | NEOM | Red Sea | Diriyah | Qiddiya | ROSHN |
|--------|------|---------|---------|---------|-------|
| very_long | +3 | 0 | 0 | 0 | 0 |
| long | +2 | +1 | 0 | 0 | 0 |
| medium | 0 | +2 | +2 | +2 | 0 |
| short | 0 | 0 | 0 | +1 | +3 |

**Budget (answers.size):**

| Answer | NEOM | Red Sea | Diriyah | Qiddiya | ROSHN |
|--------|------|---------|---------|---------|-------|
| xlarge | +3 | 0 | 0 | 0 | 0 |
| large | +1 | +2 | +2 | 0 | 0 |
| mid | 0 | 0 | +2 | +2 | +2 |
| small | 0 | 0 | 0 | +1 | +3 |

**Return type (answers.type):**

| Answer | NEOM | Red Sea | Diriyah | Qiddiya | ROSHN |
|--------|------|---------|---------|---------|-------|
| vision | +3 | 0 | +1 | 0 | 0 |
| capital | +2 | +1 | 0 | 0 | 0 |
| both | 0 | +2 | +2 | 0 | 0 |
| yield | 0 | 0 | 0 | +2 | +2 |

**Risk (answers.risk):**

| Answer | NEOM | Red Sea | Diriyah | Qiddiya | ROSHN |
|--------|------|---------|---------|---------|-------|
| vhigh | +3 | 0 | 0 | 0 | 0 |
| high | +2 | +1 | 0 | 0 | 0 |
| medium | 0 | +2 | +2 | +2 | 0 |
| low | 0 | 0 | +1 | 0 | +3 |

**Sector (answers.sector):**

| Answer | NEOM | Red Sea | Diriyah | Qiddiya | ROSHN |
|--------|------|---------|---------|---------|-------|
| future | +3 | 0 | 0 | +1 | 0 |
| tourism | 0 | +3 | +1 | 0 | 0 |
| entertainment | +1 | 0 | 0 | +3 | 0 |
| residential | 0 | 0 | 0 | +1 | +3 |

### 4.2 Result Determination

Sort all five projects by total score descending. The project with the highest score is the best match. The project with the second highest score is also worth exploring.

If two projects tie on score the tiebreaker is sector alignment — the project whose sector matches the investor's sector answer wins.

### 4.3 Validation Tests

The following extreme profiles must produce the correct results:

| Profile | Expected best match |
|---------|-------------------|
| All NEOM answers (very_long, xlarge, vision, vhigh, future) | NEOM |
| All ROSHN answers (short, small, yield, low, residential) | ROSHN |
| All Red Sea answers (long, large, both, high, tourism) | Red Sea Global |
| All Qiddiya answers (medium, mid, yield, medium, entertainment) | Qiddiya |
| All Diriyah answers (medium, large, both, low, tourism) | Diriyah Gate |

---

## 5. User Interface and Interactions

### 5.1 Quiz Flow

**Entry state:**
Show question 1 with no answer selected. Next button is disabled.

**Per question state:**
- Question number shown as "Question X of 5"
- Question title prominent
- Four answer options in a two-column grid
- Selected answer is visually highlighted in gold/amber
- Next button disabled until an option is selected
- Back button hidden on question 1, visible on questions 2 through 5
- On question 5 the Next button text changes to "See my match"

**Changing answers:**
If the user presses Back and selects a different answer, their previous selection for that question is cleared and the new selection is stored. When they reach the result screen the scoring recalculates based on current answers.

**Progress indicator:**
Five dots displayed horizontally at the top of the quiz. Dots for completed and current questions are filled gold. Future question dots are empty and muted. Transitions smoothly as the user moves forward and backward.

### 5.2 Result Screen

Displayed after the fifth question is answered and See my match is clicked.

**Header line:**
"Based on your profile" — small, muted, above the cards.

**Best match card (primary):**
- Badge: "Best match" — gold/amber background, dark text
- Project name — large, 22 to 24px, font-weight 500
- Sub-project line — 13px muted
- Description — 14px body text, full paragraph
- Four stat pills in a row: Minimum investment, Ideal horizon, Risk profile, Scale/pipeline value
- Card has a 2px gold/amber border to distinguish it from secondary card

**Also worth exploring card (secondary):**
- Badge: "Also worth exploring" — neutral background, muted text
- Project name
- Sub-project line
- Description — full paragraph
- No stat pills
- Standard 0.5px border

**CTA button:**
- Full width below both cards
- Text: "Book a free 20-minute call ↗"
- Link: https://cal.com/enwere-christian-qip6n0/30min
- Opens in new tab
- Gold/amber background, dark text, prominent

**Restart link:**
- Below CTA button
- Text: "Start over"
- Clicking resets all answers and returns to question 1

---

## 6. Design Requirements

### 6.1 Aesthetic Direction
Saudi Vision 2030 premium. Bold, warm, prestigious. This tool represents a $700 billion investment programme. It must feel like it belongs on the website of a sovereign wealth fund or a luxury real estate advisor — not a generic startup, not a basic quiz tool.

### 6.2 Color Palette

| Element | Color direction |
|---------|---------------|
| Page background | Deep desert sand (#1A1208) or rich dark navy (#0A0F1E) |
| Card background | Slightly lighter than page bg |
| Primary accent | Gold (#C9A84C) or warm amber (#E0A84C) |
| Selected answer border and text | Gold accent |
| Selected answer background | Warm gold tint at low opacity |
| Primary text | Off-white (#F0EDE8) |
| Secondary text | Warm muted gray (#8B8680) |
| Stat pill background | Warm surface, slightly lighter than card |
| Best match card border | 2px gold accent |
| CTA button | Gold background, dark text |
| Progress dot filled | Gold accent |
| Progress dot empty | Low contrast muted circle |

Do not use blue, purple, or cool-toned colors anywhere. The palette is entirely warm — gold, amber, cream, sand, dark navy or charcoal.

### 6.3 Typography

Load both fonts from Google Fonts via a link tag:

- **Headings and question titles:** Tajawal or Cairo — a premium Arabic-compatible sans-serif that respects the Saudi context of the tool
- **Body and UI:** Inter or DM Sans — clean and highly readable at small sizes

| Element | Size | Weight |
|---------|------|--------|
| Question title | 20 to 24px | 500 |
| Answer option text | 14px | 400 |
| Stat value | 16px | 500 |
| Stat label | 11px uppercase, 0.08em letter-spacing | 400 |
| Project name (result) | 22px | 500 |
| Sub-project line | 13px | 400 |
| Description paragraph | 14px | 400, line-height 1.7 |
| Badge text | 11px | 500 |
| CTA button | 15px | 500 |

### 6.4 Answer Option Buttons

| State | Treatment |
|-------|-----------|
| Default | Dark surface, 0.5px muted border, warm gray text |
| Hover | Slightly lighter surface, border becomes more visible |
| Selected | 1.5px gold border, warm gold tint background, gold text |

Transition: all 150ms ease on color, background, and border-color.

Minimum height: 52px on desktop, 56px on mobile (touch target).

Two-column grid layout. If a question has an odd number of options the last option spans full width.

### 6.5 Progress Dots

Five dots in a horizontal row. 8px diameter circles. 8px gap between them.

- Empty dot: `background: rgba(201, 168, 76, 0.2)` — very faint gold
- Filled dot: `background: #C9A84C` — solid gold
- Transition: background-color 200ms ease

### 6.6 Animations and Motion

| Interaction | Animation |
|-------------|-----------|
| Question transition (forward) | Fade out current, fade in next, 200ms |
| Question transition (back) | Same fade |
| Result screen reveal | Fade in from opacity 0, 400ms |
| Answer selection | Instant color change, no delay |
| Progress dot fill | 200ms background transition |
| CTA button hover | Opacity 0.88, 150ms |
| Page load | No loading animation needed — renders instantly |

No layout shifts at any point. All elements maintain their position during transitions.

### 6.7 Responsive Design

**Desktop (600px+):**
Full layout. Answer options in two-column grid. Stat pills in a single row.

**Mobile (375px to 599px):**
Answer options in single-column grid, full width. Stat pills wrap to two columns. Project name slightly smaller (18px). All buttons full width. Progress dots centered. Back and Next buttons in a row, Next takes remaining space.

**Touch:**
All interactive elements minimum 44px touch target height. Answer buttons 56px minimum on mobile.

---

## 7. Technical Requirements

### 7.1 Stack
- Single HTML file — all CSS and JavaScript inline
- No frameworks, no build tools, no npm, no dependencies
- Vanilla JavaScript only
- Google Fonts loaded via `<link>` tag in `<head>`
- Must work in Chrome, Safari, Firefox, and Edge

### 7.2 Data Architecture
All Giga Project data stored as a JavaScript object at the top of the script block:

```javascript
var projects = {
  NEOM: { name, sub, description, min_investment, horizon, risk, pipeline },
  RedSea: { ... },
  Diriyah: { ... },
  Qiddiya: { ... },
  ROSHN: { ... }
}
```

All question data stored as a JavaScript array:

```javascript
var questions = [
  { id, title, options: [{ value, label }] },
  ...
]
```

### 7.3 State Management
Single `answers` object stores current selections:

```javascript
var answers = {}
```

Keys are question IDs (horizon, size, type, risk, sector). Values are option values. When user goes back and changes an answer the key is overwritten with the new value. Scoring reruns on every result screen render.

### 7.4 Scoring Function
Pure JavaScript function that takes the `answers` object and returns a score object:

```javascript
function score(answers) {
  var s = { NEOM: 0, RedSea: 0, Diriyah: 0, Qiddiya: 0, ROSHN: 0 }
  // apply weights per answer
  return s
}
```

Sort result: `Object.keys(s).sort((a,b) => s[b] - s[a])`

### 7.5 URL State (Version 1.1 — out of scope for v1.0)
Encode answers as query parameters so results can be shared and reloaded.

### 7.6 Performance
- First paint under 1 second on 4G mobile
- All five questions and all project data loaded on initial render, no async calls needed
- Quiz interactions feel instant — no perceivable lag

### 7.7 Accessibility
- All answer buttons are native `<button>` elements
- Progress dots have `aria-label` describing current progress
- Question title is wrapped in an appropriate heading element
- Color is never the only way information is conveyed — selected state uses both color and a checkmark or border change
- Focus states visible on all interactive elements
- Page has a meaningful `<title>` and `<meta description>`

---

## 8. Content

### 8.1 Page Title
Saudi Arabia Vision 2030 Investment Finder

### 8.2 Meta Description
Discover which Saudi Arabia Vision 2030 Giga Project matches your investor profile. Five questions, instant personalised recommendation. NEOM, Red Sea, Diriyah, Qiddiya, or ROSHN.

### 8.3 Tool Header
**Headline:** Which Vision 2030 project fits your investor profile?
**Subheadline:** Answer five questions and find your match across NEOM, Red Sea Global, Diriyah, Qiddiya, and ROSHN.

### 8.4 CTA Section
**Button text:** Book a free 20-minute call ↗
**Link:** https://cal.com/enwere-christian-qip6n0/30min

### 8.5 Footer Disclaimer
```
This tool provides general guidance based on publicly available
information about Saudi Arabia's Vision 2030 Giga Projects. Results
are indicative only and do not constitute financial or investment advice.
Consult a qualified investment advisor before making any investment
decisions. Project details, timelines, and investment structures may
change. Data sourced from PIF, Knight Frank Saudi Arabia Giga Projects
Report 2025, and official project sources.
```

---

## 9. Future Versions (Out of Scope for v1.0)

- **Arabic language toggle** — full Arabic translation of all questions, options, and results. The font choice of Tajawal or Cairo makes this straightforward to add later.
- **Email capture** — optional email field on result screen: "Get this recommendation by email." Requires backend.
- **PDF export** — branded PDF of the investor profile and recommendation.
- **Comparison mode** — show all five projects scored against each other with the investor's profile highlighted.
- **Saudi Premium Residency calculator** — add a module showing whether the recommended project qualifies for Saudi Premium Residency (minimum SAR 4 million investment required).
- **Embed code** — iframe snippet for real estate platforms and proptech companies to embed the tool on their own site.
- **Analytics integration** — track which projects are most recommended, which answers are most common, and CTA click rate.

---

## 10. Acceptance Criteria

The build is complete when every item below is confirmed:

- [ ] Tool header displays correctly with headline and subheadline
- [ ] All five questions display correctly one at a time
- [ ] All answer options are present and exactly match Section 2
- [ ] Two-column grid for answer options on desktop
- [ ] Single-column layout on mobile 375px
- [ ] Next button disabled until an answer is selected on every question
- [ ] Back button absent on question 1
- [ ] Back button present and functional on questions 2 through 5
- [ ] Changing an answer via Back correctly updates the stored answer
- [ ] Final question button text reads "See my match"
- [ ] Progress dots update correctly moving forward and backward
- [ ] Scoring function passes all five extreme profile tests from Section 4.3
- [ ] Best match card shows name, sub-project, description, and all four stat pills
- [ ] Also worth exploring card shows name, sub-project, and description
- [ ] Best match card has gold/amber 2px border
- [ ] Badge colors correct — gold for best match, neutral for secondary
- [ ] CTA button links to https://cal.com/enwere-christian-qip6n0/30min
- [ ] CTA button opens in new tab
- [ ] Restart link resets all answers and returns to question 1
- [ ] Footer disclaimer is present
- [ ] Page title and meta description are set
- [ ] Color palette is entirely warm — no blue, purple, or cool tones anywhere
- [ ] Typography uses Tajawal or Cairo for headings, Inter or DM Sans for body
- [ ] Answer buttons minimum 56px height on mobile
- [ ] Question transitions animate smoothly
- [ ] Result screen fades in on reveal
- [ ] No JavaScript errors in browser console
- [ ] Tested and working in Chrome and Safari

---

*End of PRD v1.0*
