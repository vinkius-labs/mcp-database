# E2B MCP Server

Secure cloud sandboxes for AI code execution — run Python, JavaScript, and shell commands in isolated Firecracker microVMs with ~150ms cold start.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/e2b)

## Overview
**Category:** superpower
**Tools Count:** 3

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


## Installation & Usage

To install and use the **E2B** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/e2b](https://vinkius.com/mcp/e2b)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
