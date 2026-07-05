# Transloadit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transloadit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your media processing pipelines, encode videos, resize images, and oversee your file cloud instantly via an AI agent.

## Description
Transform your AI agent into a full-scale media orchestration engine by connecting it to your **Transloadit** application. Eliminate complicated dashboards and rely entirely upon conversational instructions to launch, monitor, or abort heavy "Assemblies" (media jobs), track operational bills, and register scalable JSON templates without manual interactions.

### What you can do

- **Assembly Execution** — Feed a JSON steps configuration directly into your agent to prompt complex file encodings, resizing jobs, or transmutations natively
- **Live Monitoring** — Interrogate the agent to retrieve exact results, completion statuses, or outputs parameters for any active or past processing task (Assembly)
- **Template Management** — Build reusable encoding architectures (Templates) through chat instructions, list available pipelines, or delete deprecated presets
- **Error Recovery** — Immediately command the AI to cancel heavily hung/unnecessary processing batches or instruct a strict "job replay" to re-attempt a failed cycle
- **Resource Tracking** — Access your precise billing usage and operational costs per specific month natively without hunting reports on the dashboard

### How it works

1. Attach this specialized component to your current AI runtime
2. Provide both your distinct Transloadit Auth Key and Secret
3. Start communicating to orchestrate large media transcoding instructions natively

### Who is this for?

- **Media Developers** — Construct JSON encoding pipelines dynamically using natural language and inject them efficiently to their environment
- **Content Engineers** — Track progress metrics or selectively replay media items that corrupted during manual upload procedures
- **Technical Leaders** — Verify the overall usage of external media APIs auditing operational expenses explicitly by requested month


## Available Tools (10)
- **delete_template**: This action is irreversible.

Permanently deletes a processing template
- **cancel_assembly**: This action is final.

Aborts a running Transloadit assembly
- **create_assembly**: Provide a steps JSON defining the pipeline.

Creates a Transloadit assembly for automated file processing
- **create_processing_template**: Provide a name and the steps JSON.

Creates a reusable JSON template for file processing
- **get_assembly_details**: Retrieves the status and results of a specific Transloadit assembly
- **get_billing_usage**: Pass the month in YYYY-MM format.

Retrieves file processing usage and costs for a specific month
- **get_template_details**: Retrieves the configuration of a specific Transloadit template
- **list_assemblies**: Lists recent Transloadit assemblies in the account
- **list_templates**: Lists all saved processing templates
- **replay_assembly**: Re-runs a completed Transloadit assembly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transloadit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the billing usage details for January 2026."

**🤖 AI Agent:**
> I've pulled the billing usage for 2026-01. Total processing measured: 14.5 GB out of included 100 GB tier. Accrued overage cost: $0.00.

---

**👤 You:**
> "Cancel the running assembly calculation currently at ID b13a4x2."

**🤖 AI Agent:**
> Assembly b13a4x2 cancellation confirmed. Processing nodes have been immediately stopped.


## ❓ FAQ

**Q: Where do I find my Auth Key and Auth Secret credentials?**
Navigate directly directly to the Transloadit web frontend. Open your Account settings. On the sidebar, click on **Credentials**. You will spot your public `Auth Key` directly exposed, and right next to it the option to reveal your `Auth Secret`. Both strings are required parameters here.

**Q: Does `cancel_assembly` action cost money if triggered early?**
Yes, absolutely. Halting an assembly stops Transloadit servers from expending gigabytes processing irrelevant files immediately. Consequently, acting rapidly prevents unnecessary overuse charges and quotas from draining. Use it when observing logical JSON mistakes.

**Q: Do I need Signature Authentication for Transloadit?**
Yes. For production environments, it is strongly recommended to use Signature Authentication to prevent unauthorized use. Your Transloadit MCP integration handles this internally using the provided Auth Secret to sign requests securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transloadit](https://vinkius.com/mcp/transloadit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transloadit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transloadit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transloadit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transloadit": {
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
