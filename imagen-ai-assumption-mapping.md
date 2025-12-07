# Imagen AI - Assumption Mapping & Risk Assessment
## Phase 3: Assumption Testing Framework

*Based on Research Methodology from Next Capability Research Plan*  
*Framework: Four-Dimension Assumption Mapping*  
*Date: December 5, 2025*

---

## Executive Summary

This document maps the critical assumptions underlying Imagen AI's next capability expansion (Gallery Delivery + Payment Hub). Following the research methodology, we categorize assumptions across four dimensions: **Desirability**, **Viability**, **Feasibility**, and **Usability**. Each assumption is scored for risk and prioritized for testing.

**Key Finding:** The riskiest assumptions are around **willingness to pay for integrated delivery** and **switching behavior from existing gallery platforms**. These must be validated before significant investment.

---

## Assumption Mapping Framework

### The Four Dimensions

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         ASSUMPTION DIMENSIONS                                │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│   ┌─────────────────────────────┐   ┌─────────────────────────────┐         │
│   │                             │   │                             │         │
│   │      DESIRABILITY           │   │        VIABILITY            │         │
│   │                             │   │                             │         │
│   │   Will they want it?        │   │   Will it work for the      │         │
│   │                             │   │   business?                 │         │
│   │   • User demand             │   │   • Revenue model           │         │
│   │   • Pain intensity          │   │   • Unit economics          │         │
│   │   • Switching motivation    │   │   • Market size             │         │
│   │   • Willingness to pay      │   │   • Competitive dynamics    │         │
│   │                             │   │                             │         │
│   └─────────────────────────────┘   └─────────────────────────────┘         │
│                                                                              │
│   ┌─────────────────────────────┐   ┌─────────────────────────────┐         │
│   │                             │   │                             │         │
│   │      FEASIBILITY            │   │        USABILITY            │         │
│   │                             │   │                             │         │
│   │   Can we build it?          │   │   Can they use it?          │         │
│   │                             │   │                             │         │
│   │   • Technical capability    │   │   • Learning curve          │         │
│   │   • Infrastructure          │   │   • Workflow integration    │         │
│   │   • Timeline                │   │   • Client experience       │         │
│   │   • Resources               │   │   • Migration effort        │         │
│   │                             │   │                             │         │
│   └─────────────────────────────┘   └─────────────────────────────┘         │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Risk Scoring

| Score | Level | Description |
|-------|-------|-------------|
| 🔴 **9-10** | Critical | Must validate before any investment |
| 🟠 **7-8** | High | Should validate before major investment |
| 🟡 **5-6** | Medium | Validate during development |
| 🟢 **3-4** | Low | Monitor but don't prioritize |
| ⚪ **1-2** | Minimal | Assume true, validate post-launch |

---

## Dimension 1: Desirability Assumptions

### "Will they want it?"

#### D1: Photographers want gallery delivery integrated with editing

| Attribute | Value |
|-----------|-------|
| **Assumption** | Photographers prefer integrated gallery delivery over separate tools |
| **Risk Level** | 🟠 **7/10 - HIGH** |
| **Evidence For** | Story-based interviews mention "wish one tool did it all" |
| **Evidence Against** | No explicit feature requests; users have solved with Pixieset |
| **Why Risky** | Latent need—users don't ask for what they don't know exists |

**Test Method:** Fake door test + user interviews  
**Success Criteria:** >15% CTR on fake door, 8/10 users express strong interest  
**Timeline:** 1-2 weeks

---

#### D2: Pain with current delivery is high enough to switch

| Attribute | Value |
|-----------|-------|
| **Assumption** | Photographers find current delivery painful enough to adopt a new solution |
| **Risk Level** | 🟠 **8/10 - HIGH** |
| **Evidence For** | 40% of stories mention delivery frustration |
| **Evidence Against** | Users have already invested in Pixieset/ShootProof |
| **Why Risky** | Switching costs are real; "good enough" is the enemy |

**Test Method:** Pain scoring survey (1-10) + switching intent questions  
**Success Criteria:** >7/10 average pain score, >50% express switching intent  
**Timeline:** 1 week

---

#### D3: Photographers will pay for integrated delivery

