# Fragrance Layering Compatibility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fragrance-layering-compatibility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Analyze fragrance combinations for harmony, intensity, and optimal application order.

## Description
This MCP server provides expert olfactory analysis for fragrance layering. Use `analyze_layering_set` to evaluate how different scents interact, check family harmony with `get_family_compatibility`, and ensure your blend is appropriate for the setting using `calculate_intensity_profile`. It also provides a step-by-step guide via `suggest_application_sequence` to ensure the correct application order based on scent volatility.


## Available Tools (4)
- **analyze_layering_set**: Evaluates a group of fragrances to determine if they can be layered together effectively
- **calculate_intensity_profile**: Determines if the combined strength of a set of fragrances is appropriate for different environments
- **get_family_compatibility**: Checks if two specific fragrance families are harmonious or conflicting
- **suggest_application_sequence**: Provides a step-by-step guide on how to physically apply the fragrances for the best result


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fragrance Layering Compatibility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I layer a woody scent with a citrus scent?"

**🤖 AI Agent:**
> Yes, woody and citrus families are often harmonious, creating a balanced profile.

---

**👤 You:**
> "Is this combination too strong for an office setting: Woody (8) and Oriental (9)?"

**🤖 AI Agent:**
> No, that combination is overwhelming for an office environment.

---

**👤 You:**
> "What is the best order to apply these three fragrances?"

**🤖 AI Agent:**
> Apply the base-heavy fragrance first, followed by the heart notes, and finish with the top notes.


## ❓ FAQ

**Q: How do I know if my fragrances will clash?**
You can use the `analyze_layering_set` tool to identify specific conflicts between fragrance families in your collection.

**Q: Can I check if a scent is too strong for the office?**
Yes, the `calculate_intensity_profile` tool evaluates if your combination is appropriate for environments like the Office, Evening, or Outdoor settings.

**Q: What is the best way to apply layered scents?**
The `suggest_application_sequence` tool provides a customized step-by-step guide, typically recommending applying heavier base notes before lighter top notes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fragrance-layering-compatibility](https://vinkius.com/en/ai-agent-connect/fragrance-layering-compatibility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fragrance Layering Compatibility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fragrance-layering-compatibility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fragrance Layering Compatibility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fragrance-layering-compatibility": {
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
