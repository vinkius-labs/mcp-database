# HackEDU (Security Journey) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hackedu-security-journey)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate security training via HackEDU — manage users, track progress, and integrate vulnerability data directly from any AI agent.

## Description
Connect your **HackEDU** (now part of Security Journey) platform to any AI agent and take full control of your secure coding training workflows through natural conversation.

### What you can do

- **User & Team Management** — List all users and teams, retrieve detailed profiles, and check UUIDs for assignments.
- **Progress Tracking** — Monitor individual and team training progress to ensure security compliance across your organization.
- **Content Insights** — Browse the full catalog of available security training modules and lessons.
- **Vulnerability Integration** — Access HackEDU’s vulnerability taxonomy mapped to CWE, CVE, and CAPEC standards.
- **Adaptive Training** — Push issues from bug bounty programs or scanners to trigger personalized training plans for developers.
- **Reporting** — Instantly retrieve summaries of security training health and identifying gaps in developer knowledge.

### How it works

1. Subscribe to this server
2. Enter your HackEDU API Key (from the Admin Dashboard)
3. Start managing your security training from Claude, Cursor, or any MCP-compatible client

No more manual exporting of training reports. Your AI assistant acts as a dedicated Security Program Manager or AppSec Coordinator.

### Who is this for?

- **Security Engineers** — instantly retrieve training statuses and sync vulnerability findings to trigger adaptive lessons.
- **Engineering Managers** — track team progress and identify top security performers or areas needing improvement.
- **AppSec Teams** — automate the integration of bug bounty data into developer training flows.


## Available Tools
- **create_issue**: Create/Push a new vulnerability issue to trigger adaptive training
- **get_team_progress**: Get the training progress for a specific team
- **get_user**: Get detailed information about a specific user
- **get_user_progress**: Get the training progress for a specific user
- **list_adaptive_training_plans**: List adaptive training plans created based on vulnerability findings
- **list_content**: List all available training modules and lessons
- **list_issues**: List vulnerability issues synced from external sources (e.g., Bugcrowd, HackerOne)
- **list_teams**: List all teams configured in HackEDU
- **list_users**: List all users in your HackEDU account
- **list_vulnerabilities**: List HackEDU vulnerability taxonomy (CWE/CVE/CAPEC mapping)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HackEDU (Security Journey)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the training progress for Team Alpha."

**🤖 AI Agent:**
> Retrieving Team Alpha progress... The team currently has an overall completion rate of 78%. 12 out of 15 developers have completed the 'OWASP Top 10' module. Would you like to see the names of the pending users?

---

**👤 You:**
> "List all security lessons related to SQL Injection."

**🤖 AI Agent:**
> Searching catalog... I found 3 relevant modules: 'Basics of SQLi', 'Advanced Blind SQL Injection', and 'Preventing SQLi in Node.js'. Would you like the full description or UUID for any of these?

---

**👤 You:**
> "Create a new security issue for 'BOLA vulnerability found in API' with vulnerability ID 502."

**🤖 AI Agent:**
> Security issue created! I've logged the 'BOLA vulnerability' in HackEDU. This will automatically trigger adaptive training plans for the relevant development team. Should I list the assigned users?


## ❓ FAQ

**Q: How do I find my HackEDU API Key?**
Log in to your HackEDU Admin Dashboard and navigate to the API section. You will be able to generate and copy your unique X-API-Key from there.

**Q: Can I track the training progress of a specific team?**
Yes! Use the `get_team_progress` tool by providing the unique team ID. The agent will return the completion percentage and status for that team.

**Q: What is 'Adaptive Training' in this integration?**
Adaptive Training allows you to push real-world vulnerability findings (via `create_issue`) to HackEDU. The platform then automatically assigns relevant security lessons to developers to help them fix and prevent similar issues.

**Q: Is HackEDU now part of Security Journey?**
Yes, HackEDU was acquired by Security Journey. This integration works with accounts from both brands using the same API infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hackedu-security-journey](https://vinkius.com/mcp/hackedu-security-journey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HackEDU (Security Journey)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hackedu-security-journey` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HackEDU (Security Journey)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hackedu-security-journey": {
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
