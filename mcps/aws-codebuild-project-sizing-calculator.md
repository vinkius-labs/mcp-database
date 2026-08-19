# AWS CodeBuild Project Sizing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-codebuild-project-sizing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Deterministic sizing and limits calculator for AWS CodeBuild projects.

## Description
This MCP server provides precise calculations for AWS CodeBuild configurations. Use `calculate_project_constraints` to validate buildspec size and timeouts against hard AWS limits. Use `calculate_resource_sizing` to determine recommended storage, concurrency, and environment variable limits. Use `calculate_compute_and_config` to map memory requirements to specific AWS compute types like `BUILD_GENERAL1_SMALL` or `BUILD_GENERAL1_XLARGE` and configure VPC settings.


## Available Tools (3)
- **calculate_project_constraints**: Validates the buildspec and timeout against AWS hard limits
- **calculate_compute_and_config**: Maps resource requirements to specific AWS CodeBuild compute types and network configurations
- **calculate_resource_sizing**: Determines recommended storage, concurrency, and variable limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS CodeBuild Project Sizing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My buildspec is 70 KB. Is this valid for AWS CodeBuild?"

**🤖 AI Agent:**
> No, a buildspec size of 70 KB exceeds the hard limit of 64 KB and will cause the build to fail.

---

**👤 You:**
> "I need a build environment with 10 GB of RAM. What compute type should I use?"

**🤖 AI Agent:**
> For 10 GB of RAM, the recommended compute type is `BUILD_GENERAL1_LARGE`, which provides 15 GB of memory.

---

**👤 You:**
> "What is the recommended cache size for my CodeBuild project?"

**🤖 AI Agent:**
> A recommended cache size for CodeBuild projects is 100 GB.


## ❓ FAQ

**Q: How do I know if my buildspec is too large?**
You can use the `calculate_project_constraints` tool. It will check your buildspec size against the 64 KB hard limit and flag it if it exceeds the allowed value.

**Q: Can I run Docker builds with this tool?**
Yes. By using `calculate_compute_and_config`, you can specify if your build requires Docker. The tool will then determine if privileged mode is required for your configuration.

**Q: What are the concurrency limits for Linux builds?**
The `calculate_resource_sizing` tool will recommend a concurrency limit of 60 for Linux-based environments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-codebuild-project-sizing-calculator](https://vinkius.com/ai-agent-connect/aws-codebuild-project-sizing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS CodeBuild Project Sizing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-codebuild-project-sizing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS CodeBuild Project Sizing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-codebuild-project-sizing-calculator": {
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
