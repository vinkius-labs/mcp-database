# DonorsChoose MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donorschoose)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Equip your AI agent to search classroom projects, track funding needs, and monitor educational proposals via the DonorsChoose API.

## Description
Integrate **DonorsChoose**, the leading crowdfunding platform for public school teachers, directly into your AI workflow. Search for classroom projects across the US, filter by state, subject, or ZIP code, monitor urgent funding needs, and retrieve detailed information for educational proposals using natural language.

### What you can do

- **Project Discovery** — Search for classroom projects using keywords, subjects, or specific geographic locations (states and ZIP codes).
- **Funding Oversight** — Monitor projects that are close to their expiration or have high urgency to identify immediate support needs.
- **Proposal Intelligence** — Retrieve detailed information for specific classroom projects, including school details and itemized resource lists.
- **Newest Opportunity Tracking** — List the most recently posted classroom proposals to identify new funding opportunities across the organization.

### How it works

1. Connect the DonorsChoose integration to your AI assistant.
2. Authorize using your DonorsChoose API Key (you can use 'DONORSCHOOSE' for public access).
3. Orchestrate your educational support and project research through intuitive conversation.

### Who is this for?

- **Philanthropy Managers** — Quickly identify classroom projects in specific regions or subjects for support on the go.
- **Educational Researchers** — Gather detailed proposal metadata and school information via chat.
- **Community Organizers** — Monitor local classroom funding needs and urgent projects instantly.


## Available Tools (10)
- **get_donorschoose_api_metadata**: Retrieve metadata for the current API connection
- **get_classroom_project_details**: Get detailed information for a specific classroom project
- **quick_regional_funding_audit**: Retrieve a high-level summary of active projects in a region
- **list_high_poverty_needs**: Identify projects from schools in high-poverty areas
- **list_latest_classroom_proposals**: List the most recently posted classroom projects
- **list_projects_by_state**: List classroom projects in a specific US state (e.g., NY, CA)
- **list_projects_by_subject**: List projects filtered by subject area (e.g., Literacy, Math)
- **list_urgent_funding_needs**: Identify projects that are close to their expiration or have high urgency
- **search_projects_by_zipcode**: Search for classroom projects within a specific US ZIP code
- **search_classroom_projects**: Search for DonorsChoose classroom projects using keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DonorsChoose** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for classroom projects in New York about 'Literacy'."

**🤖 AI Agent:**
> I've found 8 projects in New York focused on Literacy, including 'Books for Our Classroom Library' and 'Reading Corner Rug'. Would you like to see the funding goal for any of these?

---

**👤 You:**
> "Show me urgent projects near ZIP code '90210'."

**🤖 AI Agent:**
> I've identified 3 urgent projects near 90210, including a science lab request at Beverly Hills High. One project is only $50 away from being fully funded. Should I pull the details for that one?

---

**👤 You:**
> "List the newest classroom proposals."

**🤖 AI Agent:**
> The latest proposals include projects for 'Special Education Sensory Tools' in Texas and 'Music Room Instruments' in Florida. Both were posted in the last hour. Would you like to see the school names for these new projects?


## ❓ FAQ

**Q: How do I get a DonorsChoose API Key?**
For general public access, you can use the API key 'DONORSCHOOSE'. If you require a unique key for high-volume use, you can apply for one through the DonorsChoose developer site.

**Q: Can the agent make donations directly?**
This integration currently focuses on searching and auditing project data. Making actual donations should be completed via the project links provided by the agent on the DonorsChoose website.

**Q: Which geographical areas are covered?**
DonorsChoose covers public and charter school classroom projects across all 50 US states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donorschoose](https://vinkius.com/mcp/donorschoose)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DonorsChoose** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `donorschoose` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DonorsChoose** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "donorschoose": {
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
