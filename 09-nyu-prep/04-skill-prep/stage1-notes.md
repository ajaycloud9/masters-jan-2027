# Stage 1 — Understanding Data & Analytics

## Study Notes

---

## 1. What is data? What is analytics?

**Data** is a recorded fact or observation with no context attached. A single cell's value. A timestamp. A customer name. On its own, it's meaningless noise.

**Information** is data with context — usually organised, aggregated, or structured so a human can understand it.

**Insight** is a pattern or explanation drawn from information that points toward a cause. It answers "why?" It's the moment data becomes useful.

**Analytics** is the systematic extraction of insight from data. It's the discipline of taking raw facts and turning them into understanding, then decisions.

The difference between a company drowning in data and one that operates on insight is often not access to *more* data, but the rigour of their analytics.

---

## 2. Four types of analytics (the spectrum)

Analytics doesn't answer one question. It answers four, in increasing order of difficulty:

### Descriptive Analytics — "What happened?"

Summarises the current or past state of a business. Dashboards, reports, KPIs. No prediction, no explanation—just observation.

**Example**: "We made $50K in revenue this month. Coffee was 60% of sales. Most transactions were between 8–9 AM."

**Why it matters**: It's the foundation. You can't understand what's happening if you can't *measure* what's happening. Most organisations start here and never leave.

**Tools**: SQL, Excel, Tableau, Power BI, dashboards, reports.

### Diagnostic Analytics — "Why did it happen?"

Investigates causes. Correlates data. Segments it. Drills down. Asks "what changed?" and tests hypotheses.

**Example**: "Revenue dropped 15% last month because we ran fewer promotions, and our competitor launched a new product in our region. Customer acquisition fell 22%, but retention was stable."

**Why it matters**: If you misdiagnose a problem, your solution will fail. Diagnosis prevents wasted money on the wrong fixes.

**Tools**: SQL, Python, statistical tests, correlation analysis, segmentation.

### Predictive Analytics — "What will happen?"

Builds models from historical data to forecast future outcomes. Uses machine learning, statistics, or heuristics.

**Example**: "Based on the last 2 years of data, we predict next quarter's revenue will be $185K, with 68% confidence. Customer churn rate will rise to 8.2% if we raise prices by 5%."

**Why it matters**: Enables proactive decisions instead of reactive ones. Plan inventory, marketing budgets, hiring.

**Tools**: Python, R, machine learning libraries, time-series forecasting, statistical models.

### Prescriptive Analytics — "What should we do?"

Goes beyond prediction. Recommends specific actions and optimises decisions.

**Example**: "To maximise profit next quarter, allocate 40% of marketing budget to customer acquisition (highest ROI), 30% to retention, 20% to upselling. This allocation will generate $210K revenue with minimal risk. Here's the exact sequence of campaigns."

**Why it matters**: This is where analytics becomes a competitive moat. Most competitors react to data. You decide in advance.

**Tools**: Optimisation algorithms, linear programming, simulation, game theory, reinforcement learning.

---

## 3. Classifying data

Data comes in three structural flavours. Understanding which you have determines what you can do with it.

### Structured Data

**What it is**: Rows and columns with a fixed schema. Every record has the same fields.

**Example**:
```
CustomerID | Name | Email | SignupDate | Revenue
101 | Alice | alice@x.com | 2025-01-15 | $450
102 | Bob | bob@y.com | 2025-02-03 | $320
103 | Carol | carol@z.com | 2025-01-20 | $890
```

**Where it lives**: Databases (PostgreSQL, MySQL, Snowflake), spreadsheets, data warehouses.

**Why it matters**: Easiest to query, filter, aggregate. This is the analyst's playground.

### Semi-Structured Data

**What it is**: Has some structure, but flexible. Records can have different fields. Hierarchical.

**Example**:
```json
{
  "customer_id": 101,
  "name": "Alice",
  "orders": [
    {"date": "2025-01-20", "amount": 150, "status": "completed"},
    {"date": "2025-02-05", "amount": 300, "status": "pending"}
  ],
  "preferences": {
    "email_frequency": "weekly",
    "language": "en"
  }
}
```

**Where it lives**: JSON files, XML, APIs, logs.

**Why it matters**: Contains richer information, but requires parsing and extraction before analysis. Modern analytics workflows handle this, but it's slower than structured.

### Unstructured Data

