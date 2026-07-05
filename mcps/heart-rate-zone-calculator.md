# Heart Rate Zone Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-rate-zone-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate personalized training zones using the Karvonen formula and sport-specific adjustments.

## Description
The Heart Rate Zone Calculator is a precision engine designed to optimize athletic performance through physiological accuracy. By utilizing the Karvonen method, it calculates heart rate ranges based on your Heart Rate Reserve (HRR), ensuring that training intensity is personalized to your specific cardiovascular fitness level. The tool supports multiple disciplines including running, cycling, and swimming, applying necessary sport-specific modifiers to intensity boundaries. Use `get_max_heart_rate` to establish your physiological ceiling, `calculate_training_zones` to define your metabolic targets, and `get_workout_distribution` to plan session durations aligned with goals like Endurance, Threshold, or VO2 Max development.


## Available Tools (3)
- **calculate_training_zones**: Calculates specific heart rate ranges for all five training zones
- **get_workout_distribution**: Provides a recommended time allocation across training zones
- **get_max_heart_rate**: Determines the most accurate maximum heart rate for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Rate Zone Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my max heart rate if I am 30 years old and recently recorded 185 bpm in a test?"

**🤖 AI Agent:**
> Your maximum heart rate is 185 bpm, based on your recent field test result.

---

**👤 You:**
> "Calculate my training zones for cycling with a max HR of 190 and resting HR of 60."

**🤖 AI Agent:**
> For cycling, your zones are: Zone 1: 123-135 bpm, Zone 2: 135-147 bpm, Zone 3: 147-159 bpm, Zone 4: 159-171 bpm, and Zone 5: 171-190 bpm.

---

**👤 You:**
> "How should I distribute a 60 minute workout for a VO2 Max focus?"

**🤖 AI Agent:**
> For a Power/VO2 Max Focus, your 60-minute session should be distributed as: Zone 1: 5 mins, Zone 2: 5 mins, Zone 3: 10 mins, Zone 4: 25 mins, and Zone 5: 15 mins.


## ❓ FAQ

**Q: How does the calculator determine my maximum heart rate?**
The `get_max_heart_rate` tool uses either a field test result if provided, or calculates an estimate by subtracting your age from 220.

**Q: What is the Karvonen method?**
The Karvonen method uses your Heart Rate Reserve (the difference between your max HR and resting HR) to create more personalized training zones than simple percentage-based methods.

**Q: Does the tool account for different sports?**
Yes, `calculate_training_zones` applies specific intensity modifiers for disciplines like cycling and swimming to account for different physiological demands.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heart-rate-zone-calculator](https://vinkius.com/mcp/heart-rate-zone-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heart Rate Zone Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heart-rate-zone-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heart Rate Zone Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heart-rate-zone-calculator": {
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
