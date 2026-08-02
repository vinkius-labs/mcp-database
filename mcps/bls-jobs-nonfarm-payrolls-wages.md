# BLS Jobs — Nonfarm Payrolls & Wages MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-jobs-nonfarm-payrolls-wages)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Access the definitive source for US employment growth. Query Nonfarm Payrolls, private sector job creation, and average hourly earnings tracked by the BLS Current Employment Statistics (CES) program.

## Description
Connect to the exact datasets used by Wall Street and the Federal Reserve to monitor US Job growth. The Bureau of Labor Statistics Jobs MCP gives your agent direct access to the Current Employment Statistics (CES) program.

### What you can do
- **Nonfarm Payrolls** — Fetch exactly how many jobs were added to the US economy each month.
- **Sector Breakdowns** — Drill down into tech, hospitality, or construction employment trends.
- **Wages & Earnings** — Query the average hourly earnings to monitor wage growth and labor tightness.

### How it works
1. Sign up for a free BLS Developer API Key
2. Provide the key in the settings
3. Ask your AI to parse nonfarm payroll additions or track total average hourly wages over the last 10 years.

### Who is this for?
- **Financial Analysts & Traders** — Build models off the monthly jobs report (NFP)
- **HR Professionals & Recruiters** — Monitor macro labor trends
- **Journalists** — Fact-check employment cycles instantly


## Available Tools (2)
- **get_nonfarm_payrolls**: Key metric for forecasting Federal Reserve interest rate movements.

Get Total Nonfarm Payroll employment (CES0000000001)
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Jobs — Nonfarm Payrolls & Wages** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the total Nonfarm Payroll growth in the last quarter?"

**🤖 AI Agent:**
> 📊 **Nonfarm Payrolls (CES0000000001)**

- **Oct**: +150,000 jobs
- **Nov**: +199,000 jobs
- **Dec**: +216,000 jobs

Total added in Q4: **565,000 jobs**, showing accelerating momentum toward the end of the year.

---

**👤 You:**
> "Show me the average hourly earnings trend for all private workers."

**🤖 AI Agent:**
> 💵 **Average Hourly Earnings (CES0500000003)**

Average hourly earnings for all employees on private nonfarm payrolls rose to **$34.27**. Over the past 12 months, average hourly earnings have increased by **4.1%**, keeping wage growth solidly above the current inflation rate.

---

**👤 You:**
> "Which sector added the most jobs in December?"

**🤖 AI Agent:**
> 📊 **Sector Job Growth (Dec)**

1. **Government**: +52,000 jobs
2. **Leisure and Hospitality**: +40,000 jobs
3. **Health Care**: +38,000 jobs

These three sectors accounted for over 60% of all nonfarm payroll additions that month.


## ❓ FAQ

**Q: How do I get started?**
Subscribe, create a Free BLS Account at **data.bls.gov/registrationEngine**, and enter your API Key. No complex coding required — your AI will automatically parse the SeriesIDs for Nonfarm Payrolls and wages, retrieving the exact macro snapshots.

**Q: Are these numbers seasonally adjusted?**
Yes, by default the AI interacts with the Seasonally Adjusted (SA) SeriesIDs for Nonfarm Payrolls, allowing you to track macro trends cleanly without the noise of holiday hiring surges.

**Q: Does this include agricultural (farm) jobs?**
No. The CES (Current Employment Statistics) specifically tracks Nonfarm payrolls, representing about 80% of workers who produce the entire Gross Domestic Product of the United States.

**Q: Can I drill down into specific industries?**
Absolutely. Ask your agent to fetch CES data for the 'Information' sector, 'Construction', or 'Leisure and Hospitality' to identify precisely which parts of the economy are hiring or firing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-jobs-nonfarm-payrolls-wages](https://vinkius.com/mcp/bls-jobs-nonfarm-payrolls-wages)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BLS Jobs — Nonfarm Payrolls & Wages** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bls-jobs-nonfarm-payrolls-wages` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BLS Jobs — Nonfarm Payrolls & Wages** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bls-jobs-nonfarm-payrolls-wages": {
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
