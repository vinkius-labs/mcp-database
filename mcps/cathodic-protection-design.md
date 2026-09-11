# Cathodic Protection Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cathodic-protection-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Design electrochemical cathodic protection systems for pipelines and structures using NACE standards.

## Description
This MCP server provides specialized engineering tools for designing cathodic protection (CP) systems. It allows engineers to calculate electrical current requirements, design sacrificial anode configurations, size impressed current systems for large-scale infrastructure, and evaluate compliance with NACE safety standards. Use `calculate_current_requirements` to determine load, `design_sacrificial_anode_system` for sacrificial setups, `size_impressed_current_system` for powered systems, and `assess_protection_compliance` to verify electrochemical potential against industry thresholds.


## Available Tools (4)
- **assess_protection_compliance**: Evaluates if the current design meets NACE safety and protection standards
- **calculate_current_requirements**: Determines the total electrical current needed to protect a specific structure
- **design_sacrificial_anode_system**: Calculates the configuration for a system using sacrificial anodes
- **size_impressed_current_system**: Designs a powered (impressed current) system for large-scale infrastructure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cathodic Protection Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the current needed for a 500 square meter structure with a 0.9 coating efficiency and 50 mA/m2 current density."

**🤖 AI Agent:**
> The total required current is 25 mA, with a bare surface area of 50 square meters.

---

**👤 You:**
> "Design a sacrificial anode system for a requirement of 100A in soil with 500 ohm-cm resistivity, using an anode with 2000 capacity, 5 year life, and 0.5 resistance."

**🤖 AI Agent:**
> The system requires 50 anodes with a total mass of 250 kg and a spacing of 10 meters.

---

**👤 You:**
> "Is a measured potential of -800mV compliant if the NACE threshold is -850mV?"

**🤖 AI Agent:**
> No, the system is not compliant because the measured potential does not meet the required -850mV threshold.


## ❓ FAQ

**Q: What standards does this tool follow?**
The tool is designed to align with NACE (National Association of Corrosion Engineers) standards for electrochemical protection.

**Q: Can I design both sacrificial and impressed current systems?**
Yes, you can use `design_sacrificial_anode_system` for sacrificial setups and `size_impressed_current_system` for powered impressed current systems.

**Q: How do I check if my system is safe?**
You can use the `assess_protection_compliance` tool to compare measured electrochemical potential against required NACE thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cathodic-protection-design](https://vinkius.com/en/ai-agent-connect/cathodic-protection-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cathodic Protection Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cathodic-protection-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cathodic Protection Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cathodic-protection-design": {
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
