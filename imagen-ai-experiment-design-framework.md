# Imagen AI - Experiment Design & Testing Framework
## Phase 4: Hypothesis Testing & Validation

*Based on Research Methodology from Next Capability Research Plan*  
*Framework: Lean Experimentation + Continuous Discovery*  
*Date: December 5, 2025*

---

## Executive Summary

This document provides a comprehensive experiment design framework for validating Imagen AI's next capability expansion. Following the principle of "test cheap before building expensive," we outline specific experiments, success metrics, and decision criteria for each critical assumption.

**Core Principle:** Run the smallest experiment that gives us the evidence we need to move forward with confidence.

---

## Experiment Philosophy

### The Experiment Hierarchy

```
EXPERIMENT HIERARCHY (Fastest → Slowest)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

LEVEL 1: HOURS
────────────────────────────────────────────────────────────────────────────────
│ One-Question Survey │ Data Mining │ Desk Research │
│ Send to 500 users   │ Check analytics │ Review competitor data │
│ Results in 24 hours │ Immediate insights │ Immediate insights │
────────────────────────────────────────────────────────────────────────────────

LEVEL 2: DAYS
────────────────────────────────────────────────────────────────────────────────
│ Customer Interviews │ Fake Door Test │ Unmoderated Usability │
│ 5-10 interviews     │ Landing page + CTA │ Maze/UsabilityHub │
│ 3-5 days            │ 3-7 days │ 2-3 days │
────────────────────────────────────────────────────────────────────────────────

LEVEL 3: WEEKS
────────────────────────────────────────────────────────────────────────────────
│ Smoke Test │ Wizard of Oz │ Pricing Research │
│ Waitlist signup │ Manual delivery │ Van Westendorp │
│ 1-2 weeks │ 2-4 weeks │ 2-3 weeks │
────────────────────────────────────────────────────────────────────────────────

LEVEL 4: MONTHS
────────────────────────────────────────────────────────────────────────────────
│ Concierge MVP │ Beta Launch │ A/B Test │
│ Manual backend │ 50 users │ Feature flag │
│ 4-8 weeks │ 6-12 weeks │ 4-8 weeks │
────────────────────────────────────────────────────────────────────────────────

RULE: Start at Level 1. Only move to Level 2+ if Level 1 shows promise.
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Experiment 1: Fake Door Test

### Purpose
Validate that photographers are interested in integrated gallery delivery before building anything.

### Hypothesis
**If** we show photographers a "Coming Soon: Imagen Galleries" feature,  
**Then** >15% will click to learn more,  
**Because** they experience pain with current fragmented delivery workflow.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | Fake Door / Painted Door |
| **Duration** | 7 days |
| **Sample Size** | 5,000 impressions minimum |
| **Effort** | Low (1-2 days to set up) |
| **Cost** | Minimal (existing infrastructure) |

### Implementation

```
FAKE DOOR TEST IMPLEMENTATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PLACEMENT OPTIONS:

Option A: In-App Banner (Recommended)
┌─────────────────────────────────────────────────────────────────────────────┐
│  Imagen AI Dashboard                                                        │
│  ─────────────────────────────────────────────────────────────────────────  │
│                                                                             │
│  ┌───────────────────────────────────────────────────────────────────────┐ │
│  │  🎉 COMING SOON: Imagen Galleries                                     │ │
│  │                                                                       │ │
│  │  Deliver galleries to clients directly from Imagen.                   │ │
│  │  No more uploading to Pixieset. No more chasing payments.            │ │
│  │                                                                       │ │
│  │  [Learn More & Join Waitlist]                                        │ │
│  └───────────────────────────────────────────────────────────────────────┘ │
│                                                                             │
│  Your Recent Edits                                                          │
│  ─────────────────                                                          │
│  ...                                                                        │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘

Option B: Post-Edit Prompt
┌─────────────────────────────────────────────────────────────────────────────┐
│  ✅ Editing Complete!                                                       │
│                                                                             │
│  Your 847 photos are ready to export.                                       │
│                                                                             │
│  [Export to Lightroom]                                                      │
│                                                                             │
│  ─────────────────────────────────────────────────────────────────────────  │
│                                                                             │
│  💡 Coming Soon: Skip the export.                                           │
│     Deliver galleries directly to clients from Imagen.                      │
│                                                                             │
│  [Tell Me More]                                                             │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘

Option C: Email Campaign
Subject: "What if you never had to upload to Pixieset again?"

