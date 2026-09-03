# Concrete Development Length Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-development-length-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates required rebar embedment length based on ACI standards.

## Description
This MCP server provides structural engineering tools to calculate the required embedment length of reinforcing steel in concrete. It uses ACI standards to determine development length, accounting for factors like bar diameter, concrete strength, steel yield strength, top bar positions, and epoxy coatings. Use `query_development_length` to find the base embedment, `query_splice_requirement` for overlap lengths, and `query_confinement_effect` to assess how concrete cover influences bond strength. A complete overview of all parameters can be retrieved using `query_rebar_summary`.


## Available Tools (4)
- **query_confinement_effect**: Evaluates how the concrete cover and surrounding reinforcement affect the development length
- **query_development_length**: Calculates the fundamental development length and the individual modification factors
- **query_rebar_summary**: Provides a summary of all calculated parameters for a specific bar configuration
- **query_splice_requirement**: Determines the necessary overlap length for joining two reinforcing bars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Development Length Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the development length for a 20mm rebar in 30MPa concrete with 400MPa steel, considering it is a top bar."

**🤖 AI Agent:**
> The required development length for the 20mm rebar is 850 mm, including the top bar modification factor.

---

**👤 You:**
> "What is the required splice length for a 16mm bar with a development length of 600mm using a lap splice?"

**🤖 AI Agent:**
> The required lap splice length for the 16mm bar is 720 mm.

---

**👤 You:**
> "Check if a 25mm bar with 40mm concrete cover has sufficient cover to prevent splitting."

**🤖 AI Agent:**
> The concrete cover is sufficient for the 25mm bar diameter.


## ❓ FAQ

**Q: What standards does this tool follow?**
The calculations are based on ACI (American Concrete Institute) standards for development length.

**Q: How do I calculate the overlap for two bars?**
You can use the `query_splice_requirement` tool, providing the bar diameter and the previously calculated development length.

**Q: Does it account for epoxy-coated rebar?**
Yes, the `query_development_length` tool includes a specific factor for epoxy coatings to account for reduced bond strength.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-development-length-calculator](https://vinkius.com/ai-agent-connect/concrete-development-length-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Development Length Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-development-length-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Development Length Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-development-length-calculator": {
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
