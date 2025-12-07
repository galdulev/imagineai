# Imagen AI - ICP Discovery Research Plan
## Using AI-Powered Research Methods (Cursor AI, Web Scraping, Analysis)

---

## Research Objective

Identify and validate Imagen AI's true Ideal Customer Profile (ICP), distinguishing between:
- **End users** (photographers using the tool)
- **Actual paying customers** (platforms/enterprises like Airbnb, real estate companies)
- **Decision makers** (who signs the contracts)

---

## Phase 1: Public Intelligence Gathering

### 1.1 LinkedIn Research

**What to Find:**
- Imagen AI employees and their titles
- Sales team structure (Enterprise vs. SMB focus?)
- Customer Success team - who are they supporting?
- Job postings mentioning customer types

**AI Research Tasks:**
```
Search queries:
- "Imagen AI" site:linkedin.com
- "Imagen AI" "enterprise" OR "partnerships"
- "Imagen AI" "customer success" job posting
- Imagen AI employees → check who they connect with
```

**Key Signals:**
| Signal | Indicates |
|--------|-----------|
| "Enterprise Account Executive" roles | B2B enterprise focus |
| "Partnerships Manager" | Platform/API deals |
| "Community Manager" | Prosumer/individual focus |
| Employees previously at Airbnb, Zillow, etc. | Target market hints |

---

### 1.2 Press & Media Scraping

**Sources to Scrape:**
- TechCrunch, VentureBeat, Forbes
- Photography industry publications (PetaPixel, Fstoppers)
- Real estate tech publications
- Startup/funding news sites

**Search Queries:**
```
"Imagen AI" + "partnership"
"Imagen AI" + "Airbnb"
"Imagen AI" + "enterprise"
"Imagen AI" + "raised" OR "funding"
"Imagen AI" + "customers include"
"Imagen AI" + "case study"
```

**What to Extract:**
- Named customers in press releases
- Partnership announcements
- Funding round details (investors often hint at market focus)
- Quotes from leadership about target market

---

### 1.3 Website & Marketing Analysis

**Pages to Analyze:**
| Page | What to Look For |
|------|------------------|
| `/enterprise` or `/business` | Enterprise offering exists? |
| `/pricing` | Tiers suggest individual vs. enterprise? |
| `/case-studies` | Named customers, company sizes |
| `/partners` or `/integrations` | Platform partnerships |
| `/about` or `/careers` | Team structure, job roles |
| `/api` or `/developers` | API offering = platform play |

**Technical Analysis:**
```bash
# Check for enterprise/API pages
curl -s https://imagen-ai.com/sitemap.xml | grep -i "enterprise\|api\|business\|partners"

# Check robots.txt for hidden sections
curl -s https://imagen-ai.com/robots.txt
```

**Marketing Language Signals:**
- "For photographers" = B2C/prosumer
- "For teams" / "For businesses" = B2B SMB
- "Enterprise solutions" / "API access" = B2B Enterprise
- "Platform partners" = B2B2C

---

### 1.4 Review & Community Mining

**Platforms to Scrape:**

#### App Store Reviews
```
Sources:
- Apple App Store reviews
- Google Play reviews (if mobile app exists)

Extract:
- User self-identification ("I'm a wedding photographer...")
- Company mentions ("Our agency uses...")
- Use case descriptions
```

#### Software Review Sites
```
Sites:
- G2.com/products/imagen-ai
- Capterra.com
- TrustRadius
- GetApp

Extract:
- Company size of reviewers
- Industry of reviewers
- Job titles of reviewers
- Use case descriptions
```

#### Community Forums
```
Sources:
- Reddit: r/photography, r/WeddingPhotography, r/RealEstatePhotography
- Facebook Groups: Wedding photographers, Real estate photographers
- Photography forums: DPReview, Fred Miranda

Search:
- "Imagen AI" mentions
- Who is talking about it?
- What context are they using it in?
```

---

### 1.5 Social Media Intelligence

