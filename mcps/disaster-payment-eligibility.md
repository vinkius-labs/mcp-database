# Disaster Payment Eligibility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/disaster-payment-eligibility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate USDA disaster program eligibility and estimated payments for ARC, PLC, ELAP, and LFP.

## Description
This MCP server provides specialized calculation engines for USDA disaster assistance programs. It allows AI agents to determine eligibility and estimate payments for Agriculture Risk Coverage (ARC), Price Loss Coverage (PLC), Emergency Assistance for Livestock, Honeybees, and Wool Producers (ELAP), and the Livestock Forage Disaster Program (LFP). Using tools like `calculate_arc_plc_eligibility` and `estimate_elap_lfp_loss`, agents can analyze crop data, yield history, and price triggers to provide precise financial insights for producers. The server also includes `get_trigger_probability` to assess historical risk and `generate_program_selection` to recommend the most beneficial program based on current market conditions.


## Available Tools (4)
- **get_trigger_probability**: Analyzes historical yield and price data to estimate the likelihood of a program trigger occurring in the next cycle
- **calculate_arc_plc_eligibility**: Determines if a producer qualifies for ARC or PLC and calculates the estimated payment for a specific crop
- **estimate_elap_lfp_loss**: Calculates potential payments for livestock and forage-related disaster scenarios
- **generate_program_selection**: Provides a recommendation on which program (ARC vs PLC) would likely yield the highest payment based on current market conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Disaster Payment Eligibility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500 base acres of Corn, 450 planted acres, a yield history of 180 bushels, and my actual production was 170. The price trigger is $4.50. My AGI is $150,000 and my payment limit is $50,000. Am I eligible for ARC or PLC?"

**🤖 AI Agent:**
> You are eligible for PLC. Your estimated payment is $12,500.

---

**👤 You:**
> "My livestock forage value is $100,000 and I've experienced a 30% loss due to drought. My AGI is $80,000. How much can I expect from ELAP or LFP?"

**🤖 AI Agent:**
> Your estimated payment for the forage loss is $30,000.

---

**👤 You:**
> "Based on these historical yields [150, 160, 145, 155, 170] and prices [5.0, 4.8, 5.2, 4.5, 4.7], what is the probability of the price falling below $4.60?"

**🤖 AI Agent:**
> The probability of the price trigger occurring is 0.4, with a frequency of occurrence of 2 out of 5 cycles.


## ❓ FAQ

**Q: How does the server determine if I am eligible for ARC or PLC?**
The `calculate_arc_plc_eligibility` tool checks your Adjusted Gross Income (AGI) against statutory limits and verifies that your planted acres do not exceed your USDA base acres.

**Q: Can I estimate losses for livestock or forage?**
Yes, you can use the `estimate_elap_lfp_loss` tool to calculate potential payments for ELAP and LFP programs based on loss severity and total asset value.

**Q: How can I decide between ARC and PLC?**
The `generate_program_selection` tool compares the potential revenue shortfall for ARC against the price shortfall for PLC to recommend the program with the higher expected payment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/disaster-payment-eligibility](https://vinkius.com/ai-agent-connect/disaster-payment-eligibility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Disaster Payment Eligibility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `disaster-payment-eligibility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Disaster Payment Eligibility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "disaster-payment-eligibility": {
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
