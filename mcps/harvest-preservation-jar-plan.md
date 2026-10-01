# Harvest Preservation Jar Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/harvest-preservation-jar-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculates required jars, lids, and processing batches for crop preservation.

## Description
This MCP server provides essential tools for agricultural preservation planning. It converts raw harvest weight into precise supply requirements and processing schedules. Use `calculate_jar_requirements` to determine the exact number of jars and lids needed, accounting for headspace loss and safety reserves. You can then use `estimate_batch_schedule` to organize your processing cycles, or `summary_report_generator` to create a consolidated plan for your preservation project.


## Available Tools (4)
- **validate_recipe_efficiency**: Checks if the current recipe yield and jar selection are practical for the harvest size
- **calculate_jar_requirements**: Determines the total number of jars and lids needed for a specific harvest
- **estimate_batch_schedule**: Determines how many processing batches are needed to handle the total volume
- **summary_report_generator**: Provides a human-readable consolidated plan of all supplies and steps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvest Preservation Jar Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 50kg of tomatoes. My recipe yields 0.8kg of sauce per kg of tomato. I am using 500ml jars with 20ml of headspace. I want a 10% reserve. How many jars and lids do I need?"

**🤖 AI Agent:**
> You will need 88 jars and 88 lids.

---

**👤 You:**
> "I need to process 100 jars. My equipment can handle 25 jars per batch. How many batches will I need?"

**🤖 AI Agent:**
> You will need 4 batches.

---

**👤 You:**
> "Generate a summary report for a harvest of 100kg with a yield of 0.5, using 500ml jars (10ml headspace) and a 10% reserve, with a batch capacity of 20 jars."

**🤖 AI Agent:**
> Your preservation plan requires 110 jars and 110 lids. You will process these in 6 batches: 5 batches of 20 jars and 1 final batch of 10 jars.


## ❓ FAQ

**Q: How do I calculate the number of jars I need?**
You can use the `calculate_jar_requirements` tool. Provide the total harvest weight, the recipe yield, the jar volume, and the required headspace loss.

**Q: Can I plan my processing batches?**
Yes, after calculating your jar requirements, use `estimate_batch_schedule` to determine how many processing cycles are needed based on your equipment capacity.

**Q: What is headspace loss?**
Headspace loss is the volume of space left at the top of a jar to allow for expansion during the preservation process. This must be subtracted from the total jar volume to find the effective volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/harvest-preservation-jar-plan](https://vinkius.com/en/ai-agent-connect/harvest-preservation-jar-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvest Preservation Jar Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `harvest-preservation-jar-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvest Preservation Jar Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvest-preservation-jar-plan": {
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
