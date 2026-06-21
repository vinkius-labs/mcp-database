# GlobalGiving MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/globalgiving)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search nonprofit projects, track crowdfunding goals, and oversee global charities via AI agents with GlobalGiving.

## Description
Connect your AI agent to the **GlobalGiving** global marketplace to automate nonprofit project discovery and charity research through the Model Context Protocol (MCP). GlobalGiving is the first and largest global crowdfunding community that connects nonprofits, donors, and companies in nearly every country. This MCP server enables you to search for grassroots projects by theme or country, retrieve detailed project summaries, and manage charity organization data directly through natural conversation.

### Key Features

- **Project Discovery** — Search for thousands of grassroots projects using keywords, themes (education, health, environment), or ISO country codes.
- **Charity Oversight** — Access detailed mission statements and profile information for vetted nonprofit organizations worldwide.
- **Crowdfunding Tracking** — Retrieve real-time progress for project goals, including total amounts raised and remaining funding needed.
- **Thematic Exploration** — Filter active projects by specific impact areas like disaster recovery, women's empowerment, or climate action.
- **Regional Insights** — Discover and list active initiatives in specific countries to understand local impact and needs.
- **Vetted Transparency** — Access metadata for verified organizations to ensure your philanthropic research is backed by due diligence.
- **Real-time Synchronization** — Keep your nonprofit and impact data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GlobalGiving API Key (request one from the GlobalGiving developer portal)
3. Start discovering and tracking nonprofit projects from Claude, Cursor, or any MCP client

### Who is this for?

- **CSR & Philanthropy Leads** — quickly research potential nonprofit partners or track project milestones without manual portal navigation.
- **Impact Researchers** — get a real-time overview of grassroots initiatives in specific regions or themes via simple AI commands.
- **Nonprofit Enthusiasts** — automate the discovery of new projects and verify the status of current crowdfunding goals.


## Available Tools
- **verify_api_connection**: Check connection
- **get_charity_details**: Get org metadata
- **get_project_details**: Get project metadata
- **list_all_projects**: List all projects
- **list_projects_by_country**: List projects by country
- **list_charity_projects**: List projects by org
- **list_projects_by_theme**: g. edu, env, health, disaster).

List projects by theme
- **list_project_themes**: List available themes
- **find_education_initiatives**: Search edu projects
- **find_environment_initiatives**: Search env projects
- **find_health_initiatives**: Search health projects
- **search_nonprofit_projects**: g. theme:edu, country:US).

Search all projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GlobalGiving** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for education projects in Brazil (BR)."

**🤖 AI Agent:**
> Searching projects... I found 5 active education initiatives in Brazil, including 'Digital Literacy for Youth' and 'School Supplies for Rural Areas'. Would you like the goal progress for any of them?

---

**👤 You:**
> "List all active projects for the organization ID '12345'."

**🤖 AI Agent:**
> Retrieving projects... For organization 12345, I found 3 active projects: 'Clean Water for All', 'Solar Power Inititative', and 'Health Clinic Support'.

---

**👤 You:**
> "Find environment projects that need less than $1000 to reach their goal."

**🤖 AI Agent:**
> Filtering projects... I found 2 environmental initiatives near their goals: 'Reforestation in Kenya' (Remaining: $450) and 'Ocean Cleanup Program' (Remaining: $820).


## ❓ FAQ

**Q: How do I get an API Key for GlobalGiving?**
Go to the GlobalGiving API website (globalgiving.org/api/) and request a free API key by filling out their registration form.

**Q: Are all organizations on GlobalGiving vetted?**
Yes, GlobalGiving performs rigorous due diligence on all nonprofit partners to ensure they are high-impact and transparent.

**Q: Can I search for projects using ISO country codes?**
Yes! Use the 'list_projects_by_country' tool and provide a standard 2-letter ISO code (e.g., 'BR' for Brazil or 'US' for the USA).

**Q: What themes are available for filtering?**
Common themes include 'edu' (education), 'env' (environment), 'health', 'disaster' (disaster recovery), and 'women' (women and girls).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/globalgiving](https://vinkius.com/mcp/globalgiving)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GlobalGiving** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `globalgiving` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GlobalGiving** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "globalgiving": {
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
