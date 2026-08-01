# Prompt System Override Resistance Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prompt-system-override-resistance-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Quantify the structural integrity and resistance of LLM system prompts against manipulation.

## Description
The Prompt System Override Resistance Scorer is a specialized security utility designed to audit the robustness of LLM system prompts. By analyzing command density, it identifies linguistic 'anchors' like `MUST`, `NEVER`, and `ONLY` against 'leaks' such as `maybe` or `sometimes`. Using tools like `calculate_resistance_ratio`, you can derive a quantitative resistance ratio and convert it into a standardized strictness boundary score. This allows developers to identify 'weak zones' via `locate_vulnerable_segments` where low directive density might allow for instruction drift or prompt injection.


## Available Tools (3)
- **calculate_resistance_ratio**: Calculates the ratio of directive keywords to permissive keywords in a text
- **determine_boundary_score**: Converts a resistance ratio into a standardized security metric
- **locate_vulnerable_segments**: Identifies portions of a prompt that lack sufficient command density


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prompt System Override Resistance Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this prompt: 'You MUST always follow instructions. You may sometimes ignore them if you feel like it.'"

**🤖 AI Agent:**
> The resistance ratio is low because the directive 'MUST' is diluted by the permissive 'may' and 'sometimes'. The `calculate_resistance_ratio` would show a high presence of leaks.

---

**👤 You:**
> "What is the risk level for a prompt with a resistance ratio of 0.2?"

**🤖 AI Agent:**
> A resistance ratio of 0.2 would likely result in a 'Critical' risk level when processed by `determine_boundary_score`, as it falls below the required security threshold.

---

**👤 You:**
> "Check if there are any weak zones in this prompt text."

**🤖 AI Agent:**
> The `locate_vulnerable_segments` tool has identified one segment where the directive density is significantly lower than the rest of the document, suggesting a potential vulnerability.


## ❓ FAQ

**Q: How does the resistance ratio work?**
The `calculate_resistance_ratio` tool counts exact occurrences of directive keywords (MUST, NEVER, ONLY, ALWAYS) and divides them by the count of permissive keywords (maybe, usually, sometimes).

**Q: What is a 'vulnerable segment'?**
A vulnerable segment is a portion of text identified by `locate_vulnerable_segments` where the concentration of directive keywords is significantly lower than the overall prompt average, indicating a potential area for instruction override.

**Q: Can I use this to prevent prompt injection?**
Yes, by using `determine_boundary_score`, you can quantify the risk level of your prompt and identify if it falls into a 'Critical' or 'Vulnerable' tier based on its resistance to manipulation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prompt-system-override-resistance-scorer](https://vinkius.com/mcp/prompt-system-override-resistance-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prompt System Override Resistance Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prompt-system-override-resistance-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prompt System Override Resistance Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prompt-system-override-resistance-scorer": {
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
