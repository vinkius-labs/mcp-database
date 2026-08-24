# Telescope Optics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/telescope-optics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate telescope performance, magnification, and viewing comfort.

## Description
This MCP server provides precise astronomical calculations for telescope configurations. Use `calculate_system_performance` to determine focal ratio, magnification, true field of view, exit pupil, Dawes' limit, and limiting magnitude. You can also use `analyze_viewing_comfort` to check if the exit pupil is optimal for an observer's age, or `compare_resolving_power` to see if magnification exceeds the diffraction limit.


## Available Tools (3)
- **analyze_viewing_comfort**: Evaluates how well the telescope's output matches the physiological capabilities of the observer
- **calculate_system_performance**: Provides a complete overview of the telescope's optical characteristics and visual utility
- **compare_resolving_power**: Compares the current setup's magnification against the physical diffraction limits of the hardware


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telescope Optics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the performance for a 100mm aperture telescope with a 1000mm focal length using a 25mm eyepiece for a 30-year-old observer."

**🤖 AI Agent:**
> The telescope has a focal ratio of f/10, magnification of 40x, a true field of view of 1.3 degrees, and an exit pupil of 2.5mm. The Dawes' limit is 1.16 arcseconds and the limiting magnitude is 12.1.

---

**👤 You:**
> "Is a 2mm exit pupil comfortable for a 65-year-old observer?"

**🤖 AI Agent:**
> The viewing comfort is low. For a 65-year-old, a larger exit pupil is recommended to account for reduced pupil dilation.

---

**👤 You:**
> "Check if 300x magnification is useful for a 150mm aperture telescope."

**🤖 AI Agent:**
> The magnification is within the useful range and does not exceed the diffraction limit for a 150mm aperture.


## ❓ FAQ

**Q: How do I calculate my telescope's magnification?**
You can use the `calculate_system_performance` tool by providing the telescope's focal length and the eyepiece's focal length.

**Q: Can this tool help with eye comfort?**
Yes, the `analyze_viewing_comfort` tool evaluates if the exit pupil is well-matched to the observer's physiological pupil dilation based on their age.

**Q: What is the Dawes' limit?**
The Dawes' limit is the theoretical resolving power of the telescope. The `calculate_system_performance` tool provides this value based on your aperture.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/telescope-optics-calculator](https://vinkius.com/ai-agent-connect/telescope-optics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Telescope Optics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `telescope-optics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telescope Optics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telescope-optics-calculator": {
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
