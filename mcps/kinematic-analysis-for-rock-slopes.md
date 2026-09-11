# Kinematic Analysis for Rock Slopes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/kinematic-analysis-for-rock-slopes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Perform kinematic analysis for rock slopes to identify planar, wedge, and toppling failure modes.

## Description
This MCP server provides specialized tools for rock mechanics and slope stability analysis. It allows AI agents to evaluate the risk of different failure modes using stereonet principles. Use `analyze_planar_failure` to check for sliding along a single plane, `analyze_wedge_failure` to evaluate the intersection of two discontinuities, and `analyze_toppling_failure` to assess rotational instability. Finally, use `get_slope_recommendations` to receive engineering mitigation strategies based on the identified risks.


## Available Tools (4)
- **analyze_planar_failure**: Determines if a single discontinuity is prone to sliding along its plane
- **get_slope_recommendations**: Provides engineering guidance based on the results of previous kinematic analyses
- **analyze_toppling_failure**: Evaluates the risk of blocks rotating out of the slope due to steep, near-vertical discontinuities
- **analyze_wedge_failure**: Identifies potential instability caused by the intersection of two discontinuity planes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kinematic Analysis for Rock Slopes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a slope with a 45 degree dip and 180 degree direction is prone to planar failure with a joint dipping at 30 degrees in the 180 direction and a 25 degree friction angle."

**🤖 AI Agent:**
> The analysis shows that the slope is prone to planar failure because the joint dips in the same direction as the slope, the joint dip is less than the slope dip, and it is greater than the friction angle.

---

**👤 You:**
> "Analyze a wedge failure for a slope dipping 50 degrees at 90 degrees, with two joints: one at 30 degrees/45 degrees and another at 35 degrees/135 degrees, with a 20 degree friction angle."

**🤖 AI Agent:**
> The wedge failure analysis indicates that the intersection line daylights in the slope and its plunge exceeds the friction angle, making it prone to instability.

---

**👤 You:**
> "What are the recommendations for a slope facing planar and wedge failures with a 30 degree friction angle?"

**🤖 AI Agent:**
> For the identified planar and wedge failures, the suggested mitigation is to use bolting or anchoring to stabilize the rock mass.


## ❓ FAQ

**Q: What failure modes can be analyzed?**
The server can analyze planar, wedge, and toppling failure modes using `analyze_planar_failure`, `analyze_wedge_failure`, and `analyze_toppling_failure`.

**Q: How do I get mitigation advice?**
After identifying failure modes, pass them to the `get_slope_recommendations` tool to receive specific engineering guidance.

**Q: What inputs are required for analysis?**
Tools require slope dip, slope dip direction, discontinuity dip/direction, and the friction angle of the rock.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/kinematic-analysis-for-rock-slopes](https://vinkius.com/en/ai-agent-connect/kinematic-analysis-for-rock-slopes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kinematic Analysis for Rock Slopes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kinematic-analysis-for-rock-slopes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kinematic Analysis for Rock Slopes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kinematic-analysis-for-rock-slopes": {
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
