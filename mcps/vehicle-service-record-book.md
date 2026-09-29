# Vehicle Service Record Book MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vehicle-service-record-book)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automotive](../categories/automotive.md)

Manage vehicle maintenance logs, track spending, and identify missing service intervals.

## Description
This MCP server provides a complete management system for vehicle maintenance. It allows AI agents to retrieve a full chronological history of service events using `get_service_history`, aggregate maintenance costs by category with `get_spending_by_category`, and identify overlooked maintenance tasks via `find_missing_intervals`. You can also log new maintenance events using `add_service_record` to keep the vehicle's digital logbook up to date.


## Available Tools (4)
- **get_service_history**: Provides a complete, ordered timeline of all maintenance performed on the vehicle
- **add_service_record**: Records a new maintenance event into the vehicle's history
- **find_missing_intervals**: Identifies scheduled maintenance tasks that have been overlooked based on mileage progression
- **get_spending_by_category**: Answers how much money has been spent on specific types of maintenance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vehicle Service Record Book** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the full service history for vehicle ID V123."

**🤖 AI Agent:**
> The service history for vehicle V123 includes: Oil Change on 2023-05-10 (15,000 miles), Brake Inspection on 2023-01-15 (10,000 miles), and Tire Rotation on 2022-11-01 (5,000 miles). Total spent: $450.

---

**👤 You:**
> "How much have I spent on 'Brakes' for my vehicle?"

**🤖 AI Agent:**
> You have spent a total of $320 on Brakes.

---

**👤 You:**
> "Add a new oil change record for vehicle V123: done on 2024-02-01, 25000 miles, by QuickFix Garage, cost $60, with warranty."

**🤖 AI Agent:**
> The service record has been successfully added. ID: REC-998, Date: 2024-02-01, Mileage: 25000, Provider: QuickFix Garage, Task: Oil Change, Cost: $60, Warranty: Yes.


## ❓ FAQ

**Q: How can I see all past repairs for my car?**
You can use the `get_service_history` tool to retrieve a complete, descending chronological list of all recorded maintenance events.

**Q: Can I track how much I spend on oil changes?**
Yes, the `get_spending_by_category` tool aggregates total costs based on the service category provided in each record.

**Q: How does the system know if I missed a service?**
By using `find_missing_intervals` with a defined maintenance schedule, the system compares the current mileage against the last recorded service to identify gaps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vehicle-service-record-book](https://vinkius.com/en/ai-agent-connect/vehicle-service-record-book)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vehicle Service Record Book** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vehicle-service-record-book` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vehicle Service Record Book** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vehicle-service-record-book": {
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
