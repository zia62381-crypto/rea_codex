# Triple Whale — Summary Dashboard, KPI Cards, Sales & Profit Charts

**Unofficial independent recreation.** This project recreates visible features of the [Triple Whale](https://www.triplewhale.com/) Summary dashboard using original React source code and deterministic sample data. It does not contain Triple Whale's proprietary source code, internal API credentials, or real store analytics.

## Implemented

- Responsive Summary / Overview dashboard with side navigation
- Six KPI cards: revenue, net profit, orders, profit margin, ad spend, blended ROAS
- Per-card mini sales/profit sparklines
- Interactive sales area chart and net-profit bar chart
- Previous-period comparison line for sales
- Date range filter: last 7, 30, or 90 days
- Marketing channel performance table and revenue shares
- Clear **demo data** indicators throughout

## Run

Node.js 18+ and npm are required.

```bash
npm install
npm run dev
```

Follow the localhost URL printed by Vite. To build: `npm run build`.

## File layout

```
Triple-Whale-Main-Dashboard-KPI-Sales-Profit/
├── README.md
├── REA_METHOD.md
├── package.json
├── index.html
├── src/
│   ├── main.jsx
│   ├── App.jsx
│   ├── data.js
│   └── style.css
└── .gitignore
```

## Data & metric caveats

All store values are generated inside `src/data.js` and have no business significance. For example, the sample net profit formula is `profit = sales * 0.38 - advertising_spend`. In real production use, cost of goods, refunds, taxes, shipping, platform fees, and other operating costs may matter. The demo's margin and blended ROAS formulas are illustrative, not necessarily equivalent to official Triple Whale definitions. KPI change percentages other than the revenue comparison are illustrative fixed demo labels. The channel table is a static example and does not respond to the date filter.

## Public references

- [Triple Whale — Track KPIs with the Summary Dashboard](https://kb.triplewhale.com/en/articles/5725275-track-kpis-with-the-summary-dashboard)
- [Triple Whale navigation guide](https://kb.triplewhale.com/en/articles/12117524-a-guide-to-triple-whale-s-navigation)
- [Triple Whale ecommerce dashboard](https://www.triplewhale.com/blog/ecommerce-dashboard)
- [Requested REA skill](https://github.com/zia62381-crypto/rea_codex/tree/main/REA_skills_Codex-main/REA-Skills/reverse-engineer-anything)

Read `REA_METHOD.md` for scope and analysis limits.

## Verification status

Files have been committed to GitHub. A complete local `npm install && npm run build` could not be completed in the authoring environment because dependency acquisition timed out. Run the commands above in an environment with npm registry access to verify the complete build.
