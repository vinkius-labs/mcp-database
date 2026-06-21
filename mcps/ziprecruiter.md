# ZipRecruiter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ziprecruiter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search millions of job listings on ZipRecruiter — find roles by keyword, location, and salary directly from your AI agent.

## Description
Connect your **ZipRecruiter** API to any AI agent to streamline your job search or recruitment research through natural conversation.

### What you can do

- **Targeted Job Search** — Find specific roles using keywords like 'Frontend Developer' or 'Project Manager' across any location.
- **Geographic Filtering** — Narrow down searches to specific cities, states, or zip codes with adjustable search radiuses.
- **Salary Refinement** — Filter results to only show opportunities that meet your minimum annual salary requirements.
- **Recency Control** — Focus on the freshest opportunities by filtering for jobs posted within a specific number of days.
- **Pagination Support** — Seamlessly browse through large result sets using page and results-per-page controls.

### How it works

1. Subscribe to this server
2. Enter your ZipRecruiter API Key
3. Start searching for jobs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Job Seekers** — quickly find and filter opportunities without manual browsing
- **Recruiters & HR** — analyze market trends and competitor listings in real-time
- **Career Coaches** — help clients find relevant roles based on specific salary and location criteria


## Available Tools
- **ziprecruiter_search_jobs**: Search for jobs on ZipRecruiter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZipRecruiter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Software Engineer' jobs in Austin, Texas."

**🤖 AI Agent:**
> I've found several Software Engineer positions in Austin. Top results include roles at TechFlow and CloudScale. Would you like more details on any of these?

---

**👤 You:**
> "Find remote Marketing roles posted in the last 3 days with a minimum salary of 90000."

**🤖 AI Agent:**
> Searching... I found 3 remote Marketing positions posted recently that meet your salary criteria. Companies include GrowthLabs and BrandSync. Shall I list the full descriptions?

---

**👤 You:**
> "Show me the second page of 'Data Scientist' jobs in San Francisco."

**🤖 AI Agent:**
> Fetching the second page of results for Data Scientist roles in San Francisco... Here are the next 20 listings, including roles at InsightAI and DataCore.


## ❓ FAQ

**Q: Can I filter jobs by a specific minimum salary?**
Yes! You can use the `refine_by_salary` parameter in the `search_jobs` tool to set a minimum annual salary floor for your results.

**Q: How do I search for jobs within a certain distance from my location?**
When using `search_jobs`, provide a `location` and set the `radius_miles` parameter to your preferred distance (default is 25 miles).

**Q: Is it possible to see only the most recently posted jobs?**
Absolutely. Use the `days_ago` parameter in the `search_jobs` tool to limit results to jobs posted within the last N days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ziprecruiter](https://vinkius.com/mcp/ziprecruiter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZipRecruiter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ziprecruiter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZipRecruiter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ziprecruiter": {
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