| Attribute | Value |
|-----------|-------|
| **Assumption** | Photographers will pay incrementally (or accept higher subscription) for delivery features |
| **Risk Level** | 🔴 **9/10 - CRITICAL** |
| **Evidence For** | Users pay $10-25/month for Pixieset; consolidation has value |
| **Evidence Against** | Price sensitivity mentioned in 20% of reviews |
| **Why Risky** | Pricing is the #1 concern in negative reviews |

**Test Method:** Van Westendorp pricing research + conjoint analysis  
**Success Criteria:** Acceptable price range overlaps with target pricing  
**Timeline:** 2-3 weeks

---

#### D4: Payment-gated galleries are acceptable to photographers

| Attribute | Value |
|-----------|-------|
| **Assumption** | Photographers will use payment-gated gallery access |
| **Risk Level** | 🟡 **6/10 - MEDIUM** |
| **Evidence For** | "I wish payment just happened" from interviews |
| **Evidence Against** | Some photographers may feel it's too aggressive |
| **Why Risky** | Cultural/relationship concerns with clients |

**Test Method:** Concept testing with 20 photographers  
**Success Criteria:** >70% find it acceptable, <10% strong objection  
**Timeline:** 1 week

---

#### D5: Clients will accept payment-gated galleries

| Attribute | Value |
|-----------|-------|
| **Assumption** | Clients (end users) will not be frustrated by payment-gated access |
| **Risk Level** | 🟡 **5/10 - MEDIUM** |
| **Evidence For** | Common practice in e-commerce; expectation of payment for service |
| **Evidence Against** | Some clients may expect photos without payment first |
| **Why Risky** | Photographer-client relationship is sacred |

**Test Method:** Client experience testing (via photographer beta users)  
**Success Criteria:** <5% client complaints, no photographer churn due to client issues  
**Timeline:** During beta

---

### Desirability Assumption Summary

| ID | Assumption | Risk | Priority |
|----|------------|------|----------|
| D1 | Want integrated delivery | 🟠 7/10 | P1 |
| D2 | Pain high enough to switch | 🟠 8/10 | P0 |
| D3 | Will pay for delivery | 🔴 9/10 | P0 |
| D4 | Payment-gated acceptable to photographers | 🟡 6/10 | P1 |
| D5 | Payment-gated acceptable to clients | 🟡 5/10 | P2 |

---

## Dimension 2: Viability Assumptions

### "Will it work for the business?"

#### V1: Transaction fees provide meaningful revenue

| Attribute | Value |
|-----------|-------|
| **Assumption** | Payment processing fees (2.9% + 30¢ pass-through + margin) generate significant revenue |
| **Risk Level** | 🟡 **5/10 - MEDIUM** |
| **Evidence For** | Industry standard; Stripe Connect is proven model |
| **Evidence Against** | Margins may be thin; volume required |
| **Why Risky** | Revenue model depends on payment volume |

**Test Method:** Financial modeling + beta usage data  
**Success Criteria:** $X revenue per active user per month  
**Timeline:** During beta

---

#### V2: Delivery features increase retention

| Attribute | Value |
|-----------|-------|
| **Assumption** | Adding delivery features reduces churn and increases LTV |
| **Risk Level** | 🟠 **7/10 - HIGH** |
| **Evidence For** | More features = higher switching cost (theory) |
| **Evidence Against** | Could dilute focus; users may prefer specialized tools |
| **Why Risky** | Core to the LTV+40% goal |

**Test Method:** Beta cohort retention analysis  
**Success Criteria:** >15% improvement in 90-day retention for feature users  
**Timeline:** 3 months post-launch

---

#### V3: Can compete with established gallery platforms

| Attribute | Value |
|-----------|-------|
| **Assumption** | Imagen AI can build galleries competitive with Pixieset/ShootProof |
| **Risk Level** | 🟠 **7/10 - HIGH** |
| **Evidence For** | Integration advantage; AI differentiation potential |
| **Evidence Against** | Pixieset has 10+ years of refinement |
| **Why Risky** | "Good enough" galleries may not be good enough |

**Test Method:** Competitive UX testing  
**Success Criteria:** Comparable or better satisfaction scores vs. Pixieset  
**Timeline:** 2-3 weeks

---

