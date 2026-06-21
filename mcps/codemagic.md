# Codemagic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/codemagic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate mobile CI/CD workflows — trigger builds, manage artifacts, and update environment variables directly from your AI agent.

## Description
Connect your **Codemagic** account to any AI agent and streamline your mobile application delivery pipeline through natural language commands.

### What you can do

- **Build Orchestration** — Start new builds for specific apps and workflows, with the ability to override branches, tags, and machine instances.
- **Build Control** — Instantly cancel ongoing builds that are no longer needed to save resources and time.
- **Artifact Management** — Retrieve authenticated download URLs for build outputs or generate temporary public links for external stakeholders.
- **Environment Configuration** — Programmatically add variables or secrets to your variable groups (v3 API) to keep your CI/CD environment up to date.
- **Workflow Customization** — Pass custom labels and environment overrides to tailor builds for specific testing or release scenarios.

### How it works

1. Subscribe to this server
2. Enter your Codemagic API Token
3. Start managing your mobile pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mobile Developers** — trigger builds and check artifact status without leaving your code editor.
- **DevOps Engineers** — automate the management of environment variables and build labels across multiple applications.
- **Release Managers** — generate public download links for QA teams or stakeholders instantly via chat.


## Available Tools
- **add_variables_to_group**: Add variables to a variable group
- **cancel_build**: Cancel a Codemagic build
- **create_public_artifact_url**: Create a public download URL for an artifact
- **get_artifact**: Get authenticated download URL for an artifact
- **start_build**: Overrides trigger/branch configs.

Start a new Codemagic build


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Codemagic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start a new build for app '642a1b2c3d4e5f' using the 'release-workflow' on the 'main' branch."

**🤖 AI Agent:**
> I've triggered the build for you. The build process has started for the 'main' branch using the specified workflow. You can track its progress in your Codemagic dashboard.

---

**👤 You:**
> "Generate a public download link for the artifact at 'build/outputs/app-release.ipa' that expires in 24 hours."

**🤖 AI Agent:**
> I've generated a temporary public URL for your artifact. It will be valid for the next 24 hours: [URL].

---

**👤 You:**
> "Add a secure variable 'API_KEY' with value 'secret123' to the variable group 'prod-secrets'."

**🤖 AI Agent:**
> The secure variable 'API_KEY' has been successfully added to the 'prod-secrets' group.


## ❓ FAQ

**Q: Can I trigger a build for a specific branch or tag using the AI?**
Yes! Use the `start_build` tool and provide the `appId`, `workflowId`, and either the `branch` or `tag` name. You can even specify the `instanceType` if you need a specific build machine.

**Q: How do I share a build artifact with someone who doesn't have a Codemagic account?**
You can use the `create_public_artifact_url` tool. Provide the artifact `path` and a UNIX timestamp for `expires_at`. The agent will generate a temporary public link for you.

**Q: Is it possible to update environment secrets safely?**
Absolutely. The `add_variables_to_group` tool allows you to add variables to a group. By setting the `secure` parameter to true, your variables will be encrypted as secrets in Codemagic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/codemagic](https://vinkius.com/mcp/codemagic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Codemagic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `codemagic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Codemagic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "codemagic": {
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
