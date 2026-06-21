# Heart Rate Zones Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-rate-zones-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise physiological training zones using Simple % and Karvonen (HRR) methods.

## Description
This MCP server provides a precision fitness utility for calculating five distinct heart rate training zones. It supports two primary calculation methodologies: the Simple Percentage method, which uses your maximum heart rate as a baseline, and the Karvonen (Heart Rate Reserve) method, which incorporates your resting heart rate for a more personalized intensity range. The server also includes advanced estimation models like Tanaka and Gulati to predict your maximum heart rate based on age and gender. Use `estimate_max_hr` to find your predicted ceiling, then apply `calculate_simple_zones` or `calculate_karvonen_zones` to define your training boundaries.


## Available Tools
- **estimate_max_hr**: Estimate maximum heart rate based on age and gender
- **calculate_karvonen_zones**: Calculate training zones using the Karvonen (HRR) method
- **calculate_simple_zones**: Calculate training zones using simple percentage of MaxHR


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Rate Zones Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a 30-year-old male. What is my estimated max heart rate?"

**🤖 AI Agent:**
> Based on the Tanaka model for a 30-year-old male, your estimated maximum heart rate is 191 BPM.

---

**👤 You:**
> "My max HR is 180 and my resting HR is 60. What are my training zones using the Karvonen method?"

**🤖 AI Agent:**
> Using the Karvonen method, your training zones are: Zone 1 (90-108 BPM), Zone 2 (108-126 BPM), Zone 3 (126-144 BPM), Zone 4 (144-162 BPM), and Zone 5 (162-180 BPM).

---

**👤 You:**
> "Calculate my simple training zones if my max HR is 190."

**🤖 AI Agent:**
> Based on a maximum heart rate of 190 BPM, your simple intensity zones are: Zone 1 (95-114 BPM), Zone 2 (114-133 BPM), Zone 3 (133-152 BPM), Zone 4 (152-171 BPM), and Zone 5 (171-190 BPM).


## ❓ FAQ

**Q: What is the difference between the Simple and Karvonen methods?**
The Simple method uses a fixed percentage of your maximum heart rate. The Karvonen method uses your Heart Rate Reserve (Max HR minus Resting HR), making it more personalized to your current fitness level.

**Q: How accurate are the maximum heart rate predictions?**
The tool uses scientifically validated models like Tanaka and Gulati. While highly accurate for general populations, clinical testing remains the gold standard.

**Q: Can I use this to plan my interval training?**
Yes, by using `calculate_karvonen_zones`, you can identify the exact BPM ranges for Zone 4 (Anaerobic) and Zone 5 (Maximum Effort) to structure your intervals.


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
3. Set Type to "SSE", enter `heart-rate-zones-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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
