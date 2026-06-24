# UV Exposure Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uv-exposure-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate maximum safe sun exposure time based on UV index, skin type, and SPF.

## Description
The UV Exposure Estimator provides precise calculations for the maximum duration you can safely remain in the sun. By using tools like `calculate_safe_minutes`, `lookup_skin_characteristics`, and `classify_uv_intensity`, AI agents can determine skin vulnerability based on the Fitzpatrick scale, assess risks from current UV levels, and factor in Sun Protection Factor (SPF) to extend safety windows.


## Available Tools (3)
- **calculate_safe_minutes**: Calculate the maximum safe duration of sun exposure
- **classify_uv_intensity**: Classify the current UV intensity level
- **lookup_skin_characteristics**: Lookup dermatological information for a specific skin type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UV Exposure Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my safe sun exposure time if the UV index is 8 and I have skin type III with SPF 30?"

**🤖 AI Agent:**
> With a UV index of 8, skin type III, and SPF 30, your safe exposure time is approximately 25 minutes.

---

**👤 You:**
> "Tell me about the characteristics of Fitzpatrick skin type I."

**🤖 AI Agent:**
> Skin type I is highly sensitive, has minimal melanin, and faces an extreme risk of sunburn.

---

**👤 You:**
> "The UV index is currently 2. What should I do?"

**🤖 AI Agent:**
> A UV index of 2 is considered Low. The risk is minimal, and standard skin resistance is usually sufficient.


## ❓ FAQ

**Q: How does the tool calculate safe exposure time?**
The `calculate_safe_minutes` tool uses your UV index, Fitzpatrick skin type, and SPF level to estimate how many minutes you can stay in the sun before reaching an erythema threshold.

**Q: What is the Fitzpatrick scale?**
The Fitzpatrick scale (I-VI) classifies skin based on its response to UV radiation, ranging from very fair/sensitive skin to deeply pigmented/resistant skin.

**Q: Can I include SPF in my calculation?**
Yes, providing an `spfLevel` to the `calculate_safe_minutes` tool will increase your calculated safe exposure duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uv-exposure-estimator](https://vinkius.com/mcp/uv-exposure-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UV Exposure Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uv-exposure-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UV Exposure Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uv-exposure-estimator": {
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
