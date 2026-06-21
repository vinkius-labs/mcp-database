# Logstash (Server-side Log Pipeline API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/logstash-server-side-log-pipeline-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Monitor and manage Logstash instances — check node health, inspect pipeline statistics, and troubleshoot hot threads directly from any AI agent.

## Description
Connect your **Logstash** instance to any AI agent to monitor and manage your server-side data processing pipelines through natural conversation.

### What you can do

- **Health Monitoring** — Get instant reports on the health status of your Logstash nodes and pipelines (Green/Yellow/Red).
- **Performance Metrics** — Retrieve detailed JVM, process, and event flow statistics to identify bottlenecks.
- **Node Inspection** — Access configuration details, OS environment, and pipeline settings.
- **Troubleshooting** — Identify performance issues by fetching current hot threads in real-time.
- **Plugin Management** — List all installed plugins and their versions to ensure environment consistency.

### How it works

1. Subscribe to this server
2. Enter your Logstash API URL and credentials (if applicable)
3. Start monitoring your data pipelines from Claude, Cursor, or any MCP-compatible client

No more manual curl commands to port 9600. Your AI acts as a dedicated systems administrator or SRE.

### Who is this for?

- **DevOps Engineers** — instantly check node health and JVM metrics without leaving the terminal or chat interface
- **SRE Teams** — troubleshoot performance bottlenecks by inspecting hot threads during incidents
- **Data Engineers** — verify pipeline settings and plugin versions across different environments


## Available Tools (6)
- **get_health_report**: Get Logstash health report
- **get_hot_threads**: Useful for troubleshooting performance issues.

Get Logstash hot threads
- **get_node_info**: Get Logstash node information
- **get_plugins_info**: Get Logstash plugins information
- **get_root**: Get Logstash root information
- **get_node_stats**: Get Logstash node statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Logstash (Server-side Log Pipeline API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current health status of my Logstash instance?"

**🤖 AI Agent:**
> I've checked the health report. Your Logstash instance is currently 'green'. All pipelines are functioning normally and no issues were detected in the latest report.

---

**👤 You:**
> "Show me the JVM and event statistics for this node."

**🤖 AI Agent:**
> Fetching node statistics... The JVM heap usage is at 45%, and the event pipeline is processing approximately 1,200 events per second with zero failures in the last 5 minutes.

---

**👤 You:**
> "Are there any hot threads causing performance issues right now?"

**🤖 AI Agent:**
> I've analyzed the hot threads. There is one thread related to the 'elasticsearch' output plugin consuming 15% CPU, but overall the process looks stable. No critical bottlenecks detected.


## ❓ FAQ

**Q: How can I check if my Logstash pipelines are running correctly?**
You can use the `get_health_report` tool. It returns a status report (green, yellow, or red) for the Logstash instance and its active pipelines, allowing you to quickly identify any operational issues.

**Q: Can the AI help me find performance bottlenecks in my Logstash node?**
Yes! Use `get_node_stats` to see detailed JVM and event metrics, or `get_hot_threads` to see which parts of the process are consuming the most CPU. This helps pinpoint exactly where the slowdown is occurring.

**Q: Is it possible to list all installed plugins and their versions?**
Absolutely. The `get_plugins_info` tool retrieves a complete list of all currently installed Logstash plugins along with their specific version numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logstash-server-side-log-pipeline-api](https://vinkius.com/mcp/logstash-server-side-log-pipeline-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Logstash (Server-side Log Pipeline API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `logstash-server-side-log-pipeline-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Logstash (Server-side Log Pipeline API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "logstash-server-side-log-pipeline-api": {
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
