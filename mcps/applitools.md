# Applitools MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/applitools)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Bring AI-powered visual testing to your AI agent — inspect test batches, review UI diffs, and manage your visual baselines naturally.

## Description
Connect your **Applitools Eyes** testing suite to your AI agent and manage your entire visual regression pipeline without opening the dashboard. Allow your agent to spot UI changes, validate baselines, and assess testing health dynamically.

### What you can do

- **Batch Observability** — Query active test batches to view aggregated statuses (Passed, Failed, Unresolved) and completion rates
- **Session & Results analysis** — Drill down into specific test sessions to examine failed step images, match levels, and browser differences
- **Baseline Management** — List your "golden" graphical baselines bound to applications or specific Git branches
- **Actionable Maintenance** — Authorize the agent to delete outdated baselines or discard legacy batches to keep your workspace clean
- **Key Validation** — Ensure connectivity against your visual AI engine before pipeline triggers

### How it works

1. Subscribe to this server
2. Insert your Applitools API Key
3. Review visual bugs and validate frontend changes directly from Claude, Cursor, or any MCP-compatible surface

### Who is this for?

- **QA Automation Engineers** — ask your agent to summarize unresolved test batches and pinpoint exact OS/browser failure combinations
- **Frontend Developers** — verify branch-specific visual baselines during PRs without context switching
- **Engineering Managers** — pull high-level batch stats to ensure release criteria are visually met
- **Designers** — request a quick breakdown of structural UI changes caught by Applitools Visual AI before deployment


## Available Tools (10)
- **list_baselines**: Returns baseline IDs, names, and env configs. Filter by app name.

List visual baselines for an app on Applitools
- **get_batch_stats**: Returns passed/failed/unresolved/new counts without full test data.

Get summary statistics for an Applitools batch
- **list_batches**: Batches group related test sessions. Returns batch IDs, names, statuses (Passed/Unresolved/Failed), and test counts. Each batch has a unique ID used to query its results.

List all test batches on Applitools Eyes
- **list_branch_baselines**: Use to inspect branch-specific visual states.

List baselines for a specific branch on Applitools
- **delete_baseline**: Use when a baseline is outdated or a page has been redesigned.

Delete an Applitools test baseline
- **delete_batch**: Does NOT affect baselines. Use with caution — this is irreversible.

Delete an Applitools test batch
- **get_batch**: Use batch ID from list_batches.

Get full details of an Applitools batch
- **list_results**: List all test results in an Applitools batch
- **get_session**: Provide batch ID and session ID.

Get details of a test session within an Applitools batch
- **validate_key**: Use to verify connectivity before running tests.

Validate the Applitools API key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Applitools** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent visual test batches in Applitools."

**🤖 AI Agent:**
> You have 3 recent batches. 'V2 Checkout Redesign' (ID: b_991x) is currently Unresolved. 'Marketing Footer Fix' (ID: b_882y) has Passed completely. 'Login Dropdown' (ID: b_773z) contains 2 Failed sessions. Would you like to inspect the failures in the Login Dropdown batch?

---

**👤 You:**
> "Get me the exact session results for our unresolved batch ID b_991x."

**🤖 AI Agent:**
> Checking batch b_991x 'V2 Checkout Redesign'. There are 4 unresolved sessions out of 10. The main mismatch occurs on the 'Payment Modal' step across Chrome 114 (Windows) and Safari 16 (iOS). The Applitools AI noticed a 12% pixel drift in the button alignment. Should I generate the links to view the diffs?

---

**👤 You:**
> "List the baselines assigned specifically to fixing the 'feature/dark-mode-header' branch."

**🤖 AI Agent:**
> I found 2 baselines associated with 'feature/dark-mode-header'. Baseline ID: bs_4ab (Nav Bar Base) and Baseline ID: bs_5cd (Mobile Hamburger Dark). They appear to have been created 3 days ago. Are these outdated, and would you like me to delete them?


## ❓ FAQ

**Q: Can my AI agent resolve a test failure on its own?**
No. The MCP server is designed for pulling state data—it retrieves batches, session diff links, and match levels so you can review them locally. Approving a new baseline or resolving a mismatch still requires human intervention within the Applitools Eyes dashboard to maintain absolute testing safety.

**Q: Can I use the agent to delete old UI snapshots?**
Yes. If your UI has undergone major structural changes and old baselines are causing false positives, you can authorize the agent to execute the `delete_baseline` tool. Provide the exact baseline ID to instantly discard the legacy screenshot from your workspace.

**Q: How fast can I summarize test errors after my CI/CD action triggers?**
Almost instantly. Rather than scrolling through dozens of Applitools logs, ask your agent to 'Get batch stats for ID 123'. It will immediately return the aggregation of Passed, Failed, and Unresolved runs, saving you countless minutes of digging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/applitools](https://vinkius.com/mcp/applitools)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Applitools** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `applitools` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Applitools** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "applitools": {
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
