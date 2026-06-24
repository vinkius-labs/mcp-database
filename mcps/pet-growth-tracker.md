# Pet Growth Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-growth-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate adult weight and track puppy growth milestones by breed.

## Description
The Pet Growth Tracker MCP server provides essential tools for puppy owners to monitor developmental progress. Using the `estimate_adult_weight` tool, you can predict a puppy's final weight based on their current age and weight. The `get_growth_curve` tool offers a roadmap of expected weight milestones for specific breeds, while `check_growth_status` evaluates if a puppy is underweight, overweight, or within the normal range relative to their breed's biological trajectory.


## Available Tools (3)
- **check_growth_status**: Evaluates whether a puppy's current weight is healthy
- **estimate_adult_weight**: Predicts the final adult weight of a puppy
- **get_growth_curve**: Provides a roadmap of expected weight milestones for a specific breed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Growth Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my 8-week old Golden Retriever, weighing 4kg, likely weigh as an adult?"

**🤖 AI Agent:**
> Based on the current weight and age, your Golden Retriever is estimated to reach an adult weight of approximately 30kg.

---

**👤 You:**
> "Is my 12-week old Chihuahua, weighing 1.5kg, growing correctly?"

**🤖 AI Agent:**
> Your Chihuahua is currently within the normal growth range for its breed and age.

---

**👤 You:**
> "Show me the expected weight milestones for a German Shepherd."

**🤖 AI Agent:**
> The growth curve for a German Shepherd includes milestones such as 4 weeks (approx 3kg), 8 weeks (approx 6kg), and 16 weeks (approx 12kg).


## ❓ FAQ

**Q: How accurate is the adult weight estimation?**
The `estimate_adult_weight` tool uses breed-specific deceleration curves to provide a scientific estimate based on current physiological markers.

**Q: Can I track breeds other than the ones listed?**
The tool currently supports a wide variety of common breeds across small, medium, large, and giant categories. If a breed is not found, the tool will return an error.

**Q: What does 'Normal' status mean in growth tracking?**
A 'Normal' status indicates that the puppy's current weight falls within the healthy variance of the expected trajectory for its specific breed and age.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-growth-tracker](https://vinkius.com/mcp/pet-growth-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Growth Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-growth-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Growth Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-growth-tracker": {
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