#### V4: Unit economics work at scale

| Attribute | Value |
|-----------|-------|
| **Assumption** | Cost of gallery hosting + payment processing is sustainable |
| **Risk Level** | 🟡 **5/10 - MEDIUM** |
| **Evidence For** | Cloud costs are predictable; CDN is commodity |
| **Evidence Against** | Storage costs for high-volume users |
| **Why Risky** | Could erode margins if not managed |

**Test Method:** Cost modeling + beta usage analysis  
**Success Criteria:** Positive unit economics at average usage  
**Timeline:** During beta

---

#### V5: Market timing is right

| Attribute | Value |
|-----------|-------|
| **Assumption** | Photographers are ready for consolidated platforms now |
| **Risk Level** | 🟡 **4/10 - LOW** |
| **Evidence For** | Tool fatigue is real; consolidation trend in SaaS |
| **Evidence Against** | Photographers may resist change |
| **Why Risky** | Market readiness affects adoption speed |

**Test Method:** Market research + beta adoption rate  
**Success Criteria:** >50% beta adoption within 30 days  
**Timeline:** During beta

---

### Viability Assumption Summary

| ID | Assumption | Risk | Priority |
|----|------------|------|----------|
| V1 | Transaction fees meaningful | 🟡 5/10 | P2 |
| V2 | Delivery increases retention | 🟠 7/10 | P1 |
| V3 | Can compete with Pixieset | 🟠 7/10 | P1 |
| V4 | Unit economics work | 🟡 5/10 | P2 |
| V5 | Market timing right | 🟡 4/10 | P3 |

---

## Dimension 3: Feasibility Assumptions

### "Can we build it?"

#### F1: Can build gallery hosting infrastructure

| Attribute | Value |
|-----------|-------|
| **Assumption** | Team can build scalable, fast gallery hosting |
| **Risk Level** | 🟡 **5/10 - MEDIUM** |
| **Evidence For** | Already handle large image volumes; cloud expertise |
| **Evidence Against** | Different use case (delivery vs. processing) |
| **Why Risky** | Performance and reliability are table stakes |

**Test Method:** Technical proof of concept  
**Success Criteria:** <2s page load, 99.9% uptime in POC  
**Timeline:** 2-3 weeks

---

#### F2: Can integrate Stripe Connect successfully

| Attribute | Value |
|-----------|-------|
| **Assumption** | Stripe Connect integration is achievable within timeline |
| **Risk Level** | 🟡 **4/10 - LOW** |
| **Evidence For** | Well-documented API; many successful implementations |
| **Evidence Against** | Compliance requirements (KYC, etc.) |
| **Why Risky** | Payment is critical path; delays are costly |

**Test Method:** Technical spike + Stripe partnership discussion  
**Success Criteria:** POC payment flow working  
**Timeline:** 2 weeks

---

#### F3: Can ship MVP in 3 months

| Attribute | Value |
|-----------|-------|
| **Assumption** | MVP (gallery + basic payment) can ship in 3 months |
| **Risk Level** | 🟠 **6/10 - MEDIUM** |
| **Evidence For** | Focused scope; experienced team |
| **Evidence Against** | New domain; unknown unknowns |
| **Why Risky** | Delays affect competitive position |

**Test Method:** Detailed sprint planning + risk buffer  
**Success Criteria:** Ship within 3 months ± 2 weeks  
**Timeline:** Ongoing

---

#### F4: Existing infrastructure can handle load

| Attribute | Value |
|-----------|-------|
| **Assumption** | Current cloud infrastructure scales for gallery delivery |
| **Risk Level** | 🟡 **5/10 - MEDIUM** |
| **Evidence For** | Already handle 150M+ photos/year |
| **Evidence Against** | Different access patterns (burst delivery vs. batch processing) |
| **Why Risky** | Performance issues damage trust |

**Test Method:** Load testing + architecture review  
**Success Criteria:** Handle 10x expected peak load  
**Timeline:** 2 weeks

---

#### F5: Can maintain editing quality while expanding

| Attribute | Value |
|-----------|-------|
| **Assumption** | Adding delivery features doesn't degrade core editing experience |
| **Risk Level** | 🟡 **4/10 - LOW** |
| **Evidence For** | Separate feature; different team focus |
| **Evidence Against** | Resource competition; attention dilution |
| **Why Risky** | Core product is the moat |

