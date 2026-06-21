# Gem MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gem)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage recruitment CRM pipelines, track candidates, and oversee outreach via AI agents with Gem.

## Description
Connect your **Gem** recruitment CRM to any AI agent to automate your talent sourcing and candidate relationship management through the Model Context Protocol (MCP). Gem is the AI-first recruiting platform that helps modern teams find, engage, and hire top talent. This MCP server enables you to manage your candidate database, organize talent projects, and retrieve detailed interaction histories directly through natural conversation.

### Key Features

- **Candidate Oversight** — List all candidates in your CRM, retrieve detailed profiles, and create new records instantly to maintain a full talent pipeline.
- **Talent Project Management** — Access your sourcing projects and fetch detailed metadata to track how your talent pools are growing.
- **Interaction Logging** — Access historical notes and interaction logs for candidates, or programmatically log new notes from your chat interface.
- **Outreach Insights** — List active outreach sequences and automated messaging campaigns to understand your engagement status.
- **Custom Metadata** — Retrieve the definitions of custom fields configured for your team to maintain consistent data tracking.
- **Workforce Collaboration** — List all team members and recruiters in the account to verify ownership and assignments.
- **Real-time Synchronization** — Keep your recruiting data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gem API Key (found in Team Settings)
3. Start managing your talent pipelines from Claude, Cursor, or any MCP client

### Who is this for?

- **Recruiters & Sourcers** — quickly check candidate profiles or log a quick interview note without manual dashboard navigation.
- **Talent Ops** — automate the retrieval of project metadata or verify custom field mappings via simple AI commands.
- **Hiring Managers** — get a real-time overview of candidate activity and interaction history for your open roles.


## Available Tools
- **verify_api_connection**: Check connection
- **create_crm_candidate**: Add new candidate
- **add_candidate_note**: Log an interaction
- **get_candidate_details**: Get candidate metadata
- **list_crm_custom_fields**: List team fields
- **get_project_details**: Get project metadata
- **list_candidates**: List CRM candidates
- **list_candidate_notes**: List interactions
- **list_talent_projects**: List Gem projects
- **list_outreach_sequences**: List sequences
- **list_recruiting_team**: List Gem users
- **update_crm_candidate**: Modify candidate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gem** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active candidates in my Gem CRM."

**🤖 AI Agent:**
> Retrieving candidates... I found 5 active profiles, including 'John Doe' (Full Stack Engineer) and 'Jane Smith' (Product Manager). Would you like to see the interaction notes for any of them?

---

**👤 You:**
> "Show me the interactions history for candidate '12345'."

**🤖 AI Agent:**
> Fetching notes... For candidate 12345, I found 3 recent interactions. Last update was from Recruiter Sarah: 'Candidate passed the technical screening and is moving to onsite'.

---

**👤 You:**
> "Create a new candidate record for 'Alice Smith' (alice@email.com)."

**🤖 AI Agent:**
> Candidate created! I have successfully added 'Alice Smith' (alice@email.com) to your Gem CRM. The new Candidate ID is 98765.


## ❓ FAQ

**Q: How do I get an API Key for Gem?**
Team Admins can generate API keys in the Team Settings dashboard of the Gem web application.

**Q: Can I search for candidates across all projects?**
Yes, the 'list_candidates' tool retrieves a global list of candidates, which you can then narrow down using IDs or details.

**Q: Is it possible to log interview notes via the agent?**
Yes! Use the 'add_candidate_note' tool and provide the Candidate ID and your text to instantly update their record in the CRM.

**Q: How do I see which sequences a candidate is in?**
The 'get_candidate_details' tool retrieves the full metadata payload, which includes information about outreach and automated messaging state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gem](https://vinkius.com/mcp/gem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gem** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gem` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gem** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gem": {
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
