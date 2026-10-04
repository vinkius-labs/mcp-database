# Tutoring Rate Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tutoring-rate-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare tutors by hourly price, travel fees, package discounts, and availability.

## Description
This MCP server provides a specialized comparison engine for finding the best tutoring options. It allows AI agents to evaluate candidates by calculating the effective cost of sessions, including travel fees and package discounts. Use `get_tutor_profiles` to find candidates, `calculate_session_costs` to determine total financial impact, `check_tutor_availability` to verify schedule compatibility, and `compare_tutors_ranking` to rank tutors by price or availability.


## Available Tools (4)
- **calculate_session_costs**: Determines the total cost of a single session or a package for a specific tutor
- **check_tutor_availability**: Validates if a tutor can accommodate a specific student's requested time slots
- **get_tutor_profiles**: Retrieves a list of all registered tutors and their basic service details
- **compare_tutors_ranking**: Ranks a subset of tutors based on a specific optimization goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tutoring Rate Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find tutors in London and tell me which one is cheapest for 5 remote sessions."

**🤖 AI Agent:**
> The cheapest option in London for 5 remote sessions is Tutor Sarah, with an effective hourly rate of £35.00.

---

**👤 You:**
> "Check if Tutor ID 't-123' is available on Mondays between 14:00 and 16:00."

**🤖 AI Agent:**
> Yes, Tutor ID 't-123' is available during the requested time slot on Mondays.

---

**👤 You:**
> "Compare the costs for 10 in-person sessions for tutors 't-001' and 't-002'."

**🤖 AI Agent:**
> For 10 in-person sessions, Tutor 't-001' has a total cost of £450.00, while Tutor 't-002' has a total cost of £420.00.


## ❓ FAQ

**Q: How does the tool calculate the total cost?**
The `calculate_session_costs` tool calculates the base rate, adds travel fees if the session is not remote, and applies any applicable package discounts to provide a final effective hourly rate.

**Q: Can I compare tutors based on their schedule?**
Yes, you can use `compare_tutors_ranking` with the 'availability' metric to rank tutors based on how well they match your target hours.

**Q: How do I find tutors in a specific city?**
You can use the `get_tutor_profiles` tool and provide a `locationQuery` to filter the list of available tutors by geographic area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tutoring-rate-comparator](https://vinkius.com/en/ai-agent-connect/tutoring-rate-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tutoring Rate Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tutoring-rate-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tutoring Rate Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tutoring-rate-comparator": {
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