**Test Method:** Quality monitoring + user feedback  
**Success Criteria:** No degradation in editing NPS  
**Timeline:** Ongoing

---

### Feasibility Assumption Summary

| ID | Assumption | Risk | Priority |
|----|------------|------|----------|
| F1 | Can build gallery hosting | 🟡 5/10 | P1 |
| F2 | Can integrate Stripe | 🟡 4/10 | P2 |
| F3 | Can ship in 3 months | 🟠 6/10 | P1 |
| F4 | Infrastructure scales | 🟡 5/10 | P1 |
| F5 | Maintain editing quality | 🟡 4/10 | P3 |

---

## Dimension 4: Usability Assumptions

### "Can they use it?"

#### U1: Photographers can set up galleries without training

| Attribute | Value |
|-----------|-------|
| **Assumption** | Gallery creation is intuitive enough for self-service |
| **Risk Level** | 🟠 **7/10 - HIGH** |
| **Evidence For** | Users already use Pixieset; familiar patterns |
| **Evidence Against** | Learning curve mentioned in 15% of reviews |
| **Why Risky** | Onboarding friction kills adoption |

**Test Method:** Unmoderated usability testing  
**Success Criteria:** >80% complete first gallery without help  
**Timeline:** 2 weeks

---

#### U2: Workflow integration feels seamless

| Attribute | Value |
|-----------|-------|
| **Assumption** | Edit → Deliver flow feels natural, not bolted-on |
| **Risk Level** | 🟠 **8/10 - HIGH** |
| **Evidence For** | Integration is our differentiator |
| **Evidence Against** | New feature may feel disconnected |
| **Why Risky** | Seamlessness is the value proposition |

**Test Method:** Workflow testing with 20 users  
**Success Criteria:** >90% describe flow as "seamless" or "natural"  
**Timeline:** 2 weeks

---

#### U3: Clients can navigate galleries easily

| Attribute | Value |
|-----------|-------|
| **Assumption** | End clients can view, pay, and download without confusion |
| **Risk Level** | 🟡 **6/10 - MEDIUM** |
| **Evidence For** | Standard e-commerce patterns |
| **Evidence Against** | Photographers' clients vary widely in tech savviness |
| **Why Risky** | Client frustration reflects on photographer |

**Test Method:** Client-side usability testing  
**Success Criteria:** >95% task completion rate  
**Timeline:** 2 weeks

---

#### U4: Migration from existing galleries is manageable

| Attribute | Value |
|-----------|-------|
| **Assumption** | Users can migrate from Pixieset/ShootProof without major friction |
| **Risk Level** | 🟡 **6/10 - MEDIUM** |
| **Evidence For** | Can start fresh; gradual migration |
| **Evidence Against** | Years of galleries, client links, etc. |
| **Why Risky** | Migration friction prevents switching |

**Test Method:** Migration pathway testing  
**Success Criteria:** <2 hours to migrate typical user  
**Timeline:** During beta

---

#### U5: Mobile experience is sufficient

| Attribute | Value |
|-----------|-------|
| **Assumption** | Galleries work well on mobile (where clients view) |
| **Risk Level** | 🟡 **5/10 - MEDIUM** |
| **Evidence For** | Mobile-first design is standard |
| **Evidence Against** | High-res images on mobile is challenging |
| **Why Risky** | 60%+ of gallery views are mobile |

**Test Method:** Mobile usability testing  
**Success Criteria:** >4.5/5 mobile experience rating  
**Timeline:** 2 weeks

---

### Usability Assumption Summary

| ID | Assumption | Risk | Priority |
|----|------------|------|----------|
| U1 | Setup without training | 🟠 7/10 | P1 |
| U2 | Seamless workflow | 🟠 8/10 | P0 |
| U3 | Client navigation easy | 🟡 6/10 | P1 |
| U4 | Migration manageable | 🟡 6/10 | P2 |
| U5 | Mobile sufficient | 🟡 5/10 | P2 |

---

## Consolidated Risk Assessment

### Risk Heat Map

