# Mental Health Resource Finder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mental-health-resource-finder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Deterministic matching for Singapore mental health resources.

## Description
This MCP server provides a deterministic matching engine for young adults in Singapore seeking mental health support. It maps symptom severity, budget, and preferred modality to specific local resources, including public institutions like IMH and private digital platforms. Users can use `find_resources` to receive a complete care plan including matched resources, cost ranges, estimated wait times, and subsidy eligibility via CHAS. The tool `validate_user_profile` ensures all inputs meet Singaporean demographic constraints before processing.


## Available Tools (3)
- **calculate_frequency_guideline**: 
- **find_resources**: 
- **validate_user_profile**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mental Health Resource Finder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am feeling mild symptoms and prefer self-help tools. My monthly income is 2500 SGD."

**🤖 AI Agent:**
> Matched Resources: Featuring apps (Wysa, Woebot) free. Cost Range: Free. Wait Time Estimate: 3-7 days. Subsidy Eligible: CHAS eligible. Recommended Frequency: monthly.

---

**👤 You:**
> "I have severe symptoms and need in-person help. My monthly income is 4000 SGD."

**🤖 AI Agent:**
> Matched Resources: IMH subsidized 20-50 SGD, private 200-300 SGD. Cost Range: 20-300 SGD. Wait Time Estimate: 2-4 weeks for public, 3-7 days for private. Subsidy Eligible: Not eligible. Recommended Frequency: weekly.

---

**👤 You:**
> "I have moderate symptoms and want online therapy. My monthly income is 2800 SGD."

**🤖 AI Agent:**
> Matched Resources: Feather 120 SGD, Mind What 150 SGD. Cost Range: 120-150 SGD. Wait Time Estimate: 3-7 days. Subsidy Eligible: CHAS eligible. Recommended Frequency: bi-weekly.


## ❓ FAQ

**Q: How is subsidy eligibility determined?**
Eligibility for CHAS subsidies is determined by the monthly income provided; if the income is strictly less than 3000 SGD, the user is marked as CHAS eligible.

**Q: What kind of resources are provided?**
The engine provides access to a range of resources including digital self-help apps, community services like TOUCH Community Services, and public institutions like IMH.

**Q: How long is the estimated wait time?**
Wait times vary by provider type: public resources typically have a 2-4 week estimate, while private resources usually have a 3-7 day estimate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mental-health-resource-finder](https://vinkius.com/ai-agent-connect/mental-health-resource-finder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mental Health Resource Finder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mental-health-resource-finder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mental Health Resource Finder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mental-health-resource-finder": {
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
