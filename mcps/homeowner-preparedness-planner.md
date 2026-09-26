# Homeowner Preparedness Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/homeowner-preparedness-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [preparedness](../categories/preparedness.md)

Convert property data and local risks into phased preparedness roadmaps and annual safety calendars.

## Description
This MCP server provides a comprehensive management system for household safety. It transforms property features, local risks, and maintenance history into actionable, phased preparedness roadmaps. Users can generate documentation tasks for insurance compliance, receive service reminders to mitigate specific property risks, and create a recurring annual exercise calendar for drills and inspections. Key tools include `get_preparedness_roadmap` for phased planning, `get_documentation_tasks` for record keeping, `get_service_reminders` for maintenance scheduling, and `get_annual_exercise_calendar` for household drills.


## Available Tools (4)
- **get_preparedness_roadmap**: Generates a phased, actionable preparedness roadmap based on property features and risk priorities
- **get_annual_exercise_calendar**: Creates a recurring schedule of drills and inspections to maintain household readiness
- **get_documentation_tasks**: Identifies necessary paperwork and digital records for insurance and emergency readiness
- **get_service_reminders**: Provides a list of upcoming maintenance actions required to mitigate specific property risks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Homeowner Preparedness Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a preparedness roadmap for a home with a wooden roof and high wildfire risk, including two elderly residents."

**🤖 AI Agent:**
> Phase 1: Life Safety - Establish evacuation routes and emergency kits for elderly residents. Phase 2: Property Hardening - Install wildfire-resistant vegetation zones and clear gutters. Phase 3: Long-term Resilience - Evaluate structural reinforcement for high-heat scenarios.

---

**👤 You:**
> "What maintenance reminders do I have based on my last HVAC service 8 months ago?"

**🤖 AI Agent:**
> You should schedule an HVAC filter replacement this month to maintain efficiency and air quality.

---

**👤 You:**
> "What documentation do I need to prepare for insurance purposes?"

**🤖 AI Agent:**
> You should create a digital photo log of your property and a detailed inventory of high-value items to ensure accurate insurance claims.


## ❓ FAQ

**Q: How does the roadmap prioritize tasks?**
The roadmap prioritizes tasks based on your specified `riskPriorities`. Additionally, life-safety tasks for vulnerable household members are always placed in the first phase.

**Q: Can I use this to manage my maintenance schedule?**
Yes, the `get_service_reminders` tool compares your maintenance history against recommended frequencies to provide upcoming maintenance actions.

**Q: What is the purpose of the annual exercise calendar?**
The `get_annual_exercise_calendar` tool creates a 12-month schedule of drills and inspections to ensure your household remains ready for various hazards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/homeowner-preparedness-planner](https://vinkius.com/en/ai-agent-connect/homeowner-preparedness-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Homeowner Preparedness Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `homeowner-preparedness-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Homeowner Preparedness Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "homeowner-preparedness-planner": {
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