Body:
"We're exploring a new feature that would let you deliver galleries
directly from Imagen—no more exporting, uploading, and waiting.

Would this be valuable to you?

[Yes, I'm Interested] [Not For Me]"

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Success Metrics

| Metric | Kill | Pivot | Go |
|--------|------|-------|-----|
| **Click-Through Rate** | <5% | 5-15% | **>15%** |
| **Waitlist Signups** | <100 | 100-500 | **>500** |
| **Email Open Rate** | <20% | 20-35% | **>35%** |
| **Qualitative Feedback** | Negative | Mixed | **Positive** |

### What We Learn

- **If Go:** Strong interest validates the opportunity
- **If Pivot:** Interest exists but messaging needs work
- **If Kill:** Users don't perceive value; explore alternatives

### Follow-Up Questions (for waitlist signups)

1. "What gallery platform do you currently use?"
2. "How painful is your current delivery process? (1-10)"
3. "What would make you switch from your current solution?"

---

## Experiment 2: Pain Scoring Survey

### Purpose
Quantify the pain intensity of current delivery workflow to validate switching motivation.

### Hypothesis
**If** we ask photographers to rate their delivery pain,  
**Then** the average score will be >7/10,  
**Because** our story-based research indicates high frustration.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | One-Question Survey |
| **Duration** | 3-5 days |
| **Sample Size** | 500 responses minimum |
| **Effort** | Very Low (1 hour to set up) |
| **Cost** | Minimal |

### Survey Design

```
PAIN SCORING SURVEY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

QUESTION 1 (Required):
"After you finish editing in Imagen AI, how painful is the process of 
delivering galleries to clients and collecting payment?"

Scale: 1-10
1 = "Completely painless, I love it"
10 = "Extremely painful, I dread it"

[1] [2] [3] [4] [5] [6] [7] [8] [9] [10]

───────────────────────────────────────────────────────────────────────────────

QUESTION 2 (Optional):
"What's the most frustrating part of your post-editing workflow?"

[ ] Uploading to gallery platform
[ ] Organizing galleries
[ ] Sending delivery emails
[ ] Chasing payment
[ ] Following up with clients
[ ] Getting reviews
[ ] Other: ___________

───────────────────────────────────────────────────────────────────────────────

QUESTION 3 (Optional):
"If Imagen AI could handle gallery delivery and payment collection, 
how likely would you be to use it?"

[1] [2] [3] [4] [5] [6] [7] [8] [9] [10]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Success Metrics

| Metric | Kill | Pivot | Go |
|--------|------|-------|-----|
| **Average Pain Score** | <5/10 | 5-7/10 | **>7/10** |
| **% Scoring 8+** | <20% | 20-40% | **>40%** |
| **Intent to Use** | <5/10 | 5-7/10 | **>7/10** |
| **Response Rate** | <10% | 10-20% | **>20%** |

### Segmentation Analysis

Analyze results by:
- **Photographer type:** Wedding vs. Event vs. Portrait
- **Volume:** High volume (>30 shoots/year) vs. Low volume
- **Current tool:** Pixieset vs. ShootProof vs. Other
- **Tenure:** New users (<6 months) vs. Established users

---

## Experiment 3: Pricing Research (Van Westendorp)

### Purpose
Determine acceptable price range for integrated gallery delivery.

### Hypothesis
**If** we use Van Westendorp pricing methodology,  
**Then** we'll identify a price point that overlaps with our target,  
**Because** photographers already pay $10-25/month for gallery tools.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | Van Westendorp Price Sensitivity Meter |
| **Duration** | 2 weeks |
| **Sample Size** | 200 responses minimum |
| **Effort** | Medium (survey design + analysis) |
| **Cost** | Low |

### Survey Design

```
VAN WESTENDORP PRICING SURVEY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

CONTEXT:
"Imagine Imagen AI offered integrated gallery delivery with these features:
- One-click gallery creation from your edited photos
- Branded client galleries with your logo and colors
- Client downloads and favorites
- Integrated payment processing (you get paid when clients access gallery)
- Automated payment reminders
- Gallery view notifications

This would replace your current gallery platform (Pixieset, ShootProof, etc.)."

───────────────────────────────────────────────────────────────────────────────

QUESTION 1: Too Cheap
"At what monthly price would you consider this TOO CHEAP—so cheap that 
you'd question the quality?"

$_____ / month

───────────────────────────────────────────────────────────────────────────────

QUESTION 2: Cheap (Good Value)
"At what monthly price would you consider this a BARGAIN—a great deal 
for the value?"

$_____ / month

───────────────────────────────────────────────────────────────────────────────

QUESTION 3: Expensive (But Acceptable)
"At what monthly price would you consider this GETTING EXPENSIVE—but 
you'd still consider it?"

$_____ / month

───────────────────────────────────────────────────────────────────────────────

QUESTION 4: Too Expensive
"At what monthly price would you consider this TOO EXPENSIVE—so expensive 
you wouldn't consider it?"

$_____ / month

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Analysis Framework

```
VAN WESTENDORP ANALYSIS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

                    PRICE SENSITIVITY METER

% of Respondents
100% │
     │
 80% │                              
     │         ╱ Too Cheap          ╲ Too Expensive
 60% │        ╱                      ╲
     │       ╱                        ╲
 40% │      ╱     ┌──────────────┐     ╲
     │     ╱      │  ACCEPTABLE  │      ╲
 20% │    ╱       │    RANGE     │       ╲
     │   ╱        └──────────────┘        ╲
  0% │──────────────────────────────────────────────────
     $0    $10    $20    $30    $40    $50    $60

KEY POINTS:
• Point of Marginal Cheapness (PMC): Where "Too Cheap" = "Cheap"
• Point of Marginal Expensiveness (PME): Where "Expensive" = "Too Expensive"
• Optimal Price Point (OPP): Where "Too Cheap" = "Too Expensive"
• Indifference Price Point (IPP): Where "Cheap" = "Expensive"

ACCEPTABLE RANGE: Between PMC and PME

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Success Metrics

| Metric | Kill | Pivot | Go |
|--------|------|-------|-----|
| **Optimal Price Point** | <$10 | $10-20 | **$20-40** |
| **Acceptable Range Width** | <$10 | $10-20 | **>$20** |
| **Overlap with Target** | None | Partial | **Full** |

### Pricing Model Options

Based on research, recommend one of:

| Model | Description | When to Use |
|-------|-------------|-------------|
| **Included** | Gallery free with subscription | If WTP is low |
| **Tiered** | Basic free, premium $X/month | If WTP is medium |
| **Transaction** | Free gallery, 2.9% + 30¢ on payments | If WTP is variable |
| **Bundle** | New tier with gallery + payment | If WTP is high |

---

## Experiment 4: Story-Based Interviews

### Purpose
Deeply understand the delivery workflow and emotional journey through specific stories.

### Hypothesis
**If** we conduct story-based interviews focused on recent delivery experiences,  
**Then** we'll uncover specific pain points and switching triggers,  
**Because** stories reveal behavior, not just opinions.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | Story-Based User Interviews |
| **Duration** | 2-3 weeks |
| **Sample Size** | 15-20 interviews |
| **Effort** | Medium-High |
| **Cost** | Moderate (interviewer time) |

### Interview Guide

```
STORY-BASED INTERVIEW GUIDE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

OPENING (5 min)
───────────────────────────────────────────────────────────────────────────────
"Thanks for taking the time. I'm researching how photographers handle 
the workflow after editing. There are no right or wrong answers—I just 
want to hear about your actual experience."

WARM-UP (5 min)
───────────────────────────────────────────────────────────────────────────────
"Tell me a bit about your photography business. What types of shoots 
do you do? How many per month?"

THE STORY (25 min)
───────────────────────────────────────────────────────────────────────────────
"Think about the last wedding (or event) you delivered to a client. 
Walk me through what happened from the moment you finished editing 
to the moment the client had their photos."

PROBING QUESTIONS:
• "What happened next?"
• "How long did that take?"
• "What was hard about that?"
• "How did that make you feel?"
• "What did you try before that?"
• "What would you have done differently?"

SPECIFIC MOMENTS TO EXPLORE:
• Gallery upload process
• Delivery communication
• Payment collection
• Client response (or non-response)
• Follow-up and reviews

THE PAIN (10 min)
───────────────────────────────────────────────────────────────────────────────
"If you could wave a magic wand and fix one thing about your 
post-editing workflow, what would it be?"

"On a scale of 1-10, how painful is your current delivery process?"

"What would make you switch from your current gallery platform?"

THE SOLUTION (10 min)
───────────────────────────────────────────────────────────────────────────────
"Imagine if after you finished editing in Imagen AI, you could 
deliver the gallery directly to clients without leaving the app. 
The client would pay before downloading. How would that change 
your workflow?"

PROBING:
• "What would be most valuable about that?"
• "What concerns would you have?"
• "What would it need to have for you to use it?"
• "What would make you NOT use it?"

CLOSING (5 min)
───────────────────────────────────────────────────────────────────────────────
"Is there anything else about your delivery workflow that I should know?"

"Can I follow up if I have more questions?"

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Interview Synthesis Template

| Interviewee | Segment | Key Story | Pain Points | Switching Trigger | Concerns | Quote |
|-------------|---------|-----------|-------------|-------------------|----------|-------|
| P01 | Wedding | ... | ... | ... | ... | "..." |
| P02 | Event | ... | ... | ... | ... | "..." |
| ... | ... | ... | ... | ... | ... | ... |

### Success Metrics

| Metric | Kill | Pivot | Go |
|--------|------|-------|-----|
| **Strong Interest** | <5/15 | 5-10/15 | **>10/15** |
| **Clear Pain Points** | Vague | Some specific | **Very specific** |
| **Switching Intent** | <30% | 30-60% | **>60%** |
| **Concerns Addressable** | Major blockers | Some concerns | **Minor concerns** |

---

## Experiment 5: Prototype Usability Testing

### Purpose
Validate that the proposed solution is usable before building.

### Hypothesis
**If** we test a clickable prototype with photographers,  
**Then** >80% will complete the core tasks without help,  
**Because** we've designed based on their existing mental models.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | Moderated Usability Testing |
| **Duration** | 2 weeks |
| **Sample Size** | 15-20 participants |
| **Effort** | High (prototype + testing) |
| **Cost** | Moderate |

### Prototype Scope

```
PROTOTYPE SCOPE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

CORE FLOWS TO TEST:

Flow 1: Create Gallery
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│ Select   │───▶│ Customize│───▶│ Set      │───▶│ Publish  │
│ Photos   │    │ Gallery  │    │ Payment  │    │ Gallery  │
└──────────┘    └──────────┘    └──────────┘    └──────────┘

Flow 2: Send to Client
┌──────────┐    ┌──────────┐    ┌──────────┐
│ Enter    │───▶│ Customize│───▶│ Send     │
│ Email    │    │ Message  │    │ Delivery │
└──────────┘    └──────────┘    └──────────┘

Flow 3: Track Engagement
┌──────────┐    ┌──────────┐    ┌──────────┐
│ View     │───▶│ See      │───▶│ Follow   │
│ Dashboard│    │ Analytics│    │ Up       │
└──────────┘    └──────────┘    └──────────┘

Flow 4: Client Experience
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│ Receive  │───▶│ View     │───▶│ Pay      │───▶│ Download │
│ Email    │    │ Gallery  │    │          │    │ Photos   │
└──────────┘    └──────────┘    └──────────┘    └──────────┘

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Test Script

```
USABILITY TEST SCRIPT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

INTRODUCTION (5 min)
───────────────────────────────────────────────────────────────────────────────
"Thanks for helping us test this prototype. This is not a test of you—
we're testing the design. Please think aloud as you go."

TASK 1: Create a Gallery (10 min)
───────────────────────────────────────────────────────────────────────────────
"Imagine you just finished editing a wedding in Imagen AI. You want to 
create a gallery for the client. Show me how you would do that."

OBSERVE:
• Where do they click first?
• Do they understand the flow?
• Where do they get stuck?
• What questions do they ask?

TASK 2: Set Up Payment (5 min)
───────────────────────────────────────────────────────────────────────────────
"The client owes you $500 for this wedding. Set up the gallery so they 
need to pay before downloading."

OBSERVE:
• Do they find the payment settings?
• Do they understand the options?
• Any confusion or concerns?

TASK 3: Send to Client (5 min)
───────────────────────────────────────────────────────────────────────────────
"Send this gallery to the client at bride@email.com."

OBSERVE:
• Is the send flow intuitive?
• Do they customize the message?
• Any hesitation?

TASK 4: Check Engagement (5 min)
───────────────────────────────────────────────────────────────────────────────
"It's been 3 days. Check if the client has viewed the gallery."

OBSERVE:
• Do they find the analytics?
• Do they understand the data?
• What would they do next?

TASK 5: Client Experience (10 min)
───────────────────────────────────────────────────────────────────────────────
"Now pretend you're the client. You received an email with the gallery 
link. Show me how you would view and download your photos."

OBSERVE:
• Is the client experience intuitive?
• Any friction in payment?
• Download experience?

DEBRIEF (10 min)
───────────────────────────────────────────────────────────────────────────────
"Overall, how was that experience?"
"What was confusing?"
"What would you change?"
"Would you use this instead of your current gallery platform?"

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Success Metrics

| Metric | Kill | Pivot | Go |
|--------|------|-------|-----|
| **Task Completion Rate** | <60% | 60-80% | **>80%** |
| **Time on Task** | >3x expected | 1.5-3x | **<1.5x** |
| **Critical Errors** | >3 per user | 1-3 | **<1** |
| **SUS Score** | <50 | 50-70 | **>70** |
| **Intent to Use** | <50% | 50-70% | **>70%** |

---

## Experiment 6: Wizard of Oz Test

### Purpose
Validate the value proposition by manually delivering the experience before building automation.

### Hypothesis
**If** we manually handle gallery delivery for 10 photographers,  
**Then** we'll validate the workflow and identify edge cases,  
**Because** real usage reveals requirements that prototypes miss.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | Wizard of Oz / Concierge |
| **Duration** | 4 weeks |
| **Sample Size** | 10 photographers, 20-30 galleries |
| **Effort** | High (manual work) |
| **Cost** | Moderate (staff time) |

### Implementation

```
WIZARD OF OZ IMPLEMENTATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

PHOTOGRAPHER EXPERIENCE (What They See):
───────────────────────────────────────────────────────────────────────────────
1. Finish editing in Imagen AI
2. Click "Create Gallery" button
3. Fill out simple form (client email, price, message)
4. Click "Send Gallery"
5. Receive notification when client views/pays
6. See analytics dashboard

BEHIND THE SCENES (What We Do Manually):
───────────────────────────────────────────────────────────────────────────────
1. Receive photographer's gallery request
2. Manually create gallery in Pixieset (or simple web page)
3. Set up Stripe payment link
4. Send email to client with our template
5. Monitor for client activity
6. Notify photographer of views/payments
7. Manually update "dashboard" (could be simple spreadsheet)

WHAT WE LEARN:
───────────────────────────────────────────────────────────────────────────────
• Actual workflow requirements
• Edge cases (international clients, refunds, etc.)
• Communication preferences
• Pricing sensitivity in practice
• Client experience issues
• Time savings (measured)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Success Metrics

| Metric | Kill | Pivot | Go |
|--------|------|-------|-----|
| **Photographer Satisfaction** | <7/10 | 7-8/10 | **>8/10** |
| **Client Completion Rate** | <70% | 70-85% | **>85%** |
| **Payment Collection Rate** | <60% | 60-80% | **>80%** |
| **Time Saved (Reported)** | <15 min | 15-30 min | **>30 min** |
| **Would Use Again** | <70% | 70-85% | **>85%** |

---

## Experiment 7: Beta Launch

### Purpose
Validate the full solution with a controlled group before general availability.

### Hypothesis
**If** we launch to 50 power users with full gallery + payment features,  
**Then** we'll achieve >60% adoption and +15% retention improvement,  
**Because** the integrated workflow solves a real pain point.

### Experiment Design

| Attribute | Value |
|-----------|-------|
| **Type** | Beta Launch |
| **Duration** | 8-12 weeks |
| **Sample Size** | 50 power users |
| **Effort** | Very High (full build) |
| **Cost** | High |

### Beta Recruitment Criteria

| Criterion | Requirement | Rationale |
|-----------|-------------|-----------|
| **Usage** | >100 images/month | Active users |
| **Tenure** | >6 months | Established workflow |
| **Segment** | Mix of wedding/event/portrait | Representative |
| **Current Gallery** | Pixieset or ShootProof | Switching potential |
| **Engagement** | Responded to surveys | Feedback-oriented |

### Beta Metrics Dashboard

```
BETA METRICS DASHBOARD
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

ADOPTION METRICS
───────────────────────────────────────────────────────────────────────────────
Feature Activation Rate:    [███████████████████░░░░░░░░░░░] 65%  Target: 60%
Galleries Created:          [██████████████████████████████] 127  Target: 100
Payments Processed:         [████████████████████░░░░░░░░░░] 68%  Target: 60%
Weekly Active Users:        [███████████████████████░░░░░░░] 78%  Target: 70%

ENGAGEMENT METRICS
───────────────────────────────────────────────────────────────────────────────
Avg. Galleries/User/Week:   2.4   (Target: 2.0)
Avg. Time in Feature:       12 min (Target: 10 min)
Return Usage Rate:          85%   (Target: 80%)
Client Engagement Rate:     92%   (Target: 85%)

SATISFACTION METRICS
───────────────────────────────────────────────────────────────────────────────
Feature NPS:                +52   (Target: +40)
Ease of Use Rating:         4.3/5 (Target: 4.0)
Would Recommend:            89%   (Target: 80%)
Prefer Over Pixieset:       72%   (Target: 60%)

BUSINESS METRICS
───────────────────────────────────────────────────────────────────────────────
Payment GMV:                $24,500 (Target: $20,000)
Revenue Per User:           $18/mo  (Target: $15/mo)
Retention (vs. Control):    +18%    (Target: +15%)
Churn (vs. Control):        -22%    (Target: -15%)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Success Metrics

| Metric | Kill | Pivot | Go to GA |
|--------|------|-------|----------|
| **Feature Activation** | <40% | 40-60% | **>60%** |
| **Weekly Active Usage** | <50% | 50-70% | **>70%** |
| **Feature NPS** | <20 | 20-40 | **>40** |
| **Retention Impact** | <5% | 5-15% | **>15%** |
| **Would Recommend** | <60% | 60-80% | **>80%** |

---

## Consolidated Experiment Timeline

```
EXPERIMENT TIMELINE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

WEEK    1    2    3    4    5    6    7    8    9   10   11   12
       ─────────────────────────────────────────────────────────────

EXP 1  ████████                                                    Fake Door
       │
       └──▶ GO/NO-GO DECISION #1

EXP 2  ████                                                        Pain Survey
       │
       └──▶ Validate pain intensity

EXP 3       ████████████                                           Pricing
            │
            └──▶ Determine price point

EXP 4       ████████████████                                       Interviews
            │
            └──▶ Deep understanding

                        ──▶ GO/NO-GO DECISION #2

EXP 5                   ████████████                               Usability
                        │
                        └──▶ Validate UX

EXP 6                        ████████████████████                  Wizard of Oz
                             │
                             └──▶ Validate value

                                            ──▶ GO/NO-GO DECISION #3

EXP 7                                            ████████████████  Beta Launch
                                                 │
                                                 └──▶ Full validation

                                                                ──▶ GA DECISION

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Decision Framework Summary

### Go/No-Go Decision Points

| Decision Point | Week | Key Metrics | Go Criteria | Kill Criteria |
|----------------|------|-------------|-------------|---------------|
| **#1: Interest** | 2 | Fake door CTR, Pain score | >15% CTR, >7/10 pain | <5% CTR, <5/10 pain |
| **#2: Value** | 6 | Interviews, Pricing | 10/15 interested, price fit | <5/15, no price fit |
| **#3: Usability** | 9 | Prototype, Wizard of Oz | >80% completion, >8/10 sat | <60% completion |
| **#4: Launch** | 12 | Beta metrics | >60% adoption, +15% retention | <40% adoption |

### Risk Mitigation by Experiment

| Risk | Experiment | Mitigation |
|------|------------|------------|
| **No demand** | Fake Door, Pain Survey | Kill early, save resources |
| **Wrong price** | Van Westendorp | Adjust pricing model |
| **Poor UX** | Prototype Testing | Iterate design |
| **Hidden complexity** | Wizard of Oz | Discover before building |
| **Low adoption** | Beta | Iterate before GA |

---

## Appendix: Experiment Templates

### A. Fake Door Test Tracking

| Date | Impressions | Clicks | CTR | Signups | Notes |
|------|-------------|--------|-----|---------|-------|
| Day 1 | | | | | |
| Day 2 | | | | | |
| ... | | | | | |
| Total | | | | | |

### B. Interview Synthesis Template

| ID | Segment | Pain Score | Switching Intent | Key Quote | Concerns |
|----|---------|------------|------------------|-----------|----------|
| P01 | | | | | |
| P02 | | | | | |
| ... | | | | | |

### C. Usability Test Results

| Task | Participant | Completed | Time | Errors | Comments |
|------|-------------|-----------|------|--------|----------|
| Task 1 | P01 | | | | |
| Task 1 | P02 | | | | |
| ... | | | | | |

---

*Experiment Framework Completed: December 5, 2025*  
*Methodology: Lean Experimentation + Continuous Discovery*  
*Total Experiments Designed: 7*  
*Estimated Timeline: 12 weeks*  
*Go/No-Go Decision Points: 4*

