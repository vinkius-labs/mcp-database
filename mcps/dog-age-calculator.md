# Dog Age Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dog-age-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Accurate canine aging estimation using scientific veterinary formulas.

## Description
This MCP server provides precise canine aging estimations by moving beyond the 'seven-year rule'. It uses size-weighted logarithmic models to account for how a dog's physical weight affects its biological maturation. Use `calculate_human_age` to find the human equivalent age, `get_life_stage_details` to understand biological phases like puppy or senior stages, and `compare_size_aging_rates` to see how weight categories influence aging speed.


## Available Tools (3)
- **calculate_human_age**: Calculate the equivalent human age of a dog based on its chronological age and weight
- **compare_size_aging_rates**: Compare how a dog's size affects its aging speed
- **get_life_stage_details**: Get detailed information about a dog's current biological life stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dog Age Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How old is my 3-year-old dog that weighs 45 lbs in human years?"

**🤖 AI Agent:**
> Your dog is approximately 29 years old in human years and is currently in the adult life stage.

---

**👤 You:**
> "What is the life stage of a 1-year-old puppy weighing 10 lbs?"

**🤖 AI Agent:**
> A 1-year-old dog weighing 10 lbs is in the puppy stage, characterized by rapid physical growth.

---

**👤 You:**
> "How does being a giant breed affect aging?"

**🤖 AI Agent:**
> Giant breeds experience a secondary acceleration in biological aging once they pass their fifth chronological year.


## ❓ FAQ

**Q: How is the age calculated?**
The calculation uses a logarithmic formula that accounts for rapid maturation in the first two years and adjusts the aging rate based on the dog's weight category.

**Q: Does size really matter for aging?**
Yes, larger breeds typically undergo biological aging more rapidly than smaller breeds, which is reflected in the `compare_size_aging_rates` tool.

**Q: What life stages are covered?**
The tool identifies four stages: Puppy, Adolescent, Adult, and Senior.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dog-age-calculator](https://vinkius.com/ai-agent-connect/dog-age-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dog Age Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dog-age-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dog Age Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dog-age-calculator": {
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