**Twitter/X Analysis:**
```
Search queries:
- "Imagen AI" from:airbnb
- "Imagen AI" from:zillow
- "@imagenai" mentions
- "Imagen AI" filter:verified (brand accounts)

Analyze:
- Who follows @imagenai?
- Who do they follow back?
- What accounts do they engage with?
```

**LinkedIn Company Page:**
```
Analyze:
- Followers by industry
- Followers by company size
- Content themes (who are they speaking to?)
- Engagement patterns
```

---

## Phase 2: Technical & Product Intelligence

### 2.1 API & Integration Research

**Check for API Documentation:**
```
URLs to check:
- imagen-ai.com/api
- imagen-ai.com/developers
- developers.imagen-ai.com
- api.imagen-ai.com
- docs.imagen-ai.com
```

**If API exists, analyze:**
- Pricing (per-image? enterprise only?)
- Rate limits (suggests volume expectations)
- Authentication (API keys = B2B focus)
- Use case examples in docs

**Integration Partners:**
```
Check:
- Adobe Exchange marketplace listing
- Zapier integrations
- Any platform marketplace listings
```

---

### 2.2 Job Posting Analysis

**Sources:**
- Imagen AI careers page
- LinkedIn Jobs
- Indeed, Glassdoor
- AngelList/Wellfound

**What Job Titles Reveal:**

| Job Title | ICP Signal |
|-----------|------------|
| Enterprise Sales | Large company customers |
| SMB Account Executive | Small business focus |
| Partnerships Manager | Platform/integration deals |
| Developer Relations | API/platform customers |
| Community Manager | Individual users |
| Customer Success (Enterprise) | Big accounts exist |

**Job Description Keywords:**
```
Look for:
- "Enterprise accounts"
- "Platform partnerships"
- "API customers"
- "Photography studios"
- "Real estate"
- "E-commerce"
- Specific company names as examples
```

---

### 2.3 Competitor Customer Analysis

**Identify Competitors:**
- Luminar Neo (Skylum)
- Topaz Labs
- Photoroom
- Remove.bg
- Let's Enhance

**Research Their Customers:**
```
For each competitor:
- Who are their enterprise customers?
- What industries do they serve?
- Do they have API/platform offerings?
- What case studies do they publish?
```

**Logic:** If competitors serve Airbnb, real estate platforms, e-commerce → Imagen AI likely targets same markets.

---

## Phase 3: Direct Intelligence

### 3.1 Pricing Page Analysis

**Scrape & Analyze:**
```
Extract:
- Tier names (Individual, Team, Enterprise, API)
- Pricing structure (per user, per image, custom)
- Feature differences between tiers
- "Contact Sales" triggers (= enterprise deals)
- Volume discounts mentioned
```

**Pricing Signals:**

| Pricing Element | ICP Signal |
|-----------------|------------|
| Per-image pricing | High-volume platform customers |
| Per-seat pricing | Team/agency customers |
| "Contact us" for pricing | Enterprise deals |
| Free tier + paid | Prosumer/PLG model |
| Annual contracts only | Enterprise focus |

---

### 3.2 Case Study & Testimonial Mining

**Extract from Website:**
```
For each case study/testimonial:
- Company name
- Company size
- Industry
- Use case
- Volume mentioned
- ROI/results quoted
- Job title of person quoted
```

**Categorize:**
```
Categories:
□ Individual photographer
□ Photography studio/agency
□ Real estate company
□ Platform (Airbnb, Zillow, etc.)
□ E-commerce company
□ Other enterprise
```

---

### 3.3 Funding & Investor Research

**Sources:**
- Crunchbase
- PitchBook (if accessible)
- AngelList
- News articles about funding rounds

**What to Extract:**
```
- Total funding raised
- Investors (what's their portfolio focus?)
- Funding round press releases (often mention traction/customers)
- Investor quotes about the company
```

**Investor Portfolio Analysis:**
```
If investors also invested in:
- Real estate tech → real estate ICP
- E-commerce tools → e-commerce ICP
- Creator economy → prosumer ICP
- Enterprise SaaS → B2B enterprise ICP
```

