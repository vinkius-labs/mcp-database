# Jooble MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jooble)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search millions of job vacancies across the globe from Jooble directly within your AI agent.

## Description
Connect your AI agent to **Jooble**, one of the world's largest job search engines, to streamline your recruitment or job-hunting process through natural conversation.

### What you can do

- **Global Job Search** — Access vacancies aggregated from thousands of job boards, corporate websites, and social networks.
- **Targeted Filtering** — Use specific keywords, job titles, or company names to find the perfect match.
- **Geographic Precision** — Filter results by city, state, zip code, or country to find local or international opportunities.
- **Market Analysis** — Quickly gather data on job trends and availability in specific industries or regions.

### How it works

1. Subscribe to this server
2. Enter your Jooble API Key
3. Start searching for opportunities from Claude, Cursor, or any MCP-compatible client

No more manual searching across dozens of job sites. Your AI acts as a dedicated recruiter or career assistant, bringing the best opportunities directly to your workflow.

### Who is this for?

- **Job Seekers** — find relevant openings and compare roles without leaving your workspace
- **Recruiters & HR** — monitor competitor listings and market availability for specific roles
- **Career Coaches** — quickly gather job market data to provide better advice to clients


## Available Tools (1)
- **search_jooble_jobs**: Search for jobs on Jooble


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jooble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Data Scientist' jobs in Berlin."

**🤖 AI Agent:**
> I've found several Data Scientist positions in Berlin. Here are the top listings from Jooble, including roles at TechHub and DataCorp.

---

**👤 You:**
> "Find remote 'Project Manager' roles."

**🤖 AI Agent:**
> Searching for remote Project Manager roles... I've retrieved 10 active vacancies that match your criteria. Would you like to see the details for the most recent one?

---

**👤 You:**
> "Look for job openings at 'Microsoft' in the United States."

**🤖 AI Agent:**
> I've identified the latest job openings at Microsoft across the US. Notable positions include 'Senior Software Engineer' in Redmond and 'Cloud Architect' in New York.


## ❓ FAQ

**Q: How can I find jobs in a specific location?**
Use the `search_jooble_jobs` tool and provide the city, state, or country in the `location` field to filter results geographically.

**Q: Can I search for jobs at a specific company?**
Yes, simply include the company name in the `keywords` parameter of the `search_jooble_jobs` tool to narrow down your search.

**Q: Is it possible to find remote work using this tool?**
Absolutely. You can add 'remote' to your `keywords` or `location` when using the `search_jooble_jobs` tool to find work-from-home opportunities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jooble](https://vinkius.com/mcp/jooble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jooble** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jooble` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jooble** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jooble": {
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
