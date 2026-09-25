# Accessible Employment Visit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-employment-visit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms employment visit details into inclusive, actionable visit protocols and communication templates.

## Description
This MCP server acts as a specialized planning engine for disability-inclusive employment visits. It processes schedules, building access data, and accommodation needs to generate structured visit plans, arrival protocols, and privacy-compliant communication messages. By using tools like `generate_visit_plan`, `validate_disclosure_compliance`, `calculate_arrival_logistics`, and `map_participation_roles`, users can ensure their accessibility requirements are met while maintaining strict control over personal information disclosure.


## Available Tools (4)
- **calculate_arrival_logistics**: Determine the sequence of physical actions required for arrival
- **validate_disclosure_compliance**: Verify that planned messages do not violate privacy boundaries
- **generate_visit_plan**: Generate a comprehensive, structured visit plan based on user inputs
- **map_participation_roles**: Assign engagement levels to participants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Employment Visit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have an interview at 10 AM at the downtown office. The building has a ramp at the North entrance. I need a quiet space for the interview. Here are my contact details and the employer's info."

**🤖 AI Agent:**
> Your visit plan is ready. You should use the North entrance for ramp access. I have prepared a request for a quiet interview space and a confirmation plan for your arrival at 10 AM.

---

**👤 You:**
> "Check if this message to the recruiter is okay: 'I require a screen reader for the technical test.'"

**🤖 AI Agent:**
> The message is compliant with your privacy boundaries and is ready to be sent to the employer.

---

**👤 You:**
> "Help me plan my arrival for the site tour tomorrow. I am taking the bus and the building has limited elevator access."

**🤖 AI Agent:**
> Based on your bus arrival and the building constraints, you should proceed to the main lobby and contact the receptionist via text to confirm elevator availability.


## ❓ FAQ

**Q: How does the server handle my private medical information?**
The server uses `validate_disclosure_compliance` to ensure that no sensitive information is included in messages sent to employers, adhering strictly to your defined privacy boundaries.

**Q: Can I generate specific arrival instructions?**
Yes, the `calculate_arrival_logistics` tool determines the exact sequence of physical actions needed to navigate a site based on your transport and building access details.

**Q: What kind of visit plans can be created?**
The `generate_visit_plan` tool creates comprehensive plans including confirmation steps, request messages for employers, arrival actions, and post-visit follow-ups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-employment-visit-planner](https://vinkius.com/en/ai-agent-connect/accessible-employment-visit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Employment Visit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-employment-visit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Employment Visit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-employment-visit-planner": {
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
