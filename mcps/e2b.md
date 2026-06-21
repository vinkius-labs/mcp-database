# E2B MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/e2b)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/e2b-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/e2b-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Secure cloud sandboxes for AI code execution — run Python, JavaScript, and shell commands in isolated Firecracker microVMs with ~150ms cold start.

## Description
Connect your AI agent to **E2B** — the leading sandbox platform for AI code execution, trusted by OpenAI, Anthropic, and thousands of AI companies.

### What you can do

- **Create Sandboxes** — Spin up isolated Linux environments in ~150ms. Each sandbox is a Firecracker microVM with its own kernel, filesystem, and network
- **List Sandboxes** — Monitor all active sandbox environments, their templates, and resource usage
- **Kill Sandboxes** — Terminate environments when done to release resources and reduce costs

### How it works

1. Subscribe to this server
2. Enter your E2B API key ($100 free credits to start)
3. Your agent can now create and manage isolated code execution environments

### Who is this for?

- **AI Agent Developers** — give agents a safe place to execute generated code without risking your infrastructure
- **Data Science Teams** — run analysis scripts in isolated environments with guaranteed reproducibility
- **EdTech Platforms** — let students execute code in sandboxed environments with full isolation


## Available Tools
- **create_sandbox**: The sandbox is an isolated Linux VM that starts in ~150ms. Use templates like "base" (default), "python3", or "node" for pre-configured environments. Default timeout is 300 seconds.

Create a new isolated cloud sandbox for running code securely. Each sandbox is a Firecracker microVM with its own filesystem
- **kill_sandbox**: The sandbox and its filesystem contents are permanently deleted.

Terminate a running sandbox by its ID
- **list_sandboxes**: Useful for monitoring active environments and managing resources.

List all currently active sandboxes in your E2B account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **E2B** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Python sandbox so I can run a data analysis script."

**🤖 AI Agent:**
> Sandbox created successfully!

| Sandbox ID | Template | Status | Info |
|---|---|---|---|
| `sbx_abc123` | python3 | running | Timeout: 300s |

Your sandbox is ready. It's an isolated Linux environment with Python 3.11 pre-installed. Use the sandbox ID to execute code.

---

**👤 You:**
> "Show me all my running sandboxes."

**🤖 AI Agent:**
> Found 3 active sandboxes:

| Sandbox ID | Template | Status | Info |
|---|---|---|---|
| `sbx_abc123` | python3 | running | Started: 5min ago |
| `sbx_def456` | node | running | Started: 12min ago |
| `sbx_ghi789` | base | running | Started: 1h ago |

---

**👤 You:**
> "Kill sandbox sbx_ghi789 — I'm done with it."

**🤖 AI Agent:**
> Sandbox terminated successfully!

| Sandbox ID | Status | Info |
|---|---|---|
| `sbx_ghi789` | killed | Sandbox terminated — resources released |


## Installation & Usage

To install and use the **E2B** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/e2b](https://vinkius.com/mcp/e2b)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
