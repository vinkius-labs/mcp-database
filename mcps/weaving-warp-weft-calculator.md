# Weaving Warp & Weft Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/weaving-warp-weft-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate precise warp and weft yarn requirements for loom weaving.

## Description
This MCP server provides precise calculations for weavers to determine yarn needs and loom configurations. Use `calculate_warp_requirements` to find total warp ends, length per end, and total yardage/weight. Use `calculate_weft_requirements` to determine the filling yarn needed for a specific fabric length and width. You can also use `calculate_loom_setup` to find the correct number of ends per dent for your reed based on your desired sett.


## Available Tools (3)
- **calculate_loom_setup**: Determines how to physically set up the reed and heddles based on the desired density
- **calculate_warp_requirements**: Calculates the total quantity of warp yarn and the physical configuration needed for the loom
- **calculate_weft_requirements**: Calculates the amount of yarn required to complete the filling (weft) portion of the weave


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weaving Warp & Weft Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much warp yarn do I need for a 20 inch wide fabric, 40 inches long, with a sett of 20 epi, 10% width take-up, 7% length take-up, 36 inches of loom waste, and 2 selvedge ends? The yarn is 1000 yards per pound."

**🤖 AI Agent:**
> You will need 412 total ends, with a warp length of 46.48 inches per end, totaling 19,150 yards of warp yarn, which weighs 19.15 pounds.

---

**👤 You:**
> "Calculate the weft yarn needed for a 20 inch wide, 40 inch long fabric with 15 picks per inch, 10% width take-up, and 7% length take-up. The yarn is 1000 yards per pound."

**🤖 AI Agent:**
> You will need 1,317.6 yards of weft yarn, which weighs 1.32 pounds.

---

**👤 You:**
> "I have a 10-dent reed and I want a sett of 20 epi. How many ends should I put in each dent?"

**🤖 AI Agent:**
> You should place 2 ends in each dent.


## ❓ FAQ

**Q: How does this tool handle loom waste?**
The `calculate_warp_requirements` tool includes a specific input for loom waste, which is the fixed length of yarn required for tying onto the loom.

**Q: Can I calculate my reed denting?**
Yes, use the `calculate_loom_setup` tool by providing your desired sett and the number of dents per inch in your reed.

**Q: What is the difference between take-up and shrinkage?**
Take-up is the length lost due to the interlacing of threads, while shrinkage is the contraction of fibers. Both are accounted for in the calculations to ensure you have enough yarn.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/weaving-warp-weft-calculator](https://vinkius.com/ai-agent-connect/weaving-warp-weft-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weaving Warp & Weft Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weaving-warp-weft-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weaving Warp & Weft Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weaving-warp-weft-calculator": {
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
