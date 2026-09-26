# Evacuation Go-Bag Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/evacuation-go-bag-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic resource allocation and preparation planner for emergency evacuation supplies.

## Description
This MCP server provides a suite of tools to manage emergency preparedness. It uses `calculate_bag_assignments` to distribute supplies based on household needs and capacity, `identify_required_documents` to ensure legal and medical readiness, `generate_packing_sequence` to optimize bag stability, and `calculate_refresh_dates` to track item expiration. It helps families prepare optimized packing lists and maintenance schedules for any transport mode.


## Available Tools (4)
- **calculate_bag_assignments**: Determines which specific items should be assigned to which household members or specific bags based on capacity and person-specific needs
- **calculate_refresh_dates**: Determines the next scheduled date to review and replace items in the go-bags
- **generate_packing_sequence**: Provides the optimal order for placing items into the bags to ensure stability and accessibility
- **identify_required_documents**: Generates a list of necessary document copies and digital preparations based on the household profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evacuation Go-Bag Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan my evacuation bag for a family of 4 walking to a shelter with 2 backpacks (10kg limit each)."

**🤖 AI Agent:**
> Your bag assignments are: Person A (Adult): Water, First Aid, ID; Person B (Adult): Food, Water, ID; Person C (Child): Snacks, Toy; Person D (Child): Snacks. Total weight per bag is within the 10kg limit.

---

**👤 You:**
> "What documents do I need to prepare for my family evacuation?"

**🤖 AI Agent:**
> You should print copies of birth certificates, medical insurance cards, and identity IDs, and prepare digital copies of all these documents.

---

**👤 You:**
> "When should I check my medical supplies again?"

**🤖 AI Agent:**
> Your next refresh date is 2025-06-15 due to the expiration of the pediatric antibiotics.


## ❓ FAQ

**Q: How does the tool handle different transport modes?**
The `calculate_bag_assignments` tool adjusts weight and volume constraints based on whether you are walking, using a vehicle, or riding a bicycle.

**Q: Can I track when my supplies expire?**
Yes, you can use `calculate_refresh_dates` to determine when food, water, or medications need to be replaced.

**Q: Does it help with document organization?**
Yes, `identify_required_documents` generates a list of necessary physical and digital copies based on your household profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/evacuation-go-bag-planner](https://vinkius.com/en/ai-agent-connect/evacuation-go-bag-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evacuation Go-Bag Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `evacuation-go-bag-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evacuation Go-Bag Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evacuation-go-bag-planner": {
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
