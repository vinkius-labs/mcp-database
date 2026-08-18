# AWS Secrets Manager Rotation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-secrets-manager-rotation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Validate AWS Secrets Manager configurations against operational limits and rotation best practices.

## Description
This MCP server provides a deterministic way to validate AWS Secrets Manager configurations. It ensures your secrets comply with hard AWS limits, such as the 64 KB size constraint, and helps plan rotation schedules. Use `validate_secret_constraints` to check name and size limits, `calculate_rotation_parameters` to verify if rotation frequency and Lambda duration meet high-security standards, and `estimate_resource_usage` to project policy sizes and replication status. It also provides essential guidance on recovery windows and cross-account sharing via RAM.


## Available Tools (4)
- **calculate_rotation_parameters**: Determines if the rotation schedule and Lambda configuration meet operational safety and frequency requirements
- **estimate_resource_usage**: Provides recommendations and estimates for versions, policies, and replication based on the scale of the secrets deployment
- **get_lifecycle_and_sharing_guidelines**: Returns standard guidance for recovery windows and cross-account sharing limits
- **validate_secret_constraints**: Checks if the provided secret configuration violates hard AWS limits for size and name length


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Secrets Manager Rotation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my secret named 'prod/api/key' with a size of 50 KB valid?"

**🤖 AI Agent:**
> Yes, the secret name and size are within the allowed AWS limits.

---

**👤 You:**
> "Calculate rotation parameters for a rotation every 2 days and a Lambda duration of 300 seconds."

**🤖 AI Agent:**
> The rotation frequency is not compliant with high-security standards (which require 4 hours or less), but the Lambda duration is within the 900-second limit.

---

**👤 You:**
> "Estimate resource usage for 50 secrets replicated across 3 regions."

**🤖 AI Agent:**
> The estimated total policy size is 1000 KB. The requested replication is within the 5-region limit.


## ❓ FAQ

**Q: What is the maximum size for an AWS secret?**
The maximum size for an individual AWS secret is 64 KB. You can use `validate_secret_constraints` to check if your secret size is within this limit.

**Q: How often should I rotate my secrets?**
For high-security standards, rotation should occur every 4 hours or less. The `calculate_rotation_parameters` tool can help you determine if your schedule is compliant.

**Q: How many versions can a secret have?**
While AWS does not enforce a hard limit, it is recommended to stay within 100 versions per secret for better manageability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-secrets-manager-rotation-calculator](https://vinkius.com/ai-agent-connect/aws-secrets-manager-rotation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Secrets Manager Rotation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-secrets-manager-rotation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Secrets Manager Rotation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-secrets-manager-rotation-calculator": {
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
