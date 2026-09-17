# Pyramid Set Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pyramid-set-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates weight, repetitions, and training metrics for pyramid training progressions.

## Description
This MCP server provides specialized tools for resistance training design using pyramid methodologies. Use `generate_pyramid_scheme` to create complete weight and repetition sequences, or `validate_progression_safety` to ensure your weight jumps are physiologically sound. It also allows for comparing workloads between different training structures using `compare_training_volumes`.


## Available Tools (4)
- **compare_training_volumes**: Compares two pyramid schemes
- **generate_pyramid_scheme**: 
- **get_pyramid_type_constraints**: Gets constraints for a pyramid type
- **validate_progression_safety**: Checks if weight progression is safe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pyramid Set Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an ascending pyramid scheme starting at 50kg, peaking at 100kg, with 5 sets."

**🤖 AI Agent:**
> Here is your ascending pyramid: Set 1: 50kg x 10 reps, Set 2: 62.5kg x 8 reps, Set 3: 75kg x 6 reps, Set 4: 87.5kg x 4 reps, Set 5: 100kg x 2 reps. Total volume: 2250kg.

---

**👤 You:**
> "Is a progression from 40kg to 120kg over 3 sets safe?"

**🤖 AI Agent:**
> No, that progression is considered unsafe due to the extreme weight jump between sets relative to the total number of sets.

---

**👤 You:**
> "What are the constraints for a descending pyramid?"

**🤖 AI Agent:**
> In a descending pyramid, the weight decreases with each subsequent set while the number of repetitions increases.


## ❓ FAQ

**Q: How do I create a new training plan?**
You can use the `generate_pyramid_scheme` tool by providing the starting weight, peak weight, and total number of sets you wish to perform.

**Q: Can I check if my training progression is too intense?**
Yes, the `validate_progression_safety` tool evaluates if your weight jumps are logical and provides intensity warnings if they are too extreme.

**Q: How is total volume calculated?**
Total volume is calculated as the sum of the weight used multiplied by the repetitions performed for every set in the sequence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pyramid-set-generator](https://vinkius.com/en/ai-agent-connect/pyramid-set-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pyramid Set Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pyramid-set-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pyramid Set Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pyramid-set-generator": {
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
