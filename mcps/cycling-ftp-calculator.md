# Cycling FTP Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cycling-ftp-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate FTP, power zones, and training metrics like TSS and IF from cycling tests.

## Description
This MCP server provides specialized tools for cyclists to quantify their performance. Use `calculate_ftp_20min` to estimate your Functional Threshold Power (FTP) based on a 20-minute maximal effort, or `calculate_ftp_ramp` if you have completed a ramp test. The server also includes `calculate_session_stress` to determine the Intensity Factor (IF) and Training Stress Score (T/SS) for any training session using your established FTP and normalized power.


## Available Tools (3)
- **calculate_ftp_20min**: Calculate FTP from a 20-minute power test
- **calculate_ftp_ramp**: Calculate FTP from a ramp test
- **calculate_session_stress**: Calculate IF and TSS for a cycling session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycling FTP Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just finished a 20-minute test with an average power of 300W and I weigh 75kg. What is my FTP and what are my power zones?"

**🤖 AI Agent:**
> Your estimated FTP is 285 Watts (285 W/kg). Your power zones are: Zone 1: 0-156.75W, Zone 2: 159.75-213.75W, Zone 3: 217.5-256.5W, Zone 4: 261W-299.25W, Zone 5: 303W-342W, Zone 6: 346.5W-427.5W, and Zone 7: Above 427.5W.

---

**👤 You:**
> "My FTP is 250W. I did a 60-minute ride at 220W normalized power. What was my IF and TSS?"

**🤖 AI Agent:**
> For that session, your Intensity Factor (IF) was 0.88 and your Training Stress Score (TSS) was 88.0.

---

**👤 You:**
> "Calculate my FTP from a ramp test where I reached exhaustion at 280W, weighing 70kg."

**🤖 AI Agent:**
> Your FTP is 280 Watts (4.0 W/kg). Your power zones are: Zone 1: 0-154W, Zone 2: 156.8-196W, Zone 3: 212.8-252W, Zone 4: 255.8-294W, Zone 5: 296.8-336W, Zone 6: 338.8-420W, and Zone 7: Above 420W.


## ❓ FAQ

**Q: How do I calculate my FTP from a 20-minute test?**
Use the `calculate_ftp_20min` tool. Provide your average power during the effort and your body weight in kilograms.

**Q: What is a Training Stress Score (TSS)?**
TSS quantifies the physiological load of a session. You can calculate it using `calculate_session_stress` by providing your FTP, normalized power, and duration.

**Q: Does this tool provide power zones?**
Yes, both the 20-minute and ramp test tools automatically calculate all 7 Andrew Coggan power zones based on your calculated FTP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cycling-ftp-calculator](https://vinkius.com/mcp/cycling-ftp-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycling FTP Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycling-ftp-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycling FTP Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycling-ftp-calculator": {
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
