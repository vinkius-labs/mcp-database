# Cardio Zone Prescriber MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cardio-zone-prescriber)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise heart rate zones and training prescriptions using the Karvonen method.

## Description
This MCP server provides specialized physiological calculations to optimize cardiovascular training. By using the Heart Rate Reserve (HRR) methodology, it helps users define their training intensity and volume. You can use `get_hr_zones` to find specific heart rate ranges, `calculate_session_prescription` to determine the ideal duration and intensity for a single workout, `calculate_weekly_schedule` to plan weekly frequency, and `analyze_training_load` to verify if your planned volume matches your physiological needs.


## Available Tools (4)
- **analyze_training_load**: Evaluates if a planned training volume is appropriate for the user's current physiological state
- **calculate_session_prescription**: Determines the ideal duration and intensity for a single training session
- **calculate_weekly_schedule**: Determines how many sessions should be performed per week to meet the user's goal
- **get_hr_zones**: Calculates the specific heart rate ranges for each training zone using the Karvonen method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cardio Zone Prescriber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my heart rate zones if my max HR is 190 and resting HR is 60?"

**🤖 AI Agent:**
> Your heart rate zones are: Zone 1 (127-138 bpm), Zone 2 (138-149 bpm), Zone 3 (149-160 bpm), Zone 4 (160-171 bpm), and Zone 5 (171-190 bpm).

---

**👤 You:**
> "I want to focus on endurance. My max HR is 185 and resting HR is 65. How long should my sessions be?"

**🤖 AI Agent:**
> For your endurance goal, the recommended session duration is 45 minutes at a target intensity within the aerobic capacity zone.

---

**👤 You:**
> "Is a weekly plan of 150 minutes appropriate for fat loss if my max HR is 180 and resting HR is 60?"

**🤖 AI Agent:**
> Yes, your planned 150 minutes per week is optimal for your fat loss goal based on your physiological metrics.


## ❓ FAQ

**Q: How are the heart rate zones calculated?**
The zones are calculated using the Karvonen method, which utilizes your Heart Rate Reserve (the difference between your maximum and resting heart rate) to provide more personalized intensity ranges.

**Q: Can I use this for fat loss training?**
Yes, you can select the 'fat loss' goal to receive prescriptions focused on moderate intensity zones that optimize metabolic efficiency.

**Q: What information do I need to provide?**
To get accurate results, you typically need to provide your maximum heart rate and your resting heart rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cardio-zone-prescriber](https://vinkius.com/en/ai-agent-connect/cardio-zone-prescriber)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cardio Zone Prescriber** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cardio-zone-prescriber` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cardio Zone Prescriber** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cardio-zone-prescriber": {
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
