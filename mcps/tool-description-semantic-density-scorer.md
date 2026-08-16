# Tool Description Semantic Density Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tool-description-semantic-density-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyzes LLM tool descriptions to evaluate linguistic precision, verb density, and naming consistency.

## Description
This MCP server provides advanced linguistic analysis for LLM tool descriptions. It quantifies 'instructional density' by measuring verb density, evaluates parameter naming uniformity (camelCase vs snake_case), and calculates a composite clarity score. Use `analyze_description_linguistics` to measure action-oriented language, `calculate_naming_uniformity` to ensure schema consistency, and `get_clarity_score` to assess overall semantic quality and return-type explicitness.


## Available Tools (3)
- **calculate_naming_uniformity**: Checks if the parameter naming within the description follows a consistent casing convention
- **get_clarity_score**: Provides a final assessment of how well an LLM will understand the tool based on semantic markers
- **analyze_description_linguistics**: Evaluates the actionable quality of the text by measuring verb density


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Description Semantic Density Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the verb density of this description: 'This tool is used for fetching user data.'"

**🤖 AI Agent:**
> {"verbCount": 1, "totalWordCount": 10, "densityRatio": 0.1}

---

**👤 You:**
> "Check if the parameter 'user_id' follows camelCase."

**🤖 AI Agent:**
> {"matchCount": 0, "mismatchCount": 1, "uniformityScore": 0.0}

---

**👤 You:**
> "What is the clarity score for: 'Retrieve user profile by ID. Returns a JSON object.'"

**🤖 AI Agent:**
> {"finalScore": 0.95, "lengthPenalty": 0, "clarityRating": "High"}


## ❓ FAQ

**Q: What is verb density?**
Verb density is the ratio of imperative/action verbs to the total word count in a description. High density indicates more direct instructions for the LLM.

**Q: How does the clarity score work?**
The clarity score is a composite metric that rewards explicit return-type definitions and penalizes descriptions that are either too brief or too verbose.

**Q: Can I check for snake_case consistency?**
Yes, you can use `calculate_naming_uniformity` to verify if parameter names follow either camelCase or snake_case conventions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tool-description-semantic-density-scorer](https://vinkius.com/ai-agent-connect/tool-description-semantic-density-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Description Semantic Density Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-description-semantic-density-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Description Semantic Density Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-description-semantic-density-scorer": {
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
