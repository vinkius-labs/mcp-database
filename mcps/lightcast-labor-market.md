# Lightcast Labor Market MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lightcast-labor-market)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Equip your AI agent to access labor market data, track skill taxonomies, and monitor job titles via the Lightcast API.

## Description
Integrate **Lightcast** (formerly Emsi Burning Glass), the global leader in labor market analytics, directly into your AI workflow. Access the world's most comprehensive skill taxonomy and job title index, track occupation trends and regional labor market summaries, and oversee workforce intelligence using natural language.

### What you can do

- **Skill Taxonomy Oversight** — List and retrieve detailed information for over 30,000 standardized technical and soft skills.
- **Job Title Intelligence** — Monitor standardized job titles and occupations, resolving unique identifiers and regional naming conventions.
- **Market Analysis** — Access high-level labor market summaries for specific economic regions, including job volumes and wage trends.
- **Workforce Auditing** — Retrieve high-level summaries of skill distributions, occupation volumes, and organizational labor market health instantly.

### How it works

1. Connect the Lightcast integration to your AI assistant.
2. Authorize using your Lightcast Client ID and Client Secret (API access required).
3. Orchestrate your workforce planning and labor market research through intuitive conversation.

### Who is this for?

- **HR & Recruiting Teams** — Quickly research skill requirements and standardized job titles on the go.
- **Economic Analysts** — Monitor regional labor market trends and wage data via chat.
- **Educational Institutions** — Map curriculum to official skill taxonomies and occupation demands instantly.


## Available Tools (10)
- **get_lightcast_api_metadata**: Retrieve metadata and authorization status for your Lightcast API connection
- **quick_labor_market_audit**: Retrieve a high-level summary of skills and occupations in the index
- **get_labor_market_region_summary**: Get a high-level labor market summary for a specific economic region
- **get_skill_details**: Get detailed settings and definition for a specific skill
- **list_standardized_job_titles**: List standardized job titles from the Lightcast index
- **list_standardized_occupations**: List occupations categorized by Lightcast (SOC/O*NET compatible)
- **list_economic_regions**: List economic regions and geographies supported by Lightcast
- **list_taxonomically_related_skills**: Identify skills that are taxonomically related to a target skill
- **list_skill_taxonomic_categories**: List high-level taxonomic categories for skills
- **list_labor_market_skills**: g., specialized, common) from the Lightcast API.

List all technical and soft skills in the Lightcast taxonomy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lightcast Labor Market** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for skills related to 'Data Science'."

**🤖 AI Agent:**
> I've found several related skills, including 'Python (Programming Language)', 'Machine Learning', 'SQL (Programming Language)', and 'Data Analysis'. Would you like the detailed definition for Machine Learning?

---

**👤 You:**
> "Show me standardized job titles for 'Software Engineer'."

**🤖 AI Agent:**
> Standardized titles matching 'Software Engineer' include 'Software Developer', 'Full Stack Engineer', 'Back End Developer', and 'Embedded Software Engineer'. Should I pull the occupation code for Full Stack Engineer?

---

**👤 You:**
> "Get a labor market summary for 'New York'."

**🤖 AI Agent:**
> In the New York region, there are currently 1.2 million active job postings. The median advertised wage is $85,000. Top in-demand skills include 'Project Management' and 'Strategic Planning'. Would you like to see the top hiring employers?


## ❓ FAQ

**Q: How do I get Lightcast API credentials?**
You need a registered developer account at the [**Lightcast Developer Portal**](https://lightcast.io/developer). Once approved, you can create an application to receive your **Client ID** and **Client Secret**.

**Q: Which API versions does this support?**
This integration currently utilizes the latest stable versions of the Skills, Titles, and Occupations APIs provided by the Lightcast platform.

**Q: Is global labor data available?**
Yes, Lightcast provides labor market data for various international regions. Availability depends on the specific geographic permissions associated with your API credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lightcast-labor-market](https://vinkius.com/mcp/lightcast-labor-market)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lightcast Labor Market** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lightcast-labor-market` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lightcast Labor Market** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lightcast-labor-market": {
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
