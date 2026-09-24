# Pet Vaccine Date Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-vaccine-date-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate future vaccination dates and booster schedules for veterinary management.

## Description
This MCP server provides veterinary professionals with precise tools to manage immunization schedules. Use `get_next_vaccination_date` to find the next due date, `calculate_booster_series` to generate full multi-dose schedules, and `check_vaccine_validity` to verify if a pet's current status is still valid. It also includes `get_vaccine_type_defaults` to retrieve standard intervals for core and non-core vaccine categories.


## Available Tools (4)
- **calculate_booster_series**: Generates a full sequence of future vaccination dates for a multi-dose series
- **check_vaccine_validity**: Determines if a pet's current vaccination status is valid based on the time elapsed since the last dose
- **get_next_vaccination_date**: Calculates the specific date for the next required vaccine dose based on a prior administration
- **get_vaccine_type_defaults**: Retrieves the standard immunization intervals for common vaccine categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Vaccine Date Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is the next dose due if the last vaccine was on 2023-05-10 and the interval is 12 months?"

**🤖 AI Agent:**
> The next vaccination date is 2024-05-10.

---

**👤 You:**
> "Generate a 3-dose series starting on 2024-01-01 with 6 month intervals."

**🤖 AI Agent:**
> Dose 1: 2024-01-01, Dose 2: 2024-07-01, Dose 3: 2025-01-01.

---

**👤 You:**
> "Is a vaccine administered on 2023-01-01 still valid if the required interval is 12 months and today is 2023-06-01?"

**🤖 AI Agent:**
> Yes, the vaccine is still valid with 6 months remaining.


## ❓ FAQ

**Q: How do I calculate a full booster schedule?**
You can use the `calculate_booster_series` tool by providing the initial dose date, the interval in months, and the total number of doses required.

**Q: Can I check if a vaccine has expired?**
Yes, the `check_vaccine_validity` tool allows you to determine if a vaccine is still valid based on the last administration date and the required interval.

**Q: What vaccine categories are supported?**
The tool supports standard categories such as core and non-core vaccines via the `get_vaccine_type_defaults` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-vaccine-date-scheduler](https://vinkius.com/en/ai-agent-connect/pet-vaccine-date-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Vaccine Date Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-vaccine-date-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Vaccine Date Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-vaccine-date-scheduler": {
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
