# Accessible Transit Enrollment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-transit-enrollment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Maps transport service rules to actionable application sequences and document checklists.

## Description
This MCP connects AI agents to transport service requirements. It uses `enroll_analyze_readiness` to determine application readiness, `generate_document_checklist` to identify missing documentation, `create_communication_scripts` for provider outreach, and `build_service_use_plan` to create logistical roadmaps based on trip needs.


## Available Tools (4)
- **build_service_use_plan**: Creates a logistical roadmap for using the service based on user needs and service deadlines
- **create_communication_scripts**: Generates tailored templates for interacting with service providers
- **enroll_analyze_readiness**: Determines which services a user can immediately apply for versus those requiring preparatory steps
- **generate_document_checklist**: Provides a precise list of what the user needs to gather to complete an application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Transit Enrollment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Am I ready to apply for the City Shuttle service?"

**🤖 AI Agent:**
> You are not ready to apply for the City Shuttle. You are missing a valid ID and have not completed the prerequisite orientation step.

---

**👤 You:**
> "What documents do I need for the Community Transit program?"

**🤖 AI Agent:**
> To enroll in Community Transit, you need to provide a proof of residence and a signed waiver.

---

**👤 You:**
> "Help me plan my trips for next week using the available shuttle."

**🤖 AI Agent:**
> Based on your trip needs, the shuttle can accommodate your Tuesday and Thursday morning requests, but it does not operate on weekends.


## ❓ FAQ

**Q: How does the tool determine if I am ready to apply?**
The `enroll_analyze_readiness` tool compares your provided documents and completed steps against the published requirements of each service.

**Q: Can this tool decide if I am eligible for a service?**
No. The system only checks if your stated documentation matches the service's requirements. It does not make eligibility determinations.

**Q: What is a service-use plan?**
A service-use plan is a logistical schedule created by `build_service_use_plan` that aligns your trip needs with service availability and deadlines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-transit-enrollment-planner](https://vinkius.com/en/ai-agent-connect/accessible-transit-enrollment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Transit Enrollment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-transit-enrollment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Transit Enrollment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-transit-enrollment-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