---

## Phase 4: Synthesis & Validation

### 4.1 ICP Hypothesis Matrix

| Potential ICP | Evidence For | Evidence Against | Confidence |
|---------------|--------------|------------------|------------|
| Individual Photographers | | | |
| Photography Studios/Agencies | | | |
| Real Estate Platforms | | | |
| Airbnb / Vacation Rentals | | | |
| E-commerce Platforms | | | |
| Enterprise (Other) | | | |

---

### 4.2 Customer Segmentation Framework

**Segment by:**

```
1. BUYER TYPE
   □ Individual (B2C)
   □ Small Business (B2B SMB)
   □ Enterprise (B2B Enterprise)
   □ Platform (B2B2C)

2. INDUSTRY
   □ Wedding/Event Photography
   □ Portrait Photography
   □ Real Estate
   □ E-commerce/Product
   □ Travel/Hospitality
   □ Other: _______

3. VOLUME
   □ <1,000 images/month
   □ 1,000-10,000 images/month
   □ 10,000-100,000 images/month
   □ 100,000+ images/month

4. DECISION MAKER
   □ Photographer (individual)
   □ Studio Owner
   □ Marketing/Brand Manager
   □ Operations/Tech Lead
   □ C-Suite
```

---

### 4.3 Validation Checklist

**Before finalizing ICP, validate:**

- [ ] Multiple sources confirm customer type
- [ ] Pricing model aligns with ICP
- [ ] Product features match ICP needs
- [ ] Marketing messaging targets ICP
- [ ] Sales team structure supports ICP
- [ ] Case studies represent ICP
- [ ] Competitors confirm market exists

---

## Research Execution Checklist

### Week 1: Public Intelligence
- [ ] LinkedIn company & employee research
- [ ] Press/media article scraping
- [ ] Website analysis (all pages)
- [ ] Review site mining (G2, Capterra)

### Week 2: Technical & Product Intel
- [ ] API/developer documentation check
- [ ] Job posting analysis
- [ ] Competitor customer research
- [ ] Pricing page deep dive

### Week 3: Direct Intelligence
- [ ] Case study extraction
- [ ] Testimonial categorization
- [ ] Funding/investor research
- [ ] Social media analysis

### Week 4: Synthesis
- [ ] Complete ICP hypothesis matrix
- [ ] Validate with multiple sources
- [ ] Create final ICP document
- [ ] Identify gaps needing further research

---

## Tools & Resources

### Web Scraping
- **Cursor AI**: Code generation for scrapers
- **Beautiful Soup / Scrapy**: Python scraping
- **Puppeteer / Playwright**: JavaScript rendering
- **Apify**: Pre-built scrapers

### Data Sources
- **Crunchbase**: Funding, investors
- **LinkedIn Sales Navigator**: Employee/company intel
- **SimilarWeb**: Traffic & audience data
- **BuiltWith**: Technology stack

### Analysis
- **Claude/GPT**: Text analysis, summarization
- **Google Sheets**: Data organization
- **Notion**: Research synthesis

---

## Output: ICP Document Template

```markdown
# Imagen AI - Ideal Customer Profile

## Primary ICP
**Customer Type:** [Platform / Enterprise / SMB / Individual]
**Industry:** [Real Estate / E-commerce / Photography / etc.]
**Company Size:** [Revenue range / Employee count]
**Decision Maker:** [Title/Role]
**Budget:** [Price point they pay]

## Key Characteristics
- Characteristic 1
- Characteristic 2
- Characteristic 3

## Pain Points We Solve
1. Pain point 1
2. Pain point 2
3. Pain point 3

## Evidence Sources
- Source 1: [link/reference]
- Source 2: [link/reference]

## Secondary ICPs
[List additional customer segments]
```

---

*This research plan enables systematic discovery of Imagen AI's true ICP using publicly available data and AI-powered analysis tools.*

