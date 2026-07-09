
# Superstore Sales & Profitability Dashboard (Power BI)

An interactive Power BI dashboard analyzing sales, profit, and returns for a
retail "Superstore" dataset — built to answer a specific set of business
questions from a stakeholder brief (see below).

![Dashboard Demo](https://github.com/DrJay-ux/resources/blob/main/superstore.gif?raw=true) 

## 📋 Business Requirements

The dashboard was built to answer these stakeholder questions:

1. **Metrics** — Sales, Profit, % of Returned Orders, each shown with % change vs. Previous Year (PY).
2. Compare Sales performance vs. Previous Year, over time.
3. Determine the most profitable product and the biggest loss-making product.
4. Find the location(s) where most of the profit is generated.
5. Break down Sales by Segment.

## 🛠 Tools & Skills Used

- **Power BI Desktop** — data modeling, DAX, report design
- **Power Query** — data cleaning and transformation
- **DAX** — time-intelligence measures (YoY %, PY comparisons), calculated KPIs
- **Data visualization** — KPI cards, line/trend charts, map visual, bar charts

## 📊 Dashboard Features

| Section | Description |
|---|---|
| KPI Cards | Sales, Profit, % Returned Orders — each with YoY % change indicator |
| Trend Chart | Sales performance over time, current year vs. previous year |
| Product Profitability | Ranked view highlighting the most profitable and most loss-making products |
| Profit by Geography | Map visual showing where profit is concentrated |
| Sales by Segment | Breakdown of sales across customer segments (Consumer / Corporate / Home Office) |
| Filters | Slicers for Region, Category, Segment, and Date range |

[dashboard_demo](https://github.com/DrJay-ux/resources/blob/main/superstore%20dashboard.jpeg?raw=true)

## 🔑 Key Insights

*(all figures calculated directly from the dataset, US region only — matching the dashboard's default filter)*

- **Total Sales:** $2,297,200.86 (displayed as $2.30M), vs. $1,563,985.61 cumulative through the prior year
- **Total Profit:** $286,397.02 (displayed as $286.40K), vs. $192,957.75 cumulative through the prior year — a **48.4%** increase
- **Returned Orders:** 5.91% of orders (296 of 5,009), vs. 5.75% in the prior-year comparison window
- **Most profitable product:** Copiers — $55,617.82 in profit, the single best-performing sub-category
- **Biggest loss-making product:** Tables — -$17,725.48, the only sub-category losing significant money
- **Other notable performers:** Phones (+$44,515.73) and Accessories (+$41,936.64) round out the top 3; Bookcases (-$3,472.56) and Supplies (-$1,189.10) are minor drags
- **Top profit region:** West ($108,418.45), driven by California ($76,381.39) and New York ($74,038.55) at the state level
- **Weakest state:** Texas, the only state with a significant loss (-$25,729.36)
- **Sales by segment:** Consumer $1,161,401 (50.56%), Corporate $706,146 (30.74%), Home Office $429,653 (18.70%)

> **Note on the YoY comparison:** the "previous year" figures aren't a simple
> single-year comparison (e.g., 2023 vs. 2022) — they're a cumulative total
> through the end of the prior year vs. the all-time cumulative total. This is
> a side effect of how the DAX time-intelligence measure resolves given the
> report's date slicer spans the full 2020–2023 range.


