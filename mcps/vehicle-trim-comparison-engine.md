# Vehicle Trim Comparison Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vehicle-trim-comparison-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automotive](../categories/automotive.md)

Rank and compare vehicle trims using weighted scoring for price, features, and utility.

## Description
This MCP server provides a specialized ranking engine to evaluate competing vehicle trims. By using `rank_vehicle_trims`, users can assign importance weights to specific attributes like price, feature sets, fuel type, warranty, and cargo capacity to generate a stable, weighted ranking. Additionally, you can use `calculate_feature_overlap` to see how well a trim meets your specific requirements, `get_trim_details` for raw specification lookups, and `compare_fuel_efficiency` to evaluate fuel type hierarchies across a group of vehicles.


## Available Tools (4)
- **compare_fuel_efficiency**: 
- **calculate_feature_overlap**: 
- **get_trim_details**: 
- **rank_vehicle_trims**: 0

Ranks supplied vehicle trims based on user-provided weights for different attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vehicle Trim Comparison Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Rank these three trims: Trim A ($30k, heated seats, 15cf cargo), Trim B ($35k, sunroof, 20cf cargo), and Trim C ($25k, basic features, 10cf cargo). Weight price at 0.5 and features at 0.5."

**🤖 AI Agent:**
> The ranked list is: 1. Trim A (Score: 0.75), 2. Trim C (Score: 0.60), 3. Trim B (Score: 0.45). The price delta is $10,000.

---

**👤 You:**
> "Does the 'Luxury Edition' trim include 'heated seats' and 'panoramic sunroof'?"

**🤖 AI Agent:**
> The 'Luxury Edition' trim has a 50% feature overlap, as it includes heated seats but is missing the panoramic sunroof.

---

**👤 You:**
> "Compare the fuel efficiency of an Electric SUV and a Gasoline Sedan."

**🤖 AI Agent:**
> The Electric SUV is the most efficient type in this comparison.


## ❓ FAQ

**Q: How do I rank multiple vehicles at once?**
You can use the `rank_vehicle_trims` tool by providing an array of trim objects and a weights object that defines the importance of each attribute.

**Q: Can I check if a specific trim has the features I need?**
Yes, use the `calculate_feature_overlap` tool to determine the percentage of your required features that are included in a specific trim.

**Q: How are the scores calculated?**
Scores are calculated by normalizing each attribute (0 to 1) and multiplying it by your provided weight. For price, a lower value results in a higher score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vehicle-trim-comparison-engine](https://vinkius.com/en/ai-agent-connect/vehicle-trim-comparison-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vehicle Trim Comparison Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vehicle-trim-comparison-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vehicle Trim Comparison Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vehicle-trim-comparison-engine": {
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
