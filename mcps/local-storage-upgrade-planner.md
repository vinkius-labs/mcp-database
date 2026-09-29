# Local Storage Upgrade Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-storage-upgrade-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate required storage capacity, hardware configurations, and cost efficiency.

## Description
This MCP server provides a suite of tools to plan storage infrastructure upgrades. It calculates total required capacity by accounting for current usage, growth rates, safety buffers, and backup overhead. Users can evaluate hardware configurations, rank them by cost-effectiveness, and perform detailed headroom analysis to ensure long-term system stability.


## Available Tools (4)
- **calculate_storage_needs**: Determines the total raw capacity required to meet all safety and growth requirements
- **evaluate_configurations**: Matches the required capacity against a list of available hardware drives to find valid setups
- **get_headroom_analysis**: Calculates the specific surplus capacity for a chosen hardware setup
- **rank_configurations**: Sorts valid storage setups by their cost-effectiveness and utility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Storage Upgrade Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500GB used, a 10% annual growth rate, want 20% free space, and a 1.5x backup overhead. How much total capacity do I need?"

**🤖 AI Agent:**
> Based on your parameters, the total required capacity is 750GB.

---

**👤 You:**
> "I need 1000GB of storage. I have two options: a 1TB drive for $100 or a 2TB drive for $180. Which is better?"

**🤖 AI Agent:**
> The 1TB drive is the most cost-effective option at $100, as it meets your minimum requirement of 1000GB.

---

**👤 You:**
> "If I buy a 4TB drive but only need 3TB, how much extra space will I have?"

**🤖 AI Agent:**
> You will have 1TB of headroom, which represents a 33.3% excess capacity.


## ❓ FAQ

**Q: How do I calculate my total storage needs?**
Use the `calculate_storage_needs` tool. You will need to provide your current used capacity, expected growth rate, desired free-space ratio, and the backup overhead multiplier.

**Q: Can I compare different hardware drives?**
Yes. After calculating your needs, use `evaluate_configurations` with a list of available drives to find valid setups, then use `rank_configurations` to find the most cost-effective option.

**Q: What is headroom in the context of storage planning?**
Headroom is the surplus capacity available in a hardware configuration after meeting all requirements. You can analyze this specifically using the `get_headroom_analysis` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-storage-upgrade-planner](https://vinkius.com/en/ai-agent-connect/local-storage-upgrade-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Storage Upgrade Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-storage-upgrade-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Storage Upgrade Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-storage-upgrade-planner": {
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