**What it is**: No fixed structure. Text, images, video, audio. Can't fit neatly into rows and columns.

**Example**: Customer reviews, social media posts, product photos, call centre transcripts, emails.

**Where it lives**: Data lakes, cloud storage (S3), document repositories.

**Why it matters**: Contains signal—sentiment, intent, patterns—but extracting it requires NLP, computer vision, or manual annotation. Time-consuming, but increasingly powerful.

---

## 4. Why this matters for you (the beginner)

If you're building a career in analytics, this foundation separates those who last from those who get frustrated.

### Why descriptive is not enough

Many analysts never move past "here's what happened." Dashboards are useful. But a CEO asking "why did revenue drop?" doesn't want to hear "because transactions fell." They want to know the *reason*. That requires diagnostic thinking.

Companies that operate only at the descriptive level are always in reactive mode. Something breaks, they see it on a dashboard, they scramble. No anticipation.

### Why you need to understand the spectrum

Job postings won't say "we need a predictive analyst." They'll say "Data Analyst" (usually descriptive + diagnostic) or "Data Scientist" (predictive + prescriptive). But understanding the spectrum tells you what career path you want and what skills to build.

Diagnostic skills are underrated. Master them, and you become valuable: you're the person who figures out what's actually wrong.

### Why this is learnable

You don't need a PhD to move up the spectrum. You need:
- Curiosity to ask "why?"
- Scepticism about simple answers
- A mental model of how your business works
- Basic SQL / Python skills
- A willingness to dig through data instead of accepting the first correlation you find

---

## 5. Real business examples (mapped to the spectrum)

### Descriptive — Zara's store-level sales reporting

Zara's competitive moat is speed. While competitors take 6–9 months to design and ship a collection, Zara does it in 2 weeks. How? Real-time data visibility.

Store managers carry handheld devices that upload daily POS (point-of-sale) data to headquarters in Spain each night. Every transaction is recorded: item code, size, colour, store ID, timestamp, price point.

No prediction. No complex modelling. Just an extremely fast, extremely clean read of the *present*.

By the next morning, Zara's design and buying teams know exactly which styles are moving at which locations, which sizes are selling, which are sitting. If a style is stalling in one region but flying in another, they reorder or halt production within *hours*. If a size is underselling (e.g., all medium but no large), they adjust the next batch.

**The insight**: Speed and granularity in data collection itself is a competitive advantage. Zara wins on descriptive analytics alone.

### Diagnostic — Netflix and subscription churn

When Netflix sees subscriber cancellations spike in a region, it needs to know *why*. Was it a price increase? A password-sharing crackdown? A competitor's new release? A feature bug?

Netflix analysts correlate the churn spike against:
- Internal events (pricing changes, feature rollouts, content releases, service outages)
- External events (competitor announcements, news coverage, seasonal trends)
- Segmented by cohort: new vs. long-tenure customers, by household type, by device, by content preference

Example: When Netflix enforced password-sharing restrictions in 2022, churn spiked. But Netflix could isolate that the spike was concentrated among secondary account holders (not the primary subscriber), suggesting the feature was working as intended (converting free riders to paid accounts) even as it generated churn.

**The insight**: Diagnosis reveals what you should *actually* be optimising for. Ignoring secondary user data would have looked like a failure; understanding it revealed the real economics.

### Predictive — Netflix's recommendation engine and content greenlight decisions

**Layer 1: What will you watch next?**

