# Endurance Training Zones MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/endurance-training-zones)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate heart rate training zones, session intensity, and recovery needs for surfers.

## Description
This MCP server provides specialized physiological analysis for surfers to optimize their training. By using heart rate reserve methodology, it calculates specific training zones tailored to both paddle-based water sessions and land-based conditioning. Users can use `get_training_zones` to define their intensity ranges, `analyze_session_distribution` to plan workout effort, and `calculate_recovery_needs` to prevent overtraining based on session intensity and modality.


## Available Tools (4)
- **analyze_session_distribution**: Determines how a planned workout session will distribute effort across different physiological zones
- **calculate_recovery_needs**: Predicts the necessary downtime required after a training session to prevent overtraining
- **get_training_zones**: Calculates specific heart rate ranges for different training intensities
- **validate_physiological_bounds**: Ensures that a user's provided biometric data is within realistic human limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Endurance Training Zones** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my training zones if my max HR is 190, resting HR is 60, I am an Intermediate athlete, and I am planning a paddle session?"

**🤖 AI Agent:**
> Your training zones for a paddle session are: Zone 1 (135-145 bpm), Zone 2 (145-158 bpm), Zone 3 (158-171 bpm), Zone 4 (171-182 bpm), and Zone 5 (182-190 bpm).

---

**👤 You:**
> "I just finished a high-intensity paddle session. My max HR is 190, resting HR is 60, I am Intermediate, and I hit Zone 4. How long should I recover?"

**🤖 AI Agent:**
> Based on your Zone 4 paddle session, it is recommended that you take 48 hours of recovery, focusing on light movement or complete rest.

---

**👤 You:**
> "How much time will I spend in Zone 2 if I do a 45-minute land training session with a max HR of 185, resting HR of 65, and Intermediate fitness?"

**🤖 AI Agent:**
> In a 45-minute land session, you will spend approximately 28 minutes in Zone 2.


## ❓ FAQ

**Q: How does paddle training differ from land training in these calculations?**
The tool accounts for the higher metabolic cost of paddling in water compared to land-based movement, adjusting the target heart rate ranges accordingly.

**Q: Can I use this to plan my weekly training load?**
Yes, by using `analyze_session_distribution`, you can see how much time you will spend in different intensity zones to ensure a balanced training load.

**Q: What information do I need to provide?**
You will need your maximum heart rate, resting heart rate, and your current fitness level (Beginner, Intermediate, or Advanced).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/endurance-training-zones](https://vinkius.com/en/ai-agent-connect/endurance-training-zones)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Endurance Training Zones** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `endurance-training-zones` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Endurance Training Zones** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "endurance-training-zones": {
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
