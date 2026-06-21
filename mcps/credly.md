# Credly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/credly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Equip your AI agent to manage digital badges, monitor issuance, and track recipient skills via the Credly API.

## Description
Integrate **Credly**, the world's largest digital credential network, directly into your AI workflow. Manage your organization's badge templates, audit issued credentials, and track member skills using natural language.

### What you can do

- **Badge Management** — List all issued badges and explore your organization's badge templates.
- **Issuance Auditing** — Monitor which recipients have received badges and track authorized issuers.
- **Skill Tracking** — Explore the full inventory of skills mapped to your digital credentials.
- **Organization Insights** — Retrieve metadata and member lists for your connected organizations.

### How it works

1. Connect the Credly integration to your AI assistant.
2. Authorize using your Credly API Key (found in your account settings).
3. Orchestrate your digital credentialing strategy through intuitive conversation.

### Who is this for?

- **HR & L&D Managers** — Quickly audit employee certifications and verified skills.
- **Certification Bodies** — Manage badge templates and monitor issuance status on the go.
- **Program Coordinators** — Track recipient engagement and verify issuer authorizations via chat.


## Available Tools (10)
- **get_badge_details**: Get detailed information for a specific issued badge
- **get_organization_info**: Get metadata for a specific organization
- **get_template_details**: Get full design and criteria for a badge template
- **list_issued_badges**: List all badges issued by your organization
- **list_authorized_issuers**: List people authorized to issue badges
- **list_org_members**: List all members of your organization on Credly
- **list_connected_organizations**: List organizations connected to your account
- **list_badge_recipients**: List people who have received badges
- **list_badge_skills**: List all skills mapped to badges in the system
- **list_badge_templates**: List all badge templates available for issuance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Credly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all badges issued by my organization in the last month."

**🤖 AI Agent:**
> I've found 25 badges issued in the last 30 days. Most are for the 'Cloud Architecture' and 'Agile Leadership' templates. Would you like to see the names of the recipients?

---

**👤 You:**
> "Show me the details for badge ID 'b8s9df7'."

**🤖 AI Agent:**
> Badge 'b8s9df7' was issued to John Doe for completing 'Python for Data Science'. It is currently 'Accepted'. The associated skills include 'Data Analysis' and 'Python'. Should I list the criteria for this badge?

---

**👤 You:**
> "What skills are associated with the 'Senior DevOps Engineer' badge template?"

**🤖 AI Agent:**
> The 'Senior DevOps Engineer' template is mapped to several skills: 'CI/CD Pipelines', 'Kubernetes Orchestration', 'Infrastructure as Code', and 'Cloud Security'. Would you like to see which employees have already earned this badge?


## ❓ FAQ

**Q: How do I get a Credly API Key?**
Log in to your Credly account and navigate to the organization settings to generate or retrieve your API Key. Ensure you have administrative privileges.

**Q: Can the agent issue badges to new recipients?**
This integration currently provides tools for listing and auditing badges and templates. Issuing new badges should be handled through the Credly dashboard or specific automated workflows.

**Q: What badge details can I retrieve?**
You can retrieve full badge profiles including recipient details, template criteria, associated skills, and current status (e.g., pending, accepted).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/credly](https://vinkius.com/mcp/credly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Credly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `credly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Credly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "credly": {
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