Netflix predicts which shows you'll watch based on collaborative filtering (users like you watched X, so you'll like X) and content-based filtering (you watched sci-fi, here's new sci-fi). The model outputs P(watch | user) for every title. Top 50 become your homepage.

Measurement: Did the recommendation increase click-through? Completion rate? Repeat viewing?

**Layer 2: Should we greenlight this $200M show?**

Netflix predicts the addressable audience for a show based on historical viewing patterns. Example: for a spy thriller with actor X, Netflix finds all users who watched spy thrillers or prior films with actor X. It models:
- % of those users who will click
- % who will complete episode 1
- % who will complete the season
- LTV impact (how much longer do they stay subscribed?)

If the math doesn't work—if predicted revenue is less than cost—Netflix doesn't greenlight it. Even critical darlings get cancelled if their audience is too small.

**The insight**: Prediction lets you compete on data instead of instinct.

### Prescriptive — UPS ORION (On-Road Integrated Optimization and Navigation)

Every day, UPS operates 120K vehicles making 100+ stops each. A tiny inefficiency compounds: 1 extra mile × 120K vehicles × 250 working days = 30M excess miles.

ORION solves the Traveling Salesman Problem (TSP) for each driver: given traffic predictions, delivery windows, truck capacity, and hours-of-service regulations, what sequence of stops minimises total distance?

Drivers get a route: "Go to 123 Main St, then 456 Elm Ave, then..." Turn-by-turn optimised. They can deviate, but ORION's suggestion is near-optimal by default.

**Result**: 100M miles saved annually (publicly stated by UPS).

**The insight**: Prescriptive analytics doesn't just predict. It *tells you what to do*.

---

## 6. The decision ladder (from data to business impact)

### What you need to climb it

1. **Clean data** — No typos, duplicates, or NULLs that sink your analysis
2. **The right question** — "How many?" is easier than "Why?" is easier than "What should we do?"
3. **The right tools** — SQL for querying, Python for modelling, Tableau for communication
4. **Domain knowledge** — You can't diagnose problems if you don't understand the business
5. **Intellectual humility** — The first explanation is usually wrong. Dig deeper.

### Where most organisations get stuck

- **Level 1 → 2**: Data quality. Messy data makes insight impossible. Organisations can get stuck here for years.
- **Level 2 → 3**: The leap from reporting to analysis. Dashboards are safe. Diagnosis requires sticking your neck out with a hypothesis.
- **Level 3 → 4**: Prediction requires historical data and pattern recognition. Many organisations don't have clean enough data to forecast reliably.
- **Level 4 → 5**: Prescriptive requires optimisation expertise, and not every decision *can* be optimised (human factors, ethics, risk).

---

## 7. Why organisations climb this curve

Consulting firms like Gartner map the spectrum onto **organisational maturity**. Most companies start purely descriptive (dashboards, reports), slowly build diagnostic capability, and only the most sophisticated organisations (Amazon, Netflix, UPS) operate comfortably at the prescriptive level across most of the business.

### Roles you'll see in job postings

| Role | Focus |
|------|-------|
| **Data Analyst** | Descriptive + diagnostic. SQL, Excel, dashboards — "what happened and why." |
| **Business Analyst** | Translates data into business strategy/process recommendations; more stakeholder-facing. |
| **BI Analyst** | Builds and maintains dashboards/reports (Power BI, Tableau) for ongoing monitoring. |
| **Data Scientist** | Predictive + prescriptive. Statistics, ML, Python. |
| **Marketing / Digital Analyst** | Applies the full spectrum specifically to campaigns, funnels, and customer acquisition. |

---

## 8. Three analytical traps to recognise

The difference between an analyst who gets fooled by data and one who interrogates it.

### Survivorship bias — Abraham Wald & the WWII bombers

The U.S. military mapped bullet holes on *returning* bombers and found damage concentrated on wings, tail, and fuselage — so the obvious move was to armor those areas. Statistician Abraham Wald pointed out the flaw: those planes *survived* being hit there. The real story was in the areas with no bullet holes on returning planes — the engines and cockpit — because planes hit there never made it back.

Wald recommended armoring the areas that looked undamaged.

**Definition**: **Survivorship bias** — drawing conclusions only from the population that "survived" a selection process, while ignoring the invisible population that didn't. Business version: analysing only retained customers to learn "what makes customers happy," missing why churned customers actually left.

### Correlation ≠ causation

Ice cream sales and drowning deaths rise and fall together every year — summer heat (a **confounding variable**) independently drives both. The "spurious correlations" website by statistician Tyler Vigen makes the same point with jokes — like the number of Nicolas Cage films released in a year tracking almost perfectly with U.S. pool drownings. With enough variables, coincidental correlations are guaranteed to appear.

**Rule of thumb**: Every time you find a correlation, ask: is there a plausible causal mechanism, or a hidden third variable driving both?

### Simpson's Paradox — UC Berkeley admissions, 1973

Aggregate data appeared to show men admitted to Berkeley graduate programs at a higher rate than women. Broken down department by department, most individual departments showed no bias — some even favoured women slightly. The gap existed because women disproportionately applied to highly competitive departments with low admission rates for everyone, while men applied more to departments with much higher overall admission rates.

**Definition**: **Simpson's Paradox** — a trend in aggregated data can reverse or vanish when the data is broken into subgroups. Always ask "what happens if I segment this?" before trusting an aggregate number.

---

## 9. More verified real-world cases

### Walmart & Hurricane Frances (2004) — Predictive

Ahead of Hurricane Frances, Walmart mined years of point-of-sale data from prior hurricanes instead of just reactively restocking water and flashlights. Former CIO Linda Dillman found strawberry Pop-Tart sales rose roughly sevenfold ahead of a hurricane, with beer the top-selling item overall. Walmart shipped Pop-Tarts toward stores in the storm's path, and they sold well.

*Source: reported by the New York Times, 2004. Unlike the beer/diapers legend, this case is well documented.*

### Capital One — Information-Based Strategy — Predictive + Prescriptive

Spun off from Signet Banking Corporation in 1994 (operational roots from 1988), founders Richard Fairbank and Nigel Morris built the company around scoring models that priced credit risk by individual borrower rather than a flat rate for everyone. The company practices "test-and-learn," running tens of thousands of experiments a year across product design, marketing, and collections to offer thousands of tailored card variations.

*Notable because analytics was the founding business model — before "data-driven" was a common phrase. A strong reference point for discussing analytics as a competitive moat, not just a support function.*

### Harrah's / Caesars — Total Rewards — Predictive

In 1998, Harrah's brought in Gary Loveman, a Harvard Business School professor, to rebuild marketing around data rather than intuition. Instead of valuing customers by observed past play, Harrah's built a quantitative model predicting customer *future* value — revealing that its most valuable customers weren't flashy high-rollers but regular, middle-income local visitors, which reshaped the entire Total Rewards loyalty strategy.

*A frequently taught customer-analytics case (featured in Thomas Davenport's "Competing on Analytics") because predictive modelling drove a full strategic repositioning, not a marginal tweak.*

### Bonus: John Snow's cholera map (1854)

Arguably the first analytics case study in history. Physician John Snow mapped cholera deaths street-by-street across London and traced the outbreak to a single contaminated water pump on Broad Street — pure descriptive, spatial analytics, a century before computers. It's credited with founding modern epidemiology, and it demonstrates that even the simplest form of analytics (plotting data on a map) can save lives when done rigorously.

---

## 10. Glossary

| Term | Definition |
|------|-----------|
| **Data** | A recorded fact or observation with no context attached. |
| **Information** | Data with context — usually organised or aggregated. |
| **Insight** | A pattern or explanation drawn from information that points toward a cause. |
| **Descriptive analytics** | Summarises what happened. |
| **Diagnostic analytics** | Explains why something happened. |
| **Predictive analytics** | Forecasts what is likely to happen next. |
| **Prescriptive analytics** | Recommends the specific action to take. |
| **Structured data** | Fits neat rows and columns. |
| **Unstructured data** | Has no predefined format. |
| **Semi-structured data** | Has some structure, but flexible (JSON, XML). |
| **Primary data** | Collected yourself for your purpose. |
| **Secondary data** | Collected by someone else for a different purpose. |
| **Survivorship bias** | Drawing conclusions only from the population that "survived" a selection process. |
| **Confounding variable** | A hidden third factor that drives two variables to move together without either causing the other. |
| **Simpson's Paradox** | A trend in aggregate data that reverses once the data is segmented. |

---

## 11. Keep learning

- **[What Is Data Analytics? — An Introduction (Full Guide)](https://www.youtube.com/watch?v=yZvFH7B6gKI)** — CareerFoundry · beginner overview of the field and the data analysis process
- **[What is the DIKW Pyramid? + Example](https://www.youtube.com/watch?v=OclzV4GA-Xc)** — Concise walkthrough of the Data–Information–Knowledge–Wisdom hierarchy
- **[Descriptive vs Diagnostic vs Predictive vs Prescriptive Analytics](https://www.youtube.com/watch?v=QoEpC7jUb9k)** — Chris Dutton · the four-part analytics spectrum with business examples
- **[Structured vs Unstructured Data Explained](https://www.youtube.com/watch?v=Av4BsJmqUQ8)** — Tech Made Simple · visual breakdown with everyday examples
- **[How Target Predicted Pregnancy Using Shopping Data](https://www.youtube.com/watch?v=8MFtrgw5Ihc)** — The purchase-pattern prediction score and its business impact

---

**Compiled study notes — Stage 1: Understanding Data & Analytics. Next up: Stage 2, How Businesses Generate Data.**