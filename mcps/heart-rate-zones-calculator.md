# Heart Rate Zones Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-rate-zones-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate personalized aerobic training zones using the Karvonen formula.

## Description
This MCP server provides specialized physiological tools to determine your optimal heart rate training zones. Using the scientifically recognized Karvonen method, you can calculate your Heart Rate Reserve (HRR) with `calculate_heart_rate_reserve`. The server also allows you to compute specific BPM boundaries for all five intensity levels using `calculate_zone_ranges`, and retrieve standard intensity descriptions via `get_zone_definitions`. Perfect for athletes looking to target specific metabolic responses like fat oxidation or anaerobic threshold improvement.


## Available Tools (3)
- **get_zone_definitions**: Retrieve standard intensity descriptions for heart rate zones
- **calculate_heart_rate_reserve**: Calculate the Heart Rate Reserve (HRR)
- **calculate_zone_ranges**: Calculate the BPM boundaries for all five training zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Rate Zones Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my heart rate zones. I am 30 years old and my resting heart rate is 60 BPM."

**🤖 AI Agent:**
> Based on your age of 30 and RHR of 60, your training zones are: Zone 1 (120-132 BPM), Zone 2 (132-144 BPM), Zone 3 (144-156 BPM), Zone 4 (156-168 BPM), and Zone 5 (168-180 BPM).

---

**👤 You:**
> "What is my Heart Rate Reserve?"

**🤖 AI Agent:**
> Please provide your age and resting heart rate so I can use `calculate_heart_rate_reserve` to find your value.

---

**👤 You:**
> "Show me the definitions for all heart rate zones."

**🤖 AI Agent:**
> Using `get_zone_definitions`, I can confirm that Zone 1 is very light (50-60%), Zone 2 is light (60-70%), Zone 3 is moderate (70-80%), Zone 4 is hard (80-90%), and Zone 5 is maximum intensity (90-100%) of your HRR.


## ❓ FAQ

**Q: What is the Karvonen formula?**
The Karvonen formula calculates Target Heart Rate (THR) by using your Heart Rate Reserve (HRR), which accounts for both your maximum heart rate and resting heart rate to provide a more personalized training intensity.

**Q: How do I use the zone ranges tool?**
To find your training boundaries, use `calculate_zone_ranges` by providing your current age and resting heart rate in BPM.

**Q: Can I calculate my Heart Rate Reserve separately?**
Yes, you can use the `calculate_heart_rate_reserve` tool to find exactly how many beats per minute are available for your training intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heart-rate-zones-calculator](https://vinkius.com/mcp/heart-rate-zones-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heart Rate Zones Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heart-rate-zones-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heart Rate Zones Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heart-rate-zones-calculator": {
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
