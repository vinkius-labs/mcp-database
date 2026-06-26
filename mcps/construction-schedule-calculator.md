# Construction Schedule Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/construction-schedule-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Estimate construction phase durations and project timelines based on building type and area.

## Description
This MCP server provides precise estimation tools for construction planning. Use `get_phase_durations` to calculate the number of weeks required for each phase, including site work, foundation, and finishes. You can also use `get_schedule_summary` to get a high-level overview of total project duration in weeks and months, or `get_construction_reference` to see supported construction types like Residential, Commercial, and Industrial.


## Available Tools (3)
- **get_construction_reference**: Retrieve metadata for available construction types
- **get_phase_durations**: Calculate estimated duration for each construction phase
- **get_schedule_summary**: Get a high-level summary of the project timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Construction Schedule Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will a 500 square meter residential construction take for each phase?"

**🤖 AI Agent:**
> For a 500 sqm residential project, the estimated durations are: Site Work: 2 weeks, Foundation: 3 weeks, Framing: 4 weeks, MEP Rough-in: 3 weeks, Insulation: 1 week, Drywall: 2 weeks, Finishes: 4 weeks, and Final Site Work: 1 week.

---

**👤 You:**
> "Give me a summary for a 2000 sqm industrial project."

**🤖 AI Agent:**
> The total estimated duration for your 2000 sqm industrial project is 45 weeks, which is approximately 10 months. The project scale is classified as Large.

---

**👤 You:**
> "What are the available construction types?"

**🤖 AI Agent:**
> The supported construction types are Residential (lower complexity), Commercial (medium complexity), and Industrial (high complexity).


## ❓ FAQ

**Q: How do I calculate the duration for specific phases?**
Use the `get_phase_durations` tool by providing your construction type and the total project area.

**Q: What construction types are supported?**
The server supports Residential, Commercial, and Industrial construction types. You can check all details using `get_construction_reference`.

**Q: Can I get a total project timeline summary?**
Yes, use the `get_schedule_summary` tool to retrieve the total estimated weeks and months for your project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/construction-schedule-calculator](https://vinkius.com/mcp/construction-schedule-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Construction Schedule Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `construction-schedule-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Construction Schedule Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "construction-schedule-calculator": {
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
