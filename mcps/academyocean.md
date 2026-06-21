# AcademyOcean MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/academyocean)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

LMS for smart corporate training — manage learners, courses, and training progress via AI.

## Description
Connect your **AcademyOcean** account to your AI agent to streamline corporate education and employee onboarding. From inviting new learners to auditing course completion rates, your agent handles learning management through natural conversation.

### What you can do

- **Learner Management** — List all registered learners and easily invite new team members to your academy
- **Course Catalog** — Browse available courses and review training materials available in your LMS
- **Progress Tracking** — Monitor detailed learner progress, including course starts, lesson completions, and quiz results
- **Team Organization** — Manage teams and ensure specific departments are assigned to the right learning paths
- **Automated Reporting** — Quickly retrieve training statistics and completion data directly from chat

### How it works

1. Subscribe to this server
2. Enter your AcademyOcean Client ID and Client Secret
3. Start managing your academy and tracking learner growth through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR & L&D Managers** — automate employee onboarding and monitor compliance training progress
- **Team Leaders** — verify team skill development and course engagement levels on the fly
- **Customer Education Teams** — manage external training portals and track client learning journeys
- **Operations Leads** — streamline user provisioning and training reports


## Available Tools
- **list_learners**: List all academy learners
- **invite_learner**: Invite a new learner
- **list_courses**: List all available courses
- **get_learner_progress**: Get course progress for learners


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AcademyOcean** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the progress of 'John Doe' in the 'Cybersecurity Basics' course."

**🤖 AI Agent:**
> John Doe has completed 75% of the 'Cybersecurity Basics' course. He has finished 6 out of 8 lessons and passed the midterm quiz with a score of 90%.


## ❓ FAQ

**Q: How do I invite a new employee to the academy?**
Use the `invite_learner` tool and provide the employee's email address. Your agent will send the official invitation and create their profile in AcademyOcean.

**Q: How do I track course completions in real-time?**
AcademyOcean supports webhooks that trigger alerts when a learner starts a course, finishes a module, or earns a certificate, keeping external HR systems perfectly synced.

**Q: Can I integrate training data with my CRM?**
Yes, you can easily export course progress and engagement data to systems like Salesforce or HubSpot via API to correlate training with performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/academyocean](https://vinkius.com/mcp/academyocean)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AcademyOcean** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `academyocean` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AcademyOcean** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "academyocean": {
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
