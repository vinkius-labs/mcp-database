# Makeup Shade Blender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/makeup-shade-blender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cosmetics](../categories/cosmetics.md)

Calculates precise cosmetic pigment blends, undertones, and color accuracy.

## Description
A professional-grade cosmetic formulation engine that connects AI agents to precise pigment mathematics. Use `calculate_blend` to determine the final RGB, HSL, and hex values of a pigment mixture based on opacity and finish weights. You can use `compare_to_target` to measure how closely a blend matches a desired shade using Delta E distance, or `validate_pigment_integrity` to ensure your formulation ratios are mathematically sound. This tool is essential for digital cosmetic prototyping and shade matching.


## Available Tools (4)
- **calculate_blend**: Calculates the final color characteristics of a mixture of pigments
- **compare_to_target**: Measures the accuracy of a blended shade against a desired reference color
- **identify_undertone_profile**: Determines the dominant color character of a specific color profile
- **validate_pigment_integrity**: Ensures a list of pigments is chemically and mathematically compatible for blending


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Makeup Shade Blender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a blend using 60% of a warm pink pigment (hex #FFB6C1, opacity 0.8) and 40% of a white pigment (hex #FFFFFF, opacity 1.0)."

**🤖 AI Agent:**
> The resulting blend is hex #F7D1D7 with a warm undertone and a light saturation profile.

---

**👤 You:**
> "Is this pigment list valid for blending: 50% Red, 50% Blue?"

**🤖 AI Agent:**
> Yes, the pigment list is compatible as the total ratio equals 1.0.

---

**👤 You:**
> "What is the dominant undertone for a color with HSL(0, 50, 50) and a cool label?"

**🤖 AI Agent:**
> The primary undertone is Cool with moderate intensity.


## ❓ FAQ

**Q: How do I ensure my pigment ratios are correct?**
You can use the `validate_pigment_integrity` tool to verify that your pigment ratios sum exactly to 1.0 and that all opacity values are within valid ranges.

**Q: Can I compare a custom blend to a specific target color?**
Yes, use the `compare_to_target` tool by providing the output from a blend calculation and the target color profile to receive a Delta E distance and match percentage.

**Q: How are undertones determined in a mixture?**
The engine determines the resulting undertone by identifying the most heavily weighted undertone from the provided pigment list during the `calculate_blend` process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/makeup-shade-blender](https://vinkius.com/en/ai-agent-connect/makeup-shade-blender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Makeup Shade Blender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `makeup-shade-blender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Makeup Shade Blender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "makeup-shade-blender": {
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
