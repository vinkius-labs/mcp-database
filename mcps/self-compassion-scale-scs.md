# Self-Compassion Scale (SCS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/self-compassion-scale-scs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate and interpret Self-Compassion Scale scores.

## Description
This MCP server provides a specialized assessment engine for the Short Form Self-Compassion Scale (SCS-SF). It allows AI agents to calculate global, subscale (Kindness, Humanity, Mindfulness), and profile scores based on 12 item responses. Use `calculate_scs_scores` to process raw inputs, `get_scale_config` to understand the scoring logic, and `get_profile_interpretation` to retrieve qualitative descriptions of self-compassion levels.


## Available Tools (3)
- **calculate_scs_scores**: Calculate Self-Compassion Scale (SCS) scores
- **get_profile_interpretation**: Get interpretation of an assessment profile
- **get_scale_config**: Retrieve the SCS scale configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Self-Compassion Scale (SCS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my self-compassion score for these responses: item1: 4, item2: 2, item3: 5, item4: 1, item5: 4, item6: 3, item7: 5, item8: 2, item9: 4, item10: 3, item11: 5, item12: 2."

**🤖 AI Agent:**
> Based on your responses, your global self-compassion score is 3.25. Your subscale scores are Kindness: 3.67, Humanity: 3.0, and Mindfulness: 3.08. Your profile is Moderate.

---

**👤 You:**
> "What items in the SCS scale need reverse scoring?"

**🤖 AI Agent:**
> The items that require reverse scoring are: 2, 5, 6, 8, and 9.

---

**👤 You:**
> "Explain what a 'High' self-compassion profile means."

**🤖 AI Agent:**
> A High profile represents a state of strong, consistent self-kindness and environmental awareness.


## ❓ FAQ

**Q: What is the SCS-SF?**
The Short Form Self-Compassion Scale (SCS-SF) is a psychometric tool used to measure an individual's capacity for self-kindness, common humanity, and mindfulness.

**Q: How do I calculate scores?**
You can use the `calculate_scs_scores` tool by providing a JSON array of item IDs and their corresponding numerical responses.

**Q: Does the tool handle reverse scoring?**
Yes, the `calculate_scs_scores` tool automatically applies reverse scoring to specific items identified in the scale configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/self-compassion-scale-scs](https://vinkius.com/mcp/self-compassion-scale-scs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Self-Compassion Scale (SCS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `self-compassion-scale-scs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Self-Compassion Scale (SCS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "self-compassion-scale-scs": {
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