```
ASSUMPTION RISK HEAT MAP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

                           IMPACT
                 Low         Medium        High
            ┌──────────┬──────────┬──────────┐
            │          │          │          │
    High    │          │   F3     │   D2     │  🔴 CRITICAL
            │          │   U1     │   D3     │     ZONE
            │          │          │   U2     │
            ├──────────┼──────────┼──────────┤
 LIKELIHOOD │          │   V1     │   D1     │  🟠 HIGH
            │   V5     │   F1     │   V2     │     RISK
    Medium  │   F5     │   F4     │   V3     │
            │          │   U4     │          │
            ├──────────┼──────────┼──────────┤
            │          │   D4     │          │  🟡 MEDIUM
    Low     │   F2     │   D5     │          │     RISK
            │          │   U3     │          │
            │          │   U5     │          │
            └──────────┴──────────┴──────────┘

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Top 10 Riskiest Assumptions

| Rank | ID | Assumption | Risk | Dimension | Test Priority |
|------|-----|------------|------|-----------|---------------|
| 1 | **D3** | Will pay for delivery | 🔴 9/10 | Desirability | **P0 - IMMEDIATE** |
| 2 | **D2** | Pain high enough to switch | 🟠 8/10 | Desirability | **P0 - IMMEDIATE** |
| 3 | **U2** | Seamless workflow | 🟠 8/10 | Usability | **P0 - IMMEDIATE** |
| 4 | **D1** | Want integrated delivery | 🟠 7/10 | Desirability | P1 |
| 5 | **V2** | Delivery increases retention | 🟠 7/10 | Viability | P1 |
| 6 | **V3** | Can compete with Pixieset | 🟠 7/10 | Viability | P1 |
| 7 | **U1** | Setup without training | 🟠 7/10 | Usability | P1 |
| 8 | **F3** | Can ship in 3 months | 🟠 6/10 | Feasibility | P1 |
| 9 | **D4** | Payment-gated acceptable | 🟡 6/10 | Desirability | P2 |
| 10 | **U3** | Client navigation easy | 🟡 6/10 | Usability | P2 |

---

## Testing Plan

### Phase 1: Pre-Investment Validation (Weeks 1-3)

**Goal:** Validate critical assumptions before committing resources

| Test | Assumption | Method | Timeline | Owner |
|------|------------|--------|----------|-------|
| **Fake Door Test** | D1, D2 | "Coming Soon" landing page | Week 1 | PM |
| **Pricing Research** | D3 | Van Westendorp survey | Week 1-2 | PM |
| **Pain Scoring Survey** | D2 | 1-question survey to 500 users | Week 1 | PM |
| **User Interviews** | D1, D2, D4 | 10 story-based interviews | Week 2-3 | UXR |
| **Technical Spike** | F1, F2 | POC for gallery + Stripe | Week 2-3 | Eng |

### Phase 2: Design Validation (Weeks 4-6)

**Goal:** Validate usability before building

| Test | Assumption | Method | Timeline | Owner |
|------|------------|--------|----------|-------|
| **Prototype Testing** | U1, U2 | Clickable prototype with 20 users | Week 4-5 | Design |
| **Workflow Testing** | U2 | End-to-end flow testing | Week 5-6 | UXR |
| **Competitive UX Testing** | V3 | Compare to Pixieset | Week 5 | UXR |
| **Client Experience Testing** | U3 | Client-side prototype testing | Week 6 | UXR |

### Phase 3: Beta Validation (Weeks 7-12)

**Goal:** Validate viability and retention assumptions

| Test | Assumption | Method | Timeline | Owner |
|------|------------|--------|----------|-------|
| **Beta Launch** | All | 50 power users | Week 7 | PM |
| **Retention Analysis** | V2 | Cohort comparison | Week 10-12 | Analytics |
| **Revenue Tracking** | V1 | Payment volume monitoring | Week 8-12 | Analytics |
| **NPS Tracking** | V2, U2 | Weekly NPS survey | Week 8-12 | PM |

---

## Go/No-Go Decision Framework

### Decision Point 1: After Pre-Investment Validation (Week 3)

| Signal | Go | Pivot | Kill |
|--------|-----|-------|------|
| **Fake Door CTR** | >15% | 10-15% | <10% |
| **Pain Score** | >7/10 | 5-7/10 | <5/10 |
| **Pricing Fit** | Clear overlap | Narrow overlap | No overlap |
| **Interview Enthusiasm** | 8/10 strong interest | 5/10 interest | <5/10 interest |
| **Technical Feasibility** | POC works | POC with issues | POC fails |

**If Go:** Proceed to design phase  
**If Pivot:** Adjust scope or positioning  
**If Kill:** Explore alternative opportunities

### Decision Point 2: After Design Validation (Week 6)

| Signal | Go | Pivot | Kill |
|--------|-----|-------|------|
| **Usability Score** | >80% task completion | 60-80% | <60% |
| **Workflow Seamlessness** | >90% "seamless" | 70-90% | <70% |
| **Competitive Comparison** | Equal or better | Slightly worse | Much worse |
| **Client Experience** | >95% completion | 85-95% | <85% |

**If Go:** Proceed to build phase  
**If Pivot:** Redesign problem areas  
**If Kill:** Reassess opportunity

### Decision Point 3: After Beta (Week 12)

| Signal | Go | Pivot | Kill |
|--------|-----|-------|------|
| **Beta Adoption** | >60% of beta users | 40-60% | <40% |
| **Retention Impact** | >15% improvement | 5-15% | <5% |
| **NPS Impact** | +5 points | 0-5 points | Negative |
| **Revenue Per User** | On target | 50-100% of target | <50% |

**If Go:** Full launch  
**If Pivot:** Iterate before launch  
**If Kill:** Sunset feature, learn for next opportunity

---

## Risk Mitigation Strategies

### For Critical Assumptions

#### D3: Willingness to Pay

**Mitigation Strategies:**
1. **Bundle with subscription** — Include basic delivery free, charge for premium
2. **Transaction fee only** — No subscription increase, just payment processing fee
3. **Freemium model** — Free tier drives adoption, paid tier for power users
4. **Competitive pricing** — Match or beat Pixieset pricing

#### D2: Pain High Enough to Switch

**Mitigation Strategies:**
1. **Migration tools** — Make switching from Pixieset easy
2. **Parallel use** — Allow using both during transition
3. **Incentives** — Free months for switchers
4. **Superior integration** — Make the workflow so good they can't resist

#### U2: Seamless Workflow

**Mitigation Strategies:**
1. **Extensive UX testing** — Test early, test often
2. **Photographer co-design** — Involve users in design process
3. **Gradual rollout** — Beta → soft launch → full launch
4. **Rapid iteration** — Fix issues quickly based on feedback

---

## Assumption Tracking Template

### Weekly Assumption Review

| Week | Assumption | Test Conducted | Result | Confidence | Next Action |
|------|------------|----------------|--------|------------|-------------|
| 1 | D3 | Van Westendorp | TBD | TBD | TBD |
| 1 | D2 | Pain survey | TBD | TBD | TBD |
| 1 | D1 | Fake door | TBD | TBD | TBD |
| 2 | D1, D2, D4 | Interviews | TBD | TBD | TBD |
| 3 | F1, F2 | Technical POC | TBD | TBD | TBD |

---

## Key Takeaways

### What We Know

1. **Editing pain is solved** — High confidence from 1,526 reviews
2. **Post-delivery is fragmented** — High confidence from story analysis
3. **Integration is valued** — Medium-high confidence from interviews
4. **Technical feasibility is likely** — Medium confidence from team assessment

### What We Don't Know (Must Validate)

1. **Will they pay?** — Critical unknown, must test before building
2. **Will they switch?** — High-risk assumption, must validate
3. **Is our UX good enough?** — Must test against Pixieset
4. **Will it increase retention?** — Can only validate in beta

### Recommended Next Steps

1. **Week 1:** Launch fake door test + pricing survey
2. **Week 2:** Conduct 10 user interviews
3. **Week 3:** Complete technical POC + go/no-go decision
4. **Week 4-6:** Design sprint + usability testing
5. **Week 7-12:** Beta launch + validation

---

*Assumption Mapping Completed: December 5, 2025*  
*Methodology: Four-Dimension Assumption Framework*  
*Total Assumptions Mapped: 20*  
*Critical Assumptions: 3*  
*High-Risk Assumptions: 7*

