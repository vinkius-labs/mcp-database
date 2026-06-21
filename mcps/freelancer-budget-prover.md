# Freelancer Budget Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freelancer-budget-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A designer charged $100/hour and calculated annual income as $208,000. Then reality arrived. Billable hours dropped to 1,352 after admin, sales, and vacation. Gross: $135,200. Self-employment tax, health insurance, tools, and accounting consumed $60,685. Net take-home: $74,515. Effective hourly rate: $35.82. Three clients paid 45 days late. This tool forces five budget axes: realistic revenue, complete costs, cash flow buffers, minimum viable pricing, and profitability with scope creep analysis.

## Description
## The Problem

1. **Revenue Fantasy** — hourly × 2,080 ignoring 30-40% non-billable time.
2. **Invisible Costs** — SE tax 15.3%, health, tools, retirement = 30-45% of gross.
3. **Cash Flow Blindness** — 42% of invoices paid late. Zero income during illness.
4. **Underpricing** — 'market rate' instead of minimum viable rate from costs.
5. **Scope Creep** — 20h project → 35h = 43% effective rate reduction.


## Available Tools (1)
- **validate_freelancer_budget**: Freelancer finances are uniquely brutal — irregular income, no employer benefits, self-employment tax, and the constant pressure to underprice. You must: (1) project REVENUE with utilization — billable hours × rate × utilization rate (60-70%, never 100%). The 30-40% non-billable time is real: proposals, admin, marketing, learning, contract gaps. Hourly × 2,080 is a fantasy, (2) account for ALL COSTS — self-employment tax (15.3%), income tax (bracket-dependent), health insurance ($400-800/mo), liability insurance, tools/software, accounting, retirement (no employer match), home office, professional development. Total hidden costs: 35-45% of gross revenue, (3) plan CASH FLOW for irregular income — payment terms (Net-30/60/90), late payment rate (42% per Freelancers Union), seasonal gaps (2 months/year average), illness coverage (zero sick days), 3-6 month emergency fund, (4) calculate PRICING from costs — minimum viable rate = total annual costs ÷ (1 - margin) ÷ billable hours. NOT "what others charge" — YOUR costs determine YOUR floor. Value-based pricing for the ceiling, (5) analyze PROFITABILITY on ALL hours — effective hourly = net income ÷ ALL hours worked (billable + non-billable). Scope creep impact: free work hours × hourly rate = lost revenue. If rejected, your freelancer math will lead to burnout or insolvency.

Structured reflection tool for realistic freelancer financial planning — forces revenue modeling with utilization rates, complete cost accounting, cash flow planning for irregular income, cost-plus pricing calculation, and profitability analysis on ALL hours worked. Catches Revenue Fantasy (hourly rate × 2,080 hours — the fantasy that ignores utilization. A freelancer billing $150/hr at 65% utilization earns $101,400, not $312,000. The 35% non-billable time includes proposals, admin, accounting, marketing, learning, and the 2-week gaps between contracts that nobody plans for), Invisible Costs (forgetting that self-employment tax is 15.3%, health insurance is $400-800/month, liability insurance is $1,200/year, tools are $3,600/year, accounting is $2,400/year, retirement contributions have no employer match — freelancers pay the employer AND employee share of everything. Total hidden costs: 35-45% of gross revenue), Cash Flow Blindness (ignoring that 42% of invoices are paid late per Freelancers Union, Net-60 means you work in January and get paid in March, seasonal gaps mean 2 months/year with zero income, and illness means zero revenue with no sick days), Underpricing (using "market rate" instead of calculating the minimum viable rate — total costs ÷ (1 - margin) ÷ billable hours. "What others charge" ignores YOUR costs), and Scope Creep Exposure (undefined deliverables, unlimited revisions, and "quick favors" — scope creep costs the average freelancer 15-20% of billable revenue per year. Every hour of free work is an hour you cannot bill). Call once per freelancer financial plan or pricing decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freelancer Budget Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I charge $95/hour. Potential income: $95 × 2,080 = $197,600. Low expenses. Clients pay on time."

**🤖 AI Agent:**
> REVENUE_FANTASY — 2,080h ignores 35% non-billable. 'Low expenses' ignores $75K+ invisible costs. 'Clients pay on time' contradicts 42% late rate.

---

**👤 You:**
> "Revenue: $95/hr × 1,352h (65%) = $128,440. Costs: $79,764 total. Net: $48,676. Cash flow: Net-30, 18% late, $24K emergency. Pricing: min $79.20/hr, current $95. Profit: 37.9% margin, scope creep 3/12 projects +40%."

**🤖 AI Agent:**
> BUDGET_PROVEN — All five axes validated.

---

**👤 You:**
> "Revenue: $110/hr × 1,400h. Costs: $76,462. Cash flow: 'clients pay on time.' Pricing: 'based on what competitors charge.'"

**🤖 AI Agent:**
> CASHFLOW_BLIND — No late payment buffer, no emergency fund, no seasonal gap plan. Pricing from competitors not from YOUR costs.


## ❓ FAQ

**Q: Why is $100/hr × 2,080 a fantasy?**
Freelancers are billable 60-70% of working hours after admin, sales, learning, and vacation. Real: 1,352 hours × $100 = $135,200 — not $208,000.

**Q: How do I calculate minimum viable rate?**
Total costs ($82K) ÷ (1 - target margin 20%) = $102,500 ÷ 1,300 billable hours = $78.85/hr minimum. Below this you lose money.

**Q: How does scope creep destroy profitability?**
20h project at $100/hr = $2,000. Client adds 'small changes.' Actual: 35h. Effective rate: $57.14/hr — 43% reduction. If minimum viable is $79/hr, you worked 15 hours below cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freelancer-budget-prover](https://vinkius.com/mcp/freelancer-budget-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freelancer Budget Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freelancer-budget-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freelancer Budget Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freelancer-budget-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
